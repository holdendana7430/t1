代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jt.wgjwhj.cn

[Q60] 取上一行 / 下一行
来源：http://wj.hnjuh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://md.shxzskj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hm.jianghongdianzi.cn

[Q61] 移动平均
来源：http://vj.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ep.wgjwhj.cn

[Q62] 分组占比
来源：http://uk.nicolike.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ij.nszjky.cn

[Q63] 开启事务
来源：http://ms.shxzskj.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qs.szxytkj.cn

[Q64] 提交事务
来源：http://yd.yuntaijiaju.cn

COMMIT;
来源：http://tr.hahajie.cn

[Q65] 回滚事务
来源：http://do.haigaiapp.cn

ROLLBACK;
来源：http://an.szsharing.cn

[Q66] 行锁查询
来源：http://cq.lnxyls.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sf.lnxyls.cn

[Q67] 设置隔离级别
来源：http://tu.9csxet.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mu.shxzukj.cn

[Q68] 保存点
来源：http://bz.newstarts.cn

SAVEPOINT sp1;
来源：http://nc.huanxung.cn

ROLLBACK TO sp1;
来源：http://rh.nszjky.cn

[Q69] 查看执行计划
来源：http://qu.huixiangedu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ac.szsharing.cn

[Q70] 更新统计信息
来源：http://tq.panjiajie.cn

ANALYZE TABLE users;
来源：http://ca.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://ce.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://be.huixinmuqiang.cn

[Q72] 查看索引
来源：http://ae.shxzskj.cn

SHOW INDEX FROM users;
来源：http://jv.panjiajie.cn

[Q73] 查看表状态
来源：http://fn.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mu.bjjhwx.cn

[Q74] 强制使用索引
来源：http://vy.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dp.lnxyls.cn

[Q75] 日期格式化
来源：http://gz.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kc.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hq.haigaiapp.cn

[Q76] 按天统计
来源：http://qp.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fi.shxzskj.cn

[Q77] 时间加减
来源：http://qi.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ie.colortex.cn

[Q78] 当前时间
来源：http://dk.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://me.lnxyls.cn

[Q79] 字符串拼接
来源：http://qi.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ec.chemitech.net.cn

[Q80] 字符串截取
来源：http://wd.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ib.shxzskj.cn

[Q81] 字符串替换
来源：http://xr.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://be.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://mo.szxytkj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ut.asd995.cn

[Q83] 大小写转换
来源：http://hl.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://as.huanxung.cn

[Q84] 去除首尾空格
来源：http://ic.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://jv.wgjwhj.cn

[Q85] 数值取整
来源：http://sm.newstarts.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cw.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://tc.huixiangedu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wa.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://vy.jianghongdianzi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rw.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://zo.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zp.shtwfgs.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cb.hnjuh.cn

[Q89] 判断表是否存在
来源：http://ep.bookmarksfly.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ud.huixinmuqiang.cn

[Q90] 生成序号列
来源：http://jg.yuntaijiaju.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zb.hahajie.cn

================================================================================
来源：http://dk.muxihuayi.cn

R. Bash 专题
来源：http://hq.521024.cn

================================================================================
来源：http://es.hahajie.cn

[R01] shebang 与严格模式
来源：http://tg.bjjhwx.cn

#!/usr/bin/env bash
来源：http://zl.nicolike.cn

set -euo pipefail
来源：http://gw.szxytkj.cn

[R02] 变量赋值与使用
来源：http://pj.9csxet.cn

name="Tom"; echo "$name"
来源：http://ry.jctech888.com.cn

[R03] 只读变量
来源：http://wo.muxihuayi.cn

readonly PI=3.14
来源：http://pb.asd995.cn

[R04] 位置参数
来源：http://jn.huanxung.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eo.lnxyls.cn

[R05] 参数默认值
来源：http://xw.shxzskj.cn

name="${1:-default}"
来源：http://zs.nszjky.cn

[R06] 判断命令是否存在
来源：http://dh.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wd.yuexingan06.cn

[R07] if 判断文件
来源：http://lr.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pe.jctech888.com.cn

[R08] 数值比较
来源：http://nl.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hj.jianghongdianzi.cn

[R09] 字符串比较
来源：http://vx.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uq.gzmigu.cn

[R10] 正则匹配
来源：http://fq.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://id.9csxet.cn

[R11] case 多分支
来源：http://lv.huanxung.cn

case "$1" in
来源：http://xy.gzmigu.cn

start) echo "启动" ;;
来源：http://im.9csxet.cn

stop)  echo "停止" ;;
来源：http://nh.huanxung.cn

*)     echo "未知命令" ;;
来源：http://oj.haigaiapp.cn

esac
来源：http://ag.huixiangedu.cn

[R12] for 遍历文件
来源：http://lq.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://yb.shxzukj.cn

