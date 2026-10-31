代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vs.hnjuh.cn

[Q58] 累计求和
来源：http://kp.chemitech.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sb.jianghongdianzi.cn

[Q59] 分组内累计
来源：http://yk.shxzskj.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ys.asd995.cn

[Q60] 取上一行 / 下一行
来源：http://ho.hahajie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vo.nicolike.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pk.gzmigu.cn

[Q61] 移动平均
来源：http://mf.huixiangedu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mn.bjjhwx.cn

[Q62] 分组占比
来源：http://kf.asd995.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gc.shxzukj.cn

[Q63] 开启事务
来源：http://fv.yuntaijiaju.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xm.huixiangedu.cn

[Q64] 提交事务
来源：http://jp.jctech888.com.cn

COMMIT;
来源：http://wp.gzmigu.cn

[Q65] 回滚事务
来源：http://ib.shxzskj.cn

ROLLBACK;
来源：http://du.wgjwhj.cn

[Q66] 行锁查询
来源：http://jo.szsharing.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qs.colortex.cn

[Q67] 设置隔离级别
来源：http://uj.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ko.muxihuayi.cn

[Q68] 保存点
来源：http://jt.gzmigu.cn

SAVEPOINT sp1;
来源：http://gd.yuexingan06.cn

ROLLBACK TO sp1;
来源：http://gc.szsharing.cn

[Q69] 查看执行计划
来源：http://vf.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sj.shtwfgs.cn

[Q70] 更新统计信息
来源：http://rq.gzmigu.cn

ANALYZE TABLE users;
来源：http://py.shxzukj.cn

[Q71] 查看建表语句
来源：http://dd.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zh.newstarts.cn

[Q72] 查看索引
来源：http://gt.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://xi.haigaiapp.cn

[Q73] 查看表状态
来源：http://tp.bjjhwx.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ly.shtwfgs.cn

[Q74] 强制使用索引
来源：http://hk.muxihuayi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ub.bjjhwx.cn

[Q75] 日期格式化
来源：http://iv.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qq.chemitech.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lt.hnjuh.cn

[Q76] 按天统计
来源：http://jh.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://de.chemitech.net.cn

[Q77] 时间加减
来源：http://qc.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jp.shtwfgs.cn

[Q78] 当前时间
来源：http://bm.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mu.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://dl.huanxung.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yr.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://ij.lnxyls.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ia.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://to.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ke.hahajie.cn

[Q82] 字符长度与字节长度
来源：http://df.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ow.szsharing.cn

[Q83] 大小写转换
来源：http://ci.asd995.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ga.yuntaijiaju.cn

[Q84] 去除首尾空格
来源：http://gj.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://us.newstarts.cn

[Q85] 数值取整
来源：http://ug.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eh.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://jh.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hv.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://qc.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oh.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://bu.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ah.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ff.9csxet.cn

[Q89] 判断表是否存在
来源：http://ap.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ox.shxzskj.cn

[Q90] 生成序号列
来源：http://xr.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xv.lnxyls.cn

================================================================================
来源：http://tl.shxzskj.cn

R. Bash 专题
来源：http://qp.lnxyls.cn

================================================================================
来源：http://ak.haigaiapp.cn

[R01] shebang 与严格模式
来源：http://vv.chemitech.net.cn

#!/usr/bin/env bash
来源：http://ej.nszjky.cn

set -euo pipefail
来源：http://zm.shxzskj.cn

[R02] 变量赋值与使用
来源：http://vc.gzmigu.cn

name="Tom"; echo "$name"
来源：http://hb.jianghongdianzi.cn

[R03] 只读变量
来源：http://ex.gzmigu.cn

readonly PI=3.14
来源：http://yw.9csxet.cn

[R04] 位置参数
来源：http://wu.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nj.hahajie.cn

[R05] 参数默认值
来源：http://kn.lnxyls.cn

name="${1:-default}"
来源：http://nb.hnjuh.cn

[R06] 判断命令是否存在
来源：http://sd.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ar.shxzskj.cn

[R07] if 判断文件
来源：http://zq.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ue.shtwfgs.cn

[R08] 数值比较
来源：http://pe.panjiajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nv.panjiajie.cn

[R09] 字符串比较
来源：http://li.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fo.asd995.cn

[R10] 正则匹配
来源：http://ps.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uy.bjjhwx.cn

[R11] case 多分支
来源：http://yz.9csxet.cn

case "$1" in
来源：http://me.lnxyls.cn

start) echo "启动" ;;
来源：http://yz.huanxung.cn

stop)  echo "停止" ;;
来源：http://mz.nicolike.cn

*)     echo "未知命令" ;;
来源：http://mq.asd995.cn

esac
来源：http://oc.yuntaijiaju.cn

[R12] for 遍历文件
来源：http://ll.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://jb.huixiangedu.cn

[R13] for 计数循环
来源：http://cl.muxihuayi.cn

for i in {1..10}; do echo "$i"; done
来源：http://nz.bjjhwx.cn

[R14] C 风格 for
来源：http://to.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xz.yuexingan06.cn

[R15] while 逐行读文件
来源：http://mk.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tg.nicolike.cn

[R16] until 等待条件
来源：http://bz.9csxet.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wd.nicolike.cn

[R17] 数组定义与取值
来源：http://cs.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ug.szsharing.cn

[R18] 遍历数组
来源：http://bh.huixiangedu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lj.jctech888.com.cn

[R19] 数组长度
来源：http://sc.hahajie.cn

echo "${#arr[@]}"
来源：http://tg.asd995.cn

[R20] 关联数组（字典）
来源：http://gk.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nb.huixinmuqiang.cn

[R21] 字符串长度
来源：http://bu.wgjwhj.cn

echo "${#s}"
来源：http://yg.haigaiapp.cn

[R22] 截取子串
来源：http://pj.muxihuayi.cn

echo "${s:0:5}"
来源：http://lm.colortex.cn

[R23] 字符串替换
来源：http://ep.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fp.chemitech.net.cn

[R24] 大小写转换
来源：http://ai.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wq.hnjuh.cn

[R25] 去后缀 / 去前缀
来源：http://eo.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://qr.jctech888.com.cn

[R26] 命令替换
来源：http://je.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://ud.521024.cn

[R27] 算术展开
来源：http://tm.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://cg.huixiangedu.cn

[R28] 浮点运算
来源：http://wm.jianghongdianzi.cn

echo "scale=2; 10/3" | bc
来源：http://ec.szsharing.cn

[R29] 定义函数
来源：http://sb.huanxung.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dp.szxytkj.cn

[R30] 函数返回状态码
来源：http://zz.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ag.huanxung.cn

[R31] 局部变量
来源：http://zz.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://jo.huanxung.cn

[R32] 参数个数校验
来源：http://mo.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qy.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://yx.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cr.huanxung.cn

[R34] 退出时清理
来源：http://rw.huanxung.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bd.huixiangedu.cn

[R35] 后台执行并等待
来源：http://gp.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mp.gzmigu.cn

[R36] 并发执行多个任务
来源：http://gp.szxytkj.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oc.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://mj.hnjuh.cn

files=$(ls -1)
来源：http://eg.muxihuayi.cn

[R38] 管道串联
来源：http://gh.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://nv.haigaiapp.cn

[R39] 重定向标准输出与错误
来源：http://dn.huixinmuqiang.cn

cmd > out.log 2>&1
来源：http://mx.yuexingan06.cn

[R40] 追加写日志
来源：http://ux.lnxyls.cn

echo "log" >> out.log
来源：http://ey.lnxyls.cn

[R41] 丢弃输出
来源：http://nc.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://ta.bookmarksfly.cn

[R42] 输入重定向
来源：http://mq.szsharing.cn

wc -l < a.txt
来源：http://xk.shxzskj.cn

[R43] 按名字查找文件
来源：http://hf.521024.cn

find . -name "*.log" -type f
来源：http://va.nszjky.cn

[R44] 按修改时间查找
来源：http://zd.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://yt.lnxyls.cn

[R45] 批量删除
来源：http://pa.huanxung.cn

find . -name "*.tmp" -delete
来源：http://yc.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://ep.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ku.asd995.cn

[R47] sed 单行替换
来源：http://ry.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vr.jctech888.com.cn

[R48] awk 取指定列
来源：http://kz.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://oe.huixinmuqiang.cn

[R49] awk 带条件
来源：http://pr.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jb.nszjky.cn

[R50] awk 求和
来源：http://pm.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xj.nszjky.cn

[R51] 排序去重取前几
来源：http://bb.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nc.521024.cn

[R52] 统计行数
来源：http://vt.muxihuayi.cn

wc -l a.txt
来源：http://nl.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://tt.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wp.shxzskj.cn

[R54] 比较两个文件
来源：http://hf.newstarts.cn

diff a.txt b.txt
来源：http://fl.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://zd.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tz.521024.cn

[R56] 远程拷贝
来源：http://wy.huixiangedu.cn

scp file user@host:/path/
来源：http://do.asd995.cn

[R57] 远程执行命令
来源：http://lk.gzmigu.cn

ssh user@host 'uptime'
来源：http://xk.szxytkj.cn

[R58] 下载文件
来源：http://dx.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kt.yuexingan06.cn

[R59] 发 POST JSON
来源：http://tw.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qj.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://lc.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://to.szsharing.cn

[R61] 磁盘占用
来源：http://qc.huixinmuqiang.cn

df -h;  du -sh *
来源：http://bv.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://kl.hahajie.cn

du -ah . | sort -rh | head -10
来源：http://un.newstarts.cn

[R63] 内存与进程
来源：http://sn.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://mq.asd995.cn

[R64] 结束进程
来源：http://oo.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://el.hahajie.cn

[R65] 查看端口占用
来源：http://ev.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jn.bjjhwx.cn

[R66] 定时任务
来源：http://vz.9csxet.cn

crontab -e;  crontab -l
来源：http://va.colortex.cn

[R67] 生成随机十六进制串
来源：http://la.asd995.cn

openssl rand -hex 16
来源：http://ft.521024.cn

[R68] 计算文件校验值
来源：http://hv.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ug.jctech888.com.cn

[R69] 生成随机密码
来源：http://hx.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ta.wgjwhj.cn

[R70] 时间戳与互转
来源：http://qt.9csxet.cn

date +%s;  date -d @1700000000
来源：http://jt.shxzukj.cn

[R71] 日期格式化
来源：http://xm.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://px.colortex.cn

[R72] 等待端口就绪
来源：http://mh.szxytkj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://el.asd995.cn

[R73] 分割大日志
来源：http://hd.521024.cn

split -l 1000 big.log part_
来源：http://bw.shxzskj.cn

[R74] 批量重命名
来源：http://rt.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ja.asd995.cn

[R75] 导出环境变量
来源：http://uj.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://bi.shxzukj.cn

[R76] 使用临时文件
来源：http://mh.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ld.colortex.cn

[R77] 读取用户输入
来源：http://tn.muxihuayi.cn

read -rp "请输入: " ans
来源：http://io.nicolike.cn

[R78] 交互式菜单
来源：http://gz.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tv.haigaiapp.cn

[R79] 解析命令行选项
来源：http://wt.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yg.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://tn.huixinmuqiang.cn

time ./run.sh
来源：http://ry.panjiajie.cn

================================================================================
来源：http://mn.lnxyls.cn

S. C / C++ 专题
来源：http://zi.chemitech.net.cn

================================================================================
来源：http://qh.huanxung.cn

[S01] C：Hello World
来源：http://cv.colortex.cn

#include <stdio.h>
来源：http://op.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tk.nszjky.cn

[S02] C：变量与格式化输出
来源：http://sk.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://yk.jianghongdianzi.cn

[S03] C：读入整数
来源：http://yo.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://db.gzmigu.cn

[S04] C：字符串复制
来源：http://dl.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pb.chemitech.net.cn

[S05] C：字符串长度
来源：http://gk.jctech888.com.cn

strlen(s)
来源：http://xy.hahajie.cn

[S06] C：字符串比较
来源：http://ka.bjjhwx.cn

strcmp(a, b) == 0
来源：http://sv.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://yi.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jz.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://no.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pv.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://vj.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sh.shtwfgs.cn

[S10] C：指针与解引用
来源：http://um.newstarts.cn

int *p = &a;  *p = 5;
来源：http://lb.szxytkj.cn

[S11] C：逐行读文件
来源：http://kd.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://bv.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://da.hahajie.cn

fclose(f);
来源：http://aj.szsharing.cn

[S12] C：写文件
来源：http://rx.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ri.newstarts.cn

[S13] C：宏定义
来源：http://qw.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qp.jctech888.com.cn

[S14] C：枚举
来源：http://da.jianghongdianzi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ys.haigaiapp.cn

[S15] C：类型转换
来源：http://if.szxytkj.cn

(double) a / b
来源：http://sz.huanxung.cn

[S16] C：位操作置位
来源：http://rg.asd995.cn

x |= (1 << 3);
来源：http://pd.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://ax.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://il.huanxung.cn

[S18] C：命令行参数
来源：http://le.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://gf.nszjky.cn

[S19] C：快速排序
来源：http://ui.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kn.shxzskj.cn

[S20] C：二分查找
来源：http://pf.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ok.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://wv.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ct.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://kh.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uy.hahajie.cn

[S23] C：随机数
来源：http://dc.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kj.huixiangedu.cn

[S24] C：获取本地时间
来源：http://is.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gt.9csxet.cn

[S25] C：内存拷贝
来源：http://iw.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://fx.nicolike.cn

[S26] C：内存清零
来源：http://ha.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://sj.521024.cn

[S27] C：定义常量
来源：http://ta.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://ta.huanxung.cn

[S28] C：静态变量
来源：http://gx.yuntaijiaju.cn


<!-- 参考信息 -->