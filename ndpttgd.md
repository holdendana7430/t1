代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bb.gzmigu.cn

[Q58] 累计求和
来源：http://aw.9csxet.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sb.szsharing.cn

[Q59] 分组内累计
来源：http://oj.wgjwhj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kz.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://ru.shxzskj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xb.yuexingan06.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gu.bjjhwx.cn

[Q61] 移动平均
来源：http://wn.gzmigu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hq.huanxung.cn

[Q62] 分组占比
来源：http://sz.yuexingan06.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xv.colortex.cn

[Q63] 开启事务
来源：http://cv.nicolike.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://da.yuexingan06.cn

[Q64] 提交事务
来源：http://fk.bookmarksfly.cn

COMMIT;
来源：http://aj.huixinmuqiang.cn

[Q65] 回滚事务
来源：http://ey.gzmigu.cn

ROLLBACK;
来源：http://rp.newstarts.cn

[Q66] 行锁查询
来源：http://bu.panjiajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://az.jctech888.com.cn

[Q67] 设置隔离级别
来源：http://mv.jctech888.com.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bw.jctech888.com.cn

[Q68] 保存点
来源：http://zn.szsharing.cn

SAVEPOINT sp1;
来源：http://hc.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://dn.lnxyls.cn

[Q69] 查看执行计划
来源：http://mj.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://je.bjjhwx.cn

[Q70] 更新统计信息
来源：http://cf.huixiangedu.cn

ANALYZE TABLE users;
来源：http://tz.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://ki.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cc.hahajie.cn

[Q72] 查看索引
来源：http://tz.9csxet.cn

SHOW INDEX FROM users;
来源：http://pq.asd995.cn

[Q73] 查看表状态
来源：http://lp.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nx.yuexingan06.cn

[Q74] 强制使用索引
来源：http://jm.hahajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kw.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://kw.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fa.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ea.hahajie.cn

[Q76] 按天统计
来源：http://yt.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tm.yuexingan06.cn

[Q77] 时间加减
来源：http://jp.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xn.yuexingan06.cn

[Q78] 当前时间
来源：http://bt.yuexingan06.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iy.szsharing.cn

[Q79] 字符串拼接
来源：http://mf.haigaiapp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://na.lnxyls.cn

[Q80] 字符串截取
来源：http://ir.newstarts.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ro.panjiajie.cn

[Q81] 字符串替换
来源：http://na.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ys.521024.cn

[Q82] 字符长度与字节长度
来源：http://kd.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oh.9csxet.cn

[Q83] 大小写转换
来源：http://tu.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kp.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://du.jctech888.com.cn

SELECT TRIM(name) FROM users;
来源：http://qt.jianghongdianzi.cn

[Q85] 数值取整
来源：http://au.shxzskj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://li.jianghongdianzi.cn

[Q86] 读取 JSON 字段
来源：http://ro.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wl.colortex.cn

[Q87] JSON 字段做条件
来源：http://na.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cr.gzmigu.cn

[Q88] 行转列（条件聚合）
来源：http://lv.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mh.yuntaijiaju.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xb.521024.cn

[Q89] 判断表是否存在
来源：http://id.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://og.shxzukj.cn

[Q90] 生成序号列
来源：http://gy.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dh.yuntaijiaju.cn

================================================================================
来源：http://rd.jianghongdianzi.cn

R. Bash 专题
来源：http://ww.huanxung.cn

================================================================================
来源：http://fr.9csxet.cn

[R01] shebang 与严格模式
来源：http://mf.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://xc.bjjhwx.cn

set -euo pipefail
来源：http://ps.nicolike.cn

[R02] 变量赋值与使用
来源：http://qv.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://gt.asd995.cn

[R03] 只读变量
来源：http://kr.szxytkj.cn

readonly PI=3.14
来源：http://su.nszjky.cn

[R04] 位置参数
来源：http://la.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jm.bjjhwx.cn

[R05] 参数默认值
来源：http://as.szsharing.cn

name="${1:-default}"
来源：http://vd.wgjwhj.cn

[R06] 判断命令是否存在
来源：http://dc.lnxyls.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iz.gzmigu.cn

[R07] if 判断文件
来源：http://gx.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xx.nszjky.cn

[R08] 数值比较
来源：http://ew.shxzukj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wb.huixinmuqiang.cn

[R09] 字符串比较
来源：http://bw.huixinmuqiang.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mc.bjjhwx.cn

[R10] 正则匹配
来源：http://cx.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nu.haigaiapp.cn

[R11] case 多分支
来源：http://rg.panjiajie.cn