[R13] for 计数循环
来源：http://ch.jctech888.com.cn

for i in {1..10}; do echo "$i"; done
来源：http://ud.szxytkj.cn

[R14] C 风格 for
来源：http://cj.shxzskj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ig.asd995.cn

[R15] while 逐行读文件
来源：http://px.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ea.shxzskj.cn

[R16] until 等待条件
来源：http://pv.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ww.jctech888.com.cn

[R17] 数组定义与取值
来源：http://kl.szxytkj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gr.szxytkj.cn

[R18] 遍历数组
来源：http://ac.shxzukj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ce.shxzskj.cn

[R19] 数组长度
来源：http://vj.huanxung.cn

echo "${#arr[@]}"
来源：http://rf.asd995.cn

[R20] 关联数组（字典）
来源：http://ch.colortex.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bw.chemitech.net.cn

[R21] 字符串长度
来源：http://qe.newstarts.cn

echo "${#s}"
来源：http://el.huanxung.cn

[R22] 截取子串
来源：http://qi.jianghongdianzi.cn

echo "${s:0:5}"
来源：http://dj.gzmigu.cn

[R23] 字符串替换
来源：http://tz.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://he.9csxet.cn

[R24] 大小写转换
来源：http://hu.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pb.chemitech.net.cn

[R25] 去后缀 / 去前缀
来源：http://or.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yi.nicolike.cn

[R26] 命令替换
来源：http://fk.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://vs.jianghongdianzi.cn

[R27] 算术展开
来源：http://xn.shxzskj.cn

echo $((1 + 2 * 3))
来源：http://nj.chemitech.net.cn

[R28] 浮点运算
来源：http://sm.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://fr.newstarts.cn

[R29] 定义函数
来源：http://mj.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yj.nszjky.cn

[R30] 函数返回状态码
来源：http://ya.9csxet.cn

f() { return 0; }; f || echo "失败了"
来源：http://eh.shtwfgs.cn

[R31] 局部变量
来源：http://ls.gzmigu.cn

f() { local x=1; echo "$x"; }
来源：http://vr.shxzukj.cn

[R32] 参数个数校验
来源：http://hr.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cx.lnxyls.cn

[R33] 捕获错误并提示行号
来源：http://zh.huanxung.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vh.huanxung.cn

[R34] 退出时清理
来源：http://kx.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kq.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://ax.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jy.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://bz.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hv.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://ga.hnjuh.cn

files=$(ls -1)
来源：http://wr.hahajie.cn

[R38] 管道串联
来源：http://oz.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://vu.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://zc.haigaiapp.cn

cmd > out.log 2>&1
来源：http://it.huixinmuqiang.cn

[R40] 追加写日志
来源：http://cn.9csxet.cn

echo "log" >> out.log
来源：http://se.hahajie.cn

[R41] 丢弃输出
来源：http://jh.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://es.shxzskj.cn

[R42] 输入重定向
来源：http://ev.nszjky.cn

wc -l < a.txt
来源：http://ml.521024.cn

[R43] 按名字查找文件
来源：http://pc.shxzukj.cn

find . -name "*.log" -type f
来源：http://ps.haigaiapp.cn

[R44] 按修改时间查找
来源：http://vl.szsharing.cn

find . -mtime -7 -type f
来源：http://vi.panjiajie.cn

[R45] 批量删除
来源：http://tu.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://jn.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://yk.panjiajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sj.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://th.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ll.nszjky.cn

[R48] awk 取指定列
来源：http://al.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://va.szxytkj.cn

[R49] awk 带条件
来源：http://im.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ue.shxzskj.cn

[R50] awk 求和
来源：http://vv.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ua.nszjky.cn

[R51] 排序去重取前几
来源：http://se.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zy.chemitech.net.cn

[R52] 统计行数
来源：http://qh.jianghongdianzi.cn

wc -l a.txt
来源：http://eu.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://hi.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mu.hnjuh.cn

[R54] 比较两个文件
来源：http://fp.szxytkj.cn

diff a.txt b.txt
来源：http://bd.bookmarksfly.cn

[R55] 压缩与解压
来源：http://bk.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yb.hahajie.cn

[R56] 远程拷贝
来源：http://vc.shtwfgs.cn

scp file user@host:/path/
来源：http://rj.jctech888.com.cn

[R57] 远程执行命令
来源：http://dz.huanxung.cn

ssh user@host 'uptime'
来源：http://gr.yuntaijiaju.cn

[R58] 下载文件
来源：http://xn.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://en.wgjwhj.cn

[R59] 发 POST JSON
来源：http://jw.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lh.9csxet.cn

[R60] 只看 HTTP 状态码
来源：http://ig.huixinmuqiang.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oo.bjjhwx.cn

[R61] 磁盘占用
来源：http://ib.szsharing.cn

df -h;  du -sh *
来源：http://ug.newstarts.cn

[R62] 找最占空间的文件
来源：http://ua.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://oj.asd995.cn

[R63] 内存与进程
来源：http://kg.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://va.chemitech.net.cn

[R64] 结束进程
来源：http://px.haigaiapp.cn

kill -9 $(pgrep -f app.py)
来源：http://dr.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://nf.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ti.yuexingan06.cn

[R66] 定时任务
来源：http://tj.nicolike.cn

crontab -e;  crontab -l
来源：http://lp.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://tz.gzmigu.cn

openssl rand -hex 16
来源：http://gg.bjjhwx.cn

[R68] 计算文件校验值
来源：http://kt.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kr.nszjky.cn

[R69] 生成随机密码
来源：http://hx.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://xh.hahajie.cn

[R70] 时间戳与互转
来源：http://bv.9csxet.cn

date +%s;  date -d @1700000000
来源：http://js.asd995.cn

[R71] 日期格式化
来源：http://jj.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yv.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://yi.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pk.szsharing.cn

[R73] 分割大日志
来源：http://dn.jctech888.com.cn

split -l 1000 big.log part_
来源：http://kj.521024.cn

[R74] 批量重命名
来源：http://de.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wu.chemitech.net.cn

[R75] 导出环境变量
来源：http://xt.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://cs.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://vs.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yx.jctech888.com.cn

[R77] 读取用户输入
来源：http://gu.hnjuh.cn

read -rp "请输入: " ans
来源：http://lb.hahajie.cn

[R78] 交互式菜单
来源：http://uj.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xb.hahajie.cn

[R79] 解析命令行选项
来源：http://di.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mh.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://fg.newstarts.cn

time ./run.sh
来源：http://oe.bookmarksfly.cn

================================================================================
来源：http://zo.asd995.cn

S. C / C++ 专题
来源：http://ax.huanxung.cn

================================================================================
来源：http://jz.szsharing.cn

[S01] C：Hello World
来源：http://bk.huixinmuqiang.cn

#include <stdio.h>
来源：http://ml.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qc.asd995.cn

[S02] C：变量与格式化输出
来源：http://wk.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://gh.yuntaijiaju.cn

[S03] C：读入整数
来源：http://zb.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://sx.huanxung.cn

[S04] C：字符串复制
来源：http://jc.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lj.huanxung.cn

[S05] C：字符串长度
来源：http://tj.newstarts.cn

strlen(s)
来源：http://pk.newstarts.cn

[S06] C：字符串比较
来源：http://ep.szsharing.cn

strcmp(a, b) == 0
来源：http://vs.hahajie.cn

[S07] C：数组遍历求和
来源：http://gu.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oc.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://bw.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kh.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://uh.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sx.chemitech.net.cn

[S10] C：指针与解引用
来源：http://qo.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://ws.huanxung.cn

[S11] C：逐行读文件
来源：http://jd.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ex.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ra.shxzukj.cn

fclose(f);
来源：http://rj.szxytkj.cn

[S12] C：写文件
来源：http://pe.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sf.muxihuayi.cn

[S13] C：宏定义
来源：http://wk.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yx.szsharing.cn

[S14] C：枚举
来源：http://fn.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://qk.szxytkj.cn

[S15] C：类型转换
来源：http://eh.asd995.cn

(double) a / b
来源：http://ze.muxihuayi.cn

[S16] C：位操作置位
来源：http://nt.nszjky.cn

x |= (1 << 3);
来源：http://sj.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://vd.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jn.jctech888.com.cn

[S18] C：命令行参数
来源：http://fg.panjiajie.cn

int main(int argc, char **argv)
来源：http://zl.huixinmuqiang.cn

[S19] C：快速排序
来源：http://mh.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sz.gzmigu.cn

[S20] C：二分查找
来源：http://nq.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nm.huixiangedu.cn

[S21] C：字符类别判断
来源：http://ja.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hc.hahajie.cn

[S22] C：字符串转数字
来源：http://mu.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://da.9csxet.cn

[S23] C：随机数
来源：http://uk.huixiangedu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xe.shtwfgs.cn

[S24] C：获取本地时间
来源：http://bw.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ap.gzmigu.cn

[S25] C：内存拷贝
来源：http://cf.gzmigu.cn

memcpy(dst, src, n);
来源：http://hs.jianghongdianzi.cn

[S26] C：内存清零
来源：http://jj.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://sx.bookmarksfly.cn

[S27] C：定义常量
来源：http://gu.muxihuayi.cn

const double PI = 3.14159;
来源：http://tg.newstarts.cn

[S28] C：静态变量
来源：http://cs.hahajie.cn

static int counter = 0;
来源：http://zr.szsharing.cn

[S29] C：变参函数
来源：http://zn.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hx.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://hd.haigaiapp.cn


<!-- 参考信息 -->