代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aa.gzmigu.cn

[Q60] 取上一行 / 下一行
来源：http://ui.gzmigu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zk.nszjky.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wy.yuntaijiaju.cn

[Q61] 移动平均
来源：http://he.nszjky.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qb.huanxung.cn

[Q62] 分组占比
来源：http://rl.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zu.9csxet.cn

[Q63] 开启事务
来源：http://xt.muxihuayi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ze.bjjhwx.cn

[Q64] 提交事务
来源：http://th.nicolike.cn

COMMIT;
来源：http://kl.colortex.cn

[Q65] 回滚事务
来源：http://ku.huixinmuqiang.cn

ROLLBACK;
来源：http://ef.yuexingan06.cn

[Q66] 行锁查询
来源：http://fa.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ki.yuexingan06.cn

[Q67] 设置隔离级别
来源：http://js.asd995.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mt.colortex.cn

[Q68] 保存点
来源：http://fc.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://zx.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://mw.521024.cn

[Q69] 查看执行计划
来源：http://lw.panjiajie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lc.haigaiapp.cn

[Q70] 更新统计信息
来源：http://xl.lnxyls.cn

ANALYZE TABLE users;
来源：http://aa.hahajie.cn

[Q71] 查看建表语句
来源：http://kq.9csxet.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oy.gzmigu.cn

[Q72] 查看索引
来源：http://rf.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://zz.bookmarksfly.cn

[Q73] 查看表状态
来源：http://vh.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gf.bjjhwx.cn

[Q74] 强制使用索引
来源：http://cb.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xo.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://rh.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bp.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vp.nszjky.cn

[Q76] 按天统计
来源：http://kk.colortex.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fv.huixiangedu.cn

[Q77] 时间加减
来源：http://he.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sl.nszjky.cn

[Q78] 当前时间
来源：http://pu.huixinmuqiang.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://es.newstarts.cn

[Q79] 字符串拼接
来源：http://jc.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tb.jctech888.com.cn

[Q80] 字符串截取
来源：http://pe.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dh.jctech888.com.cn

[Q81] 字符串替换
来源：http://ei.panjiajie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://an.huanxung.cn

[Q82] 字符长度与字节长度
来源：http://ho.muxihuayi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sb.haigaiapp.cn

[Q83] 大小写转换
来源：http://nv.lnxyls.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xq.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://xh.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://ah.szxytkj.cn

[Q85] 数值取整
来源：http://yq.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zk.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://tm.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://am.panjiajie.cn

[Q87] JSON 字段做条件
来源：http://iv.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hj.wgjwhj.cn

[Q88] 行转列（条件聚合）
来源：http://tf.jctech888.com.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://by.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oi.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://tn.wgjwhj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lo.nszjky.cn

[Q90] 生成序号列
来源：http://ot.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pa.shxzukj.cn

================================================================================
来源：http://td.nszjky.cn

R. Bash 专题
来源：http://qb.shtwfgs.cn

================================================================================
来源：http://rh.szsharing.cn

[R01] shebang 与严格模式
来源：http://pe.shtwfgs.cn

#!/usr/bin/env bash
来源：http://mc.yuexingan06.cn

set -euo pipefail
来源：http://be.newstarts.cn

[R02] 变量赋值与使用
来源：http://yq.hahajie.cn

name="Tom"; echo "$name"
来源：http://jq.muxihuayi.cn

[R03] 只读变量
来源：http://ob.yuntaijiaju.cn

readonly PI=3.14
来源：http://dw.bookmarksfly.cn

[R04] 位置参数
来源：http://uo.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kv.521024.cn

[R05] 参数默认值
来源：http://ak.colortex.cn

name="${1:-default}"
来源：http://wk.colortex.cn

[R06] 判断命令是否存在
来源：http://da.jctech888.com.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qs.huixinmuqiang.cn

[R07] if 判断文件
来源：http://ii.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pk.hahajie.cn

[R08] 数值比较
来源：http://ka.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mr.gzmigu.cn

[R09] 字符串比较
来源：http://fl.wgjwhj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oc.jianghongdianzi.cn

[R10] 正则匹配
来源：http://di.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yy.nicolike.cn

[R11] case 多分支
来源：http://rc.521024.cn

case "$1" in
来源：http://do.huanxung.cn

start) echo "启动" ;;
来源：http://qo.szsharing.cn

stop)  echo "停止" ;;
来源：http://hp.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://wo.colortex.cn

esac
来源：http://zj.panjiajie.cn

[R12] for 遍历文件
来源：http://il.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://yb.chemitech.net.cn

[R13] for 计数循环
来源：http://vb.shxzukj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ng.haigaiapp.cn

[R14] C 风格 for
来源：http://au.huixiangedu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tj.newstarts.cn

[R15] while 逐行读文件
来源：http://pf.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nm.yuexingan06.cn

[R16] until 等待条件
来源：http://ku.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pa.colortex.cn

[R17] 数组定义与取值
来源：http://xj.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fn.hnjuh.cn

[R18] 遍历数组
来源：http://mw.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hc.colortex.cn

[R19] 数组长度
来源：http://rc.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://sl.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://eb.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ht.hahajie.cn

[R21] 字符串长度
来源：http://rk.hnjuh.cn

echo "${#s}"
来源：http://vj.jianghongdianzi.cn

[R22] 截取子串
来源：http://ff.lnxyls.cn

echo "${s:0:5}"
来源：http://gc.bjjhwx.cn

[R23] 字符串替换
来源：http://nl.huixiangedu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sz.shtwfgs.cn

[R24] 大小写转换
来源：http://ns.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zc.muxihuayi.cn

[R25] 去后缀 / 去前缀
来源：http://hh.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://on.jianghongdianzi.cn

[R26] 命令替换
来源：http://ns.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ao.colortex.cn

[R27] 算术展开
来源：http://lu.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://ks.9csxet.cn

[R28] 浮点运算
来源：http://rr.gzmigu.cn

echo "scale=2; 10/3" | bc
来源：http://fi.szsharing.cn

[R29] 定义函数
来源：http://et.yuexingan06.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fy.szxytkj.cn

[R30] 函数返回状态码
来源：http://ow.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://em.shtwfgs.cn

[R31] 局部变量
来源：http://vs.chemitech.net.cn

f() { local x=1; echo "$x"; }
来源：http://ha.jctech888.com.cn

[R32] 参数个数校验
来源：http://qn.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bt.521024.cn

[R33] 捕获错误并提示行号
来源：http://sn.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ty.shtwfgs.cn

[R34] 退出时清理
来源：http://ca.asd995.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ql.gzmigu.cn

[R35] 后台执行并等待
来源：http://ov.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ie.lnxyls.cn

[R36] 并发执行多个任务
来源：http://hj.hahajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mf.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://qa.szsharing.cn

files=$(ls -1)
来源：http://dj.jianghongdianzi.cn

[R38] 管道串联
来源：http://ql.haigaiapp.cn

cat a.txt | grep -i error | wc -l
来源：http://gv.huanxung.cn

[R39] 重定向标准输出与错误
来源：http://dn.chemitech.net.cn

cmd > out.log 2>&1
来源：http://bu.lnxyls.cn

[R40] 追加写日志
来源：http://rm.haigaiapp.cn

echo "log" >> out.log
来源：http://wp.9csxet.cn

[R41] 丢弃输出
来源：http://sy.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://va.yuexingan06.cn

[R42] 输入重定向
来源：http://sz.nicolike.cn

wc -l < a.txt
来源：http://yt.lnxyls.cn

[R43] 按名字查找文件
来源：http://of.bjjhwx.cn

find . -name "*.log" -type f
来源：http://ms.hnjuh.cn

[R44] 按修改时间查找
来源：http://fp.chemitech.net.cn

find . -mtime -7 -type f
来源：http://hn.szxytkj.cn

[R45] 批量删除
来源：http://oo.szsharing.cn

find . -name "*.tmp" -delete
来源：http://gv.nszjky.cn

[R46] 递归替换文件内容
来源：http://nz.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hg.wgjwhj.cn

[R47] sed 单行替换
来源：http://mw.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gy.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://fq.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://yp.shxzskj.cn

[R49] awk 带条件
来源：http://lx.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qt.huixiangedu.cn

[R50] awk 求和
来源：http://py.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://uh.szxytkj.cn

[R51] 排序去重取前几
来源：http://js.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iq.yuntaijiaju.cn

[R52] 统计行数
来源：http://ao.shxzskj.cn

wc -l a.txt
来源：http://vf.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://oe.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lk.nicolike.cn

[R54] 比较两个文件
来源：http://cv.yuexingan06.cn

diff a.txt b.txt
来源：http://ye.haigaiapp.cn

[R55] 压缩与解压
来源：http://fn.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qy.haigaiapp.cn

[R56] 远程拷贝
来源：http://dn.bookmarksfly.cn

scp file user@host:/path/
来源：http://co.jctech888.com.cn

[R57] 远程执行命令
来源：http://gz.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://cm.asd995.cn

[R58] 下载文件
来源：http://nk.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tf.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://tz.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ft.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ju.jianghongdianzi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ag.colortex.cn

[R61] 磁盘占用
来源：http://ts.chemitech.net.cn

df -h;  du -sh *
来源：http://jf.asd995.cn

[R62] 找最占空间的文件
来源：http://ul.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://ag.huanxung.cn

[R63] 内存与进程
来源：http://mt.521024.cn