case "$1" in
来源：http://fx.szsharing.cn

start) echo "启动" ;;
来源：http://wf.jctech888.com.cn

stop)  echo "停止" ;;
来源：http://zw.huanxung.cn

*)     echo "未知命令" ;;
来源：http://ew.nicolike.cn

esac
来源：http://lq.newstarts.cn

[R12] for 遍历文件
来源：http://mk.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://zg.gzmigu.cn

[R13] for 计数循环
来源：http://pf.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://vr.jctech888.com.cn

[R14] C 风格 for
来源：http://do.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tx.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://fb.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nz.bookmarksfly.cn

[R16] until 等待条件
来源：http://ly.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lg.hahajie.cn

[R17] 数组定义与取值
来源：http://sr.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ur.bookmarksfly.cn

[R18] 遍历数组
来源：http://kw.szsharing.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://re.bookmarksfly.cn

[R19] 数组长度
来源：http://bs.gzmigu.cn

echo "${#arr[@]}"
来源：http://ig.nicolike.cn

[R20] 关联数组（字典）
来源：http://fn.newstarts.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sr.muxihuayi.cn

[R21] 字符串长度
来源：http://mu.haigaiapp.cn

echo "${#s}"
来源：http://la.szsharing.cn

[R22] 截取子串
来源：http://oe.521024.cn

echo "${s:0:5}"
来源：http://yq.wgjwhj.cn

[R23] 字符串替换
来源：http://cj.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hi.huixiangedu.cn

[R24] 大小写转换
来源：http://pg.yuexingan06.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hl.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://ml.jianghongdianzi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ec.nszjky.cn

[R26] 命令替换
来源：http://yi.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://yy.yuntaijiaju.cn

[R27] 算术展开
来源：http://sz.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://df.haigaiapp.cn

[R28] 浮点运算
来源：http://ae.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://nf.nszjky.cn

[R29] 定义函数
来源：http://qu.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zv.yuexingan06.cn

[R30] 函数返回状态码
来源：http://gi.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://ai.hnjuh.cn

[R31] 局部变量
来源：http://br.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://ca.huixiangedu.cn

[R32] 参数个数校验
来源：http://sj.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ht.huixiangedu.cn

[R33] 捕获错误并提示行号
来源：http://xc.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ju.yuexingan06.cn

[R34] 退出时清理
来源：http://ia.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fu.bjjhwx.cn

[R35] 后台执行并等待
来源：http://oq.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lm.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://za.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sd.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://ss.panjiajie.cn

files=$(ls -1)
来源：http://lk.nszjky.cn

[R38] 管道串联
来源：http://sd.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://ut.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://br.hnjuh.cn

cmd > out.log 2>&1
来源：http://by.chemitech.net.cn

[R40] 追加写日志
来源：http://db.huixinmuqiang.cn

echo "log" >> out.log
来源：http://fn.shxzukj.cn

[R41] 丢弃输出
来源：http://gt.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://jw.haigaiapp.cn

[R42] 输入重定向
来源：http://mr.asd995.cn

wc -l < a.txt
来源：http://yw.wgjwhj.cn

[R43] 按名字查找文件
来源：http://vm.yuexingan06.cn

find . -name "*.log" -type f
来源：http://ni.huixiangedu.cn

[R44] 按修改时间查找
来源：http://cn.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://cc.hahajie.cn

[R45] 批量删除
来源：http://un.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://gv.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://jr.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vi.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://jh.haigaiapp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lf.chemitech.net.cn

[R48] awk 取指定列
来源：http://tf.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://sr.lnxyls.cn

[R49] awk 带条件
来源：http://lx.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dj.jianghongdianzi.cn

[R50] awk 求和
来源：http://wr.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jf.nszjky.cn

[R51] 排序去重取前几
来源：http://wp.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mn.jctech888.com.cn

[R52] 统计行数
来源：http://cl.colortex.cn

wc -l a.txt
来源：http://dt.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://qt.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pl.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://uz.huixiangedu.cn

diff a.txt b.txt
来源：http://vs.hahajie.cn

[R55] 压缩与解压
来源：http://wp.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ba.shtwfgs.cn

[R56] 远程拷贝
来源：http://mh.bjjhwx.cn

scp file user@host:/path/
来源：http://ei.bookmarksfly.cn

[R57] 远程执行命令
来源：http://lm.haigaiapp.cn

ssh user@host 'uptime'
来源：http://zc.gzmigu.cn

[R58] 下载文件
来源：http://yx.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://st.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://rj.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://it.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://zu.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://il.bjjhwx.cn

[R61] 磁盘占用
来源：http://ui.shxzukj.cn

df -h;  du -sh *
来源：http://ua.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://wa.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://kf.shxzskj.cn

[R63] 内存与进程
来源：http://rv.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://av.shtwfgs.cn

[R64] 结束进程
来源：http://il.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://zz.huixiangedu.cn

[R65] 查看端口占用
来源：http://nr.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dq.huixinmuqiang.cn

[R66] 定时任务
来源：http://ys.shxzskj.cn

crontab -e;  crontab -l
来源：http://fk.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://cu.hahajie.cn

openssl rand -hex 16
来源：http://lu.szxytkj.cn

[R68] 计算文件校验值
来源：http://qb.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://db.haigaiapp.cn

[R69] 生成随机密码
来源：http://ef.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ke.nszjky.cn

[R70] 时间戳与互转
来源：http://ti.nicolike.cn

date +%s;  date -d @1700000000
来源：http://yc.hnjuh.cn

[R71] 日期格式化
来源：http://zz.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zk.chemitech.net.cn

[R72] 等待端口就绪
来源：http://qk.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qu.szsharing.cn

[R73] 分割大日志
来源：http://zw.shxzskj.cn

split -l 1000 big.log part_
来源：http://gg.bookmarksfly.cn

[R74] 批量重命名
来源：http://qp.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vx.huixiangedu.cn

[R75] 导出环境变量
来源：http://pk.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://af.panjiajie.cn

[R76] 使用临时文件
来源：http://pf.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://io.asd995.cn

[R77] 读取用户输入
来源：http://in.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ed.bjjhwx.cn

[R78] 交互式菜单
来源：http://sh.shxzukj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://di.newstarts.cn

[R79] 解析命令行选项
来源：http://yc.newstarts.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ay.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://dy.lnxyls.cn

time ./run.sh
来源：http://yj.asd995.cn

================================================================================
来源：http://zj.hahajie.cn

S. C / C++ 专题
来源：http://vs.jianghongdianzi.cn

================================================================================
来源：http://vq.jianghongdianzi.cn

[S01] C：Hello World
来源：http://lk.muxihuayi.cn

#include <stdio.h>
来源：http://gr.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uf.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://on.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://wv.panjiajie.cn

[S03] C：读入整数
来源：http://yv.9csxet.cn

int x; scanf("%d", &x);
来源：http://yc.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://ic.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://df.colortex.cn

[S05] C：字符串长度
来源：http://hx.huixinmuqiang.cn

strlen(s)
来源：http://dk.shtwfgs.cn

[S06] C：字符串比较
来源：http://wl.panjiajie.cn

strcmp(a, b) == 0
来源：http://gz.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://yu.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ca.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://xw.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ch.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://yw.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lp.huanxung.cn

[S10] C：指针与解引用
来源：http://vh.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://bx.chemitech.net.cn

[S11] C：逐行读文件
来源：http://co.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xw.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fm.gzmigu.cn

fclose(f);
来源：http://xa.szsharing.cn

[S12] C：写文件
来源：http://qv.yuntaijiaju.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lt.huixiangedu.cn

[S13] C：宏定义
来源：http://ii.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jy.gzmigu.cn

[S14] C：枚举
来源：http://qv.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://mp.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ep.panjiajie.cn

(double) a / b
来源：http://ug.yuexingan06.cn

[S16] C：位操作置位
来源：http://lc.lnxyls.cn

x |= (1 << 3);
来源：http://nd.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://qr.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lk.huanxung.cn

[S18] C：命令行参数
来源：http://dq.colortex.cn

int main(int argc, char **argv)
来源：http://hq.szsharing.cn

[S19] C：快速排序
来源：http://mo.lnxyls.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fp.huixiangedu.cn

[S20] C：二分查找
来源：http://rk.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ei.asd995.cn

[S21] C：字符类别判断
来源：http://il.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://th.huixiangedu.cn

[S22] C：字符串转数字
来源：http://kd.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rq.lnxyls.cn

[S23] C：随机数
来源：http://pt.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dt.shxzskj.cn

[S24] C：获取本地时间
来源：http://ol.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ki.gzmigu.cn

[S25] C：内存拷贝
来源：http://xc.chemitech.net.cn

memcpy(dst, src, n);
来源：http://rc.yuntaijiaju.cn

[S26] C：内存清零
来源：http://oz.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://pj.lnxyls.cn

[S27] C：定义常量
来源：http://fa.szsharing.cn

const double PI = 3.14159;
来源：http://fb.9csxet.cn

[S28] C：静态变量
来源：http://pa.huixinmuqiang.cn


<!-- 参考信息 -->