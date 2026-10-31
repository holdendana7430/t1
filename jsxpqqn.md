代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wt.szxytkj.cn

[Q58] 累计求和
来源：http://yu.521024.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://df.yuexingan06.cn

[Q59] 分组内累计
来源：http://ea.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ju.shxzskj.cn

[Q60] 取上一行 / 下一行
来源：http://rf.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gp.bjjhwx.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sc.nicolike.cn

[Q61] 移动平均
来源：http://lo.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qk.jctech888.com.cn

[Q62] 分组占比
来源：http://gg.jianghongdianzi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://az.panjiajie.cn

[Q63] 开启事务
来源：http://zj.huixinmuqiang.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ir.bjjhwx.cn

[Q64] 提交事务
来源：http://zx.jianghongdianzi.cn

COMMIT;
来源：http://aj.shxzukj.cn

[Q65] 回滚事务
来源：http://ds.newstarts.cn

ROLLBACK;
来源：http://eu.huixiangedu.cn

[Q66] 行锁查询
来源：http://yz.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tw.asd995.cn

[Q67] 设置隔离级别
来源：http://mc.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hv.chemitech.net.cn

[Q68] 保存点
来源：http://po.panjiajie.cn

SAVEPOINT sp1;
来源：http://yr.hnjuh.cn

ROLLBACK TO sp1;
来源：http://eo.huanxung.cn

[Q69] 查看执行计划
来源：http://rc.shxzskj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cc.chemitech.net.cn

[Q70] 更新统计信息
来源：http://fj.wgjwhj.cn

ANALYZE TABLE users;
来源：http://ml.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://mm.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ec.shxzukj.cn

[Q72] 查看索引
来源：http://jy.shxzskj.cn

SHOW INDEX FROM users;
来源：http://mv.huixiangedu.cn

[Q73] 查看表状态
来源：http://hu.muxihuayi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gm.hahajie.cn

[Q74] 强制使用索引
来源：http://cq.9csxet.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://od.asd995.cn

[Q75] 日期格式化
来源：http://dk.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cd.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ar.hnjuh.cn

[Q76] 按天统计
来源：http://ph.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://db.nicolike.cn

[Q77] 时间加减
来源：http://uj.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://il.haigaiapp.cn

[Q78] 当前时间
来源：http://so.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hj.newstarts.cn

[Q79] 字符串拼接
来源：http://ra.yuntaijiaju.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jd.asd995.cn

[Q80] 字符串截取
来源：http://nl.chemitech.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://od.521024.cn

[Q81] 字符串替换
来源：http://oq.nszjky.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zl.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://cj.haigaiapp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ox.colortex.cn

[Q83] 大小写转换
来源：http://kw.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xj.hnjuh.cn

[Q84] 去除首尾空格
来源：http://ym.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://nk.szsharing.cn

[Q85] 数值取整
来源：http://at.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wo.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://yo.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qm.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://bn.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nt.shxzukj.cn

[Q88] 行转列（条件聚合）
来源：http://fk.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yx.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ok.asd995.cn

[Q89] 判断表是否存在
来源：http://ad.huanxung.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xu.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://jp.jianghongdianzi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gq.wgjwhj.cn

================================================================================
来源：http://vd.bjjhwx.cn

R. Bash 专题
来源：http://ac.szsharing.cn

================================================================================
来源：http://is.muxihuayi.cn

[R01] shebang 与严格模式
来源：http://ov.jctech888.com.cn

#!/usr/bin/env bash
来源：http://ag.yuexingan06.cn

set -euo pipefail
来源：http://ic.521024.cn

[R02] 变量赋值与使用
来源：http://kj.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://jg.huanxung.cn

[R03] 只读变量
来源：http://ml.shtwfgs.cn

readonly PI=3.14
来源：http://ce.nszjky.cn

[R04] 位置参数
来源：http://mi.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tj.shxzskj.cn

[R05] 参数默认值
来源：http://yo.huixinmuqiang.cn

name="${1:-default}"
来源：http://pa.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://kj.nszjky.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lc.nicolike.cn

[R07] if 判断文件
来源：http://hs.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://de.bjjhwx.cn

[R08] 数值比较
来源：http://hz.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mw.panjiajie.cn

[R09] 字符串比较
来源：http://zk.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pl.bookmarksfly.cn

[R10] 正则匹配
来源：http://no.shxzukj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rh.wgjwhj.cn

[R11] case 多分支
来源：http://gw.bjjhwx.cn

case "$1" in
来源：http://mb.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://bg.huanxung.cn

stop)  echo "停止" ;;
来源：http://qg.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://kn.chemitech.net.cn

esac
来源：http://ul.muxihuayi.cn

[R12] for 遍历文件
来源：http://mb.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://zn.newstarts.cn

[R13] for 计数循环
来源：http://ej.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://xy.nszjky.cn

[R14] C 风格 for
来源：http://lo.szxytkj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bk.haigaiapp.cn

[R15] while 逐行读文件
来源：http://tq.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rl.huixiangedu.cn

[R16] until 等待条件
来源：http://cj.yuntaijiaju.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://an.muxihuayi.cn

[R17] 数组定义与取值
来源：http://ak.newstarts.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gf.9csxet.cn

[R18] 遍历数组
来源：http://jd.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://an.szxytkj.cn

[R19] 数组长度
来源：http://ox.szsharing.cn

echo "${#arr[@]}"
来源：http://yd.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://tw.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gr.huanxung.cn

[R21] 字符串长度
来源：http://px.bjjhwx.cn

echo "${#s}"
来源：http://og.panjiajie.cn

[R22] 截取子串
来源：http://wa.nszjky.cn

echo "${s:0:5}"
来源：http://qy.huixiangedu.cn

[R23] 字符串替换
来源：http://cm.jctech888.com.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dt.huixiangedu.cn

[R24] 大小写转换
来源：http://bq.chemitech.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://np.521024.cn

[R25] 去后缀 / 去前缀
来源：http://xf.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fl.chemitech.net.cn

[R26] 命令替换
来源：http://ed.colortex.cn

now=$(date +%F); echo "$now"
来源：http://hz.nicolike.cn

[R27] 算术展开
来源：http://bb.colortex.cn

echo $((1 + 2 * 3))
来源：http://ps.haigaiapp.cn

[R28] 浮点运算
来源：http://hi.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://is.asd995.cn

[R29] 定义函数
来源：http://gk.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hb.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://kc.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://my.huixiangedu.cn

[R31] 局部变量
来源：http://my.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://yw.szsharing.cn

[R32] 参数个数校验
来源：http://hy.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nd.huixinmuqiang.cn

[R33] 捕获错误并提示行号
来源：http://bv.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rp.bjjhwx.cn

[R34] 退出时清理
来源：http://xe.9csxet.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gi.521024.cn

[R35] 后台执行并等待
来源：http://mz.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hu.jianghongdianzi.cn

[R36] 并发执行多个任务
来源：http://bm.shxzskj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sy.szxytkj.cn

[R37] 把输出赋给变量
来源：http://ex.newstarts.cn

files=$(ls -1)
来源：http://ck.panjiajie.cn

[R38] 管道串联
来源：http://hx.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://aq.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://ar.521024.cn

cmd > out.log 2>&1
来源：http://lu.nszjky.cn

[R40] 追加写日志
来源：http://in.szxytkj.cn

echo "log" >> out.log
来源：http://rl.panjiajie.cn

[R41] 丢弃输出
来源：http://ys.newstarts.cn

cmd >/dev/null 2>&1
来源：http://nx.521024.cn

[R42] 输入重定向
来源：http://jh.shxzskj.cn

wc -l < a.txt
来源：http://hi.lnxyls.cn

[R43] 按名字查找文件
来源：http://us.muxihuayi.cn

find . -name "*.log" -type f
来源：http://lc.shxzskj.cn

[R44] 按修改时间查找
来源：http://xj.gzmigu.cn

find . -mtime -7 -type f
来源：http://vf.bookmarksfly.cn

[R45] 批量删除
来源：http://cj.haigaiapp.cn

find . -name "*.tmp" -delete
来源：http://nq.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://cr.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eu.lnxyls.cn

[R47] sed 单行替换
来源：http://jp.shxzskj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zm.nszjky.cn

[R48] awk 取指定列
来源：http://jd.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://dz.hahajie.cn

[R49] awk 带条件
来源：http://jy.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mn.huixinmuqiang.cn

[R50] awk 求和
来源：http://mx.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vi.521024.cn

[R51] 排序去重取前几
来源：http://qe.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ul.yuntaijiaju.cn

[R52] 统计行数
来源：http://zj.yuexingan06.cn

wc -l a.txt
来源：http://iq.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://qu.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xb.nicolike.cn

[R54] 比较两个文件
来源：http://qb.shtwfgs.cn

diff a.txt b.txt
来源：http://wl.huixiangedu.cn

[R55] 压缩与解压
来源：http://ek.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bq.huixiangedu.cn

[R56] 远程拷贝
来源：http://do.shtwfgs.cn

scp file user@host:/path/
来源：http://zl.yuexingan06.cn

[R57] 远程执行命令
来源：http://zp.haigaiapp.cn

ssh user@host 'uptime'
来源：http://fo.szxytkj.cn

[R58] 下载文件
来源：http://aq.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oz.szsharing.cn

[R59] 发 POST JSON
来源：http://gg.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nu.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://zu.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vo.asd995.cn

[R61] 磁盘占用
来源：http://jd.panjiajie.cn

df -h;  du -sh *
来源：http://qt.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://yw.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://ao.wgjwhj.cn

[R63] 内存与进程
来源：http://wv.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://vh.jianghongdianzi.cn

[R64] 结束进程
来源：http://jt.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://du.colortex.cn

[R65] 查看端口占用
来源：http://no.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ap.shxzskj.cn

[R66] 定时任务
来源：http://qs.nszjky.cn

crontab -e;  crontab -l
来源：http://ul.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://tf.jianghongdianzi.cn

openssl rand -hex 16
来源：http://rt.haigaiapp.cn

[R68] 计算文件校验值
来源：http://cn.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ys.shxzukj.cn

[R69] 生成随机密码
来源：http://qy.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://uu.colortex.cn

[R70] 时间戳与互转
来源：http://qq.newstarts.cn

date +%s;  date -d @1700000000
来源：http://sl.wgjwhj.cn

[R71] 日期格式化
来源：http://to.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xq.yuexingan06.cn

[R72] 等待端口就绪
来源：http://xo.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gp.nszjky.cn

[R73] 分割大日志
来源：http://lf.hnjuh.cn

split -l 1000 big.log part_
来源：http://xi.yuntaijiaju.cn

[R74] 批量重命名
来源：http://jt.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://me.hnjuh.cn

[R75] 导出环境变量
来源：http://fm.521024.cn

export PATH="$HOME/bin:$PATH"
来源：http://sb.bookmarksfly.cn

[R76] 使用临时文件
来源：http://uy.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ld.hnjuh.cn

[R77] 读取用户输入
来源：http://cs.colortex.cn

read -rp "请输入: " ans
来源：http://el.shxzskj.cn

[R78] 交互式菜单
来源：http://jg.huixiangedu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lg.nszjky.cn

[R79] 解析命令行选项
来源：http://yr.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ke.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://jv.szxytkj.cn

time ./run.sh
来源：http://sg.shxzskj.cn

================================================================================
来源：http://wf.hahajie.cn

S. C / C++ 专题
来源：http://qu.shxzskj.cn

================================================================================
来源：http://wn.jianghongdianzi.cn

[S01] C：Hello World
来源：http://oh.nicolike.cn

#include <stdio.h>
来源：http://zf.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vo.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ef.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://zl.szxytkj.cn

[S03] C：读入整数
来源：http://kr.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://zl.yuexingan06.cn

[S04] C：字符串复制
来源：http://sd.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://an.gzmigu.cn

[S05] C：字符串长度
来源：http://qw.hahajie.cn

strlen(s)
来源：http://kj.gzmigu.cn

[S06] C：字符串比较
来源：http://mh.nicolike.cn

strcmp(a, b) == 0
来源：http://bx.521024.cn

[S07] C：数组遍历求和
来源：http://ix.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qp.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://uv.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xh.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://lg.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cv.lnxyls.cn

[S10] C：指针与解引用
来源：http://qd.nicolike.cn

int *p = &a;  *p = 5;
来源：http://xd.wgjwhj.cn

[S11] C：逐行读文件
来源：http://nb.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://fd.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ra.shxzukj.cn

fclose(f);
来源：http://gj.szsharing.cn

[S12] C：写文件
来源：http://hh.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wz.9csxet.cn

[S13] C：宏定义
来源：http://fd.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aw.bjjhwx.cn

[S14] C：枚举
来源：http://az.jctech888.com.cn

enum Color { RED, GREEN, BLUE };
来源：http://fi.hnjuh.cn

[S15] C：类型转换
来源：http://xf.bjjhwx.cn

(double) a / b
来源：http://xv.gzmigu.cn

[S16] C：位操作置位
来源：http://nu.yuexingan06.cn

x |= (1 << 3);
来源：http://hd.nicolike.cn

[S17] C：安全拼接字符串
来源：http://th.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vv.muxihuayi.cn

[S18] C：命令行参数
来源：http://wi.bjjhwx.cn

int main(int argc, char **argv)
来源：http://ma.chemitech.net.cn

[S19] C：快速排序
来源：http://ro.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rn.yuntaijiaju.cn

[S20] C：二分查找
来源：http://dd.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nt.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://me.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ea.newstarts.cn

[S22] C：字符串转数字
来源：http://xd.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://md.yuexingan06.cn

[S23] C：随机数
来源：http://bh.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yg.szxytkj.cn

[S24] C：获取本地时间
来源：http://lv.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jy.szxytkj.cn

[S25] C：内存拷贝
来源：http://ai.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://mk.chemitech.net.cn

[S26] C：内存清零
来源：http://ls.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://hw.nicolike.cn

[S27] C：定义常量
来源：http://mg.asd995.cn

const double PI = 3.14159;
来源：http://ot.newstarts.cn

[S28] C：静态变量
来源：http://lr.panjiajie.cn


<!-- 参考信息 -->