free -h;  ps aux | grep nginx
来源：http://ym.huixiangedu.cn

[R64] 结束进程
来源：http://bt.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://we.gzmigu.cn

[R65] 查看端口占用
来源：http://bz.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kp.haigaiapp.cn

[R66] 定时任务
来源：http://cb.gzmigu.cn

crontab -e;  crontab -l
来源：http://pa.nicolike.cn

[R67] 生成随机十六进制串
来源：http://jd.shxzukj.cn

openssl rand -hex 16
来源：http://qd.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://lh.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ep.nszjky.cn

[R69] 生成随机密码
来源：http://tt.hnjuh.cn

head -c 16 /dev/urandom | base64
来源：http://db.shtwfgs.cn

[R70] 时间戳与互转
来源：http://ux.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://sb.wgjwhj.cn

[R71] 日期格式化
来源：http://dq.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sh.shxzskj.cn

[R72] 等待端口就绪
来源：http://wp.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zi.wgjwhj.cn

[R73] 分割大日志
来源：http://cq.chemitech.net.cn

split -l 1000 big.log part_
来源：http://nj.chemitech.net.cn

[R74] 批量重命名
来源：http://ad.yuntaijiaju.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ti.szsharing.cn

[R75] 导出环境变量
来源：http://ys.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://fv.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://ke.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qk.muxihuayi.cn

[R77] 读取用户输入
来源：http://sc.chemitech.net.cn

read -rp "请输入: " ans
来源：http://mu.muxihuayi.cn

[R78] 交互式菜单
来源：http://vg.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ju.colortex.cn

[R79] 解析命令行选项
来源：http://sw.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://db.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://oe.newstarts.cn

time ./run.sh
来源：http://tm.muxihuayi.cn

================================================================================
来源：http://od.colortex.cn

S. C / C++ 专题
来源：http://sx.yuexingan06.cn

================================================================================
来源：http://wx.asd995.cn

[S01] C：Hello World
来源：http://cw.hnjuh.cn

#include <stdio.h>
来源：http://ve.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nv.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://cg.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://wp.gzmigu.cn

[S03] C：读入整数
来源：http://md.nszjky.cn

int x; scanf("%d", &x);
来源：http://hs.shtwfgs.cn

[S04] C：字符串复制
来源：http://cj.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qi.chemitech.net.cn

[S05] C：字符串长度
来源：http://qh.huanxung.cn

strlen(s)
来源：http://ul.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://xv.lnxyls.cn

strcmp(a, b) == 0
来源：http://pu.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://mp.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://em.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://xy.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://js.newstarts.cn

[S09] C：结构体定义与初始化
来源：http://hc.bookmarksfly.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ul.huanxung.cn

[S10] C：指针与解引用
来源：http://pw.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://wz.colortex.cn

[S11] C：逐行读文件
来源：http://od.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://kb.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xp.shtwfgs.cn

fclose(f);
来源：http://ch.asd995.cn

[S12] C：写文件
来源：http://ya.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kc.9csxet.cn

[S13] C：宏定义
来源：http://es.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zc.nszjky.cn

[S14] C：枚举
来源：http://pa.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://jy.9csxet.cn

[S15] C：类型转换
来源：http://al.huixiangedu.cn

(double) a / b
来源：http://fv.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://fh.hnjuh.cn

x |= (1 << 3);
来源：http://rz.nszjky.cn

[S17] C：安全拼接字符串
来源：http://ib.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jk.asd995.cn

[S18] C：命令行参数
来源：http://hs.shxzukj.cn

int main(int argc, char **argv)
来源：http://do.bjjhwx.cn

[S19] C：快速排序
来源：http://pb.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ed.lnxyls.cn

[S20] C：二分查找
来源：http://kf.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hp.muxihuayi.cn

[S21] C：字符类别判断
来源：http://za.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xl.nszjky.cn

[S22] C：字符串转数字
来源：http://jq.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ny.huanxung.cn

[S23] C：随机数
来源：http://qf.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://av.huixiangedu.cn

[S24] C：获取本地时间
来源：http://xw.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xm.bjjhwx.cn

[S25] C：内存拷贝
来源：http://si.gzmigu.cn

memcpy(dst, src, n);
来源：http://du.521024.cn

[S26] C：内存清零
来源：http://gq.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://aw.huixinmuqiang.cn

[S27] C：定义常量
来源：http://gc.panjiajie.cn

const double PI = 3.14159;
来源：http://wu.jctech888.com.cn

[S28] C：静态变量
来源：http://up.shxzukj.cn

static int counter = 0;
来源：http://yx.hnjuh.cn

[S29] C：变参函数
来源：http://mk.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://re.jctech888.com.cn

[S30] C：头文件保护
来源：http://tv.asd995.cn


<!-- 参考信息 -->