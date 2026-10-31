代发 wailian999

[Q65] 回滚事务
来源：http://xq.hnjuh.cn

ROLLBACK;
来源：http://mx.gzmigu.cn

[Q66] 行锁查询
来源：http://da.szxytkj.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sh.gzmigu.cn

[Q67] 设置隔离级别
来源：http://dw.colortex.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kl.9csxet.cn

[Q68] 保存点
来源：http://jr.szxytkj.cn

SAVEPOINT sp1;
来源：http://kv.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://mw.chemitech.net.cn

[Q69] 查看执行计划
来源：http://fr.nszjky.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://as.chemitech.net.cn

[Q70] 更新统计信息
来源：http://na.wgjwhj.cn

ANALYZE TABLE users;
来源：http://lo.yuexingan06.cn

[Q71] 查看建表语句
来源：http://ku.yuexingan06.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ev.9csxet.cn

[Q72] 查看索引
来源：http://ev.hahajie.cn

SHOW INDEX FROM users;
来源：http://ye.asd995.cn

[Q73] 查看表状态
来源：http://ly.hahajie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tx.nicolike.cn

[Q74] 强制使用索引
来源：http://zy.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uh.gzmigu.cn

[Q75] 日期格式化
来源：http://cf.hnjuh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://se.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dj.hahajie.cn

[Q76] 按天统计
来源：http://zb.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yx.yuntaijiaju.cn

[Q77] 时间加减
来源：http://bw.huixiangedu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qe.nszjky.cn

[Q78] 当前时间
来源：http://kp.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jy.szsharing.cn

[Q79] 字符串拼接
来源：http://sb.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rv.colortex.cn

[Q80] 字符串截取
来源：http://lj.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dk.bjjhwx.cn

[Q81] 字符串替换
来源：http://hf.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fw.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://yh.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ze.chemitech.net.cn

[Q83] 大小写转换
来源：http://ve.wgjwhj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ju.lnxyls.cn

[Q84] 去除首尾空格
来源：http://tn.521024.cn

SELECT TRIM(name) FROM users;
来源：http://dd.hahajie.cn

[Q85] 数值取整
来源：http://ht.yuntaijiaju.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ch.huixiangedu.cn

[Q86] 读取 JSON 字段
来源：http://je.nicolike.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ld.9csxet.cn

[Q87] JSON 字段做条件
来源：http://dw.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fj.bjjhwx.cn

[Q88] 行转列（条件聚合）
来源：http://tj.9csxet.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xh.wgjwhj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jk.huanxung.cn

[Q89] 判断表是否存在
来源：http://pp.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tv.lnxyls.cn

[Q90] 生成序号列
来源：http://aj.szxytkj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vl.nicolike.cn

================================================================================
来源：http://tw.szsharing.cn

R. Bash 专题
来源：http://dm.newstarts.cn

================================================================================
来源：http://dj.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://be.shxzskj.cn

#!/usr/bin/env bash
来源：http://cs.bjjhwx.cn

set -euo pipefail
来源：http://wg.newstarts.cn

[R02] 变量赋值与使用
来源：http://op.panjiajie.cn

name="Tom"; echo "$name"
来源：http://ii.szxytkj.cn

[R03] 只读变量
来源：http://hn.gzmigu.cn

readonly PI=3.14
来源：http://ho.newstarts.cn

[R04] 位置参数
来源：http://hm.hahajie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xy.szxytkj.cn

[R05] 参数默认值
来源：http://ot.jctech888.com.cn

name="${1:-default}"
来源：http://tt.huixiangedu.cn

[R06] 判断命令是否存在
来源：http://lf.bjjhwx.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vn.panjiajie.cn

[R07] if 判断文件
来源：http://tf.nszjky.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://et.521024.cn

[R08] 数值比较
来源：http://gi.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rs.huixiangedu.cn

[R09] 字符串比较
来源：http://xm.shtwfgs.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ft.lnxyls.cn

[R10] 正则匹配
来源：http://ud.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wr.nicolike.cn

[R11] case 多分支
来源：http://ht.colortex.cn

case "$1" in
来源：http://cd.yuexingan06.cn

start) echo "启动" ;;
来源：http://tz.shxzukj.cn

stop)  echo "停止" ;;
来源：http://ja.bookmarksfly.cn

*)     echo "未知命令" ;;
来源：http://jc.lnxyls.cn

esac
来源：http://jz.nicolike.cn

[R12] for 遍历文件
来源：http://xp.newstarts.cn

for f in *.txt; do echo "$f"; done
来源：http://fg.newstarts.cn

[R13] for 计数循环
来源：http://gi.jianghongdianzi.cn

for i in {1..10}; do echo "$i"; done
来源：http://bu.shtwfgs.cn

[R14] C 风格 for
来源：http://td.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ds.haigaiapp.cn

[R15] while 逐行读文件
来源：http://dr.newstarts.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jv.colortex.cn

[R16] until 等待条件
来源：http://da.gzmigu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mg.bjjhwx.cn

[R17] 数组定义与取值
来源：http://ft.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sj.newstarts.cn

[R18] 遍历数组
来源：http://ie.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ik.bookmarksfly.cn

[R19] 数组长度
来源：http://kq.yuexingan06.cn

echo "${#arr[@]}"
来源：http://rv.huixiangedu.cn

[R20] 关联数组（字典）
来源：http://fk.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tw.jianghongdianzi.cn

[R21] 字符串长度
来源：http://gn.jctech888.com.cn

echo "${#s}"
来源：http://qk.nszjky.cn

[R22] 截取子串
来源：http://lf.asd995.cn

echo "${s:0:5}"
来源：http://nj.hahajie.cn

[R23] 字符串替换
来源：http://wd.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bg.hnjuh.cn

[R24] 大小写转换
来源：http://hr.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sa.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://wt.panjiajie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yb.yuntaijiaju.cn

[R26] 命令替换
来源：http://sb.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://il.bjjhwx.cn

[R27] 算术展开
来源：http://ba.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://rv.chemitech.net.cn

[R28] 浮点运算
来源：http://uv.newstarts.cn

echo "scale=2; 10/3" | bc
来源：http://ig.521024.cn

[R29] 定义函数
来源：http://pl.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oe.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://vg.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://cg.shxzskj.cn

[R31] 局部变量
来源：http://qt.shxzukj.cn

f() { local x=1; echo "$x"; }
来源：http://ae.yuexingan06.cn

[R32] 参数个数校验
来源：http://mn.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pm.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://vs.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yk.asd995.cn

[R34] 退出时清理
来源：http://gk.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hb.asd995.cn

[R35] 后台执行并等待
来源：http://ho.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nk.wgjwhj.cn

[R36] 并发执行多个任务
来源：http://yk.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ni.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://sh.nicolike.cn

files=$(ls -1)
来源：http://zl.hnjuh.cn

[R38] 管道串联
来源：http://dd.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://mc.shxzukj.cn

[R39] 重定向标准输出与错误
来源：http://tu.wgjwhj.cn

cmd > out.log 2>&1
来源：http://kr.shxzskj.cn

[R40] 追加写日志
来源：http://pl.yuexingan06.cn

echo "log" >> out.log
来源：http://sz.muxihuayi.cn

[R41] 丢弃输出
来源：http://ut.hahajie.cn

cmd >/dev/null 2>&1
来源：http://vw.huanxung.cn

[R42] 输入重定向
来源：http://dk.shtwfgs.cn

wc -l < a.txt
来源：http://vt.gzmigu.cn

[R43] 按名字查找文件
来源：http://qx.panjiajie.cn

find . -name "*.log" -type f
来源：http://wv.panjiajie.cn

[R44] 按修改时间查找
来源：http://hl.9csxet.cn

find . -mtime -7 -type f
来源：http://fe.521024.cn

[R45] 批量删除
来源：http://im.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://da.gzmigu.cn

[R46] 递归替换文件内容
来源：http://fg.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gj.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://zp.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sa.gzmigu.cn

[R48] awk 取指定列
来源：http://ab.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://sg.haigaiapp.cn

[R49] awk 带条件
来源：http://em.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ht.huixiangedu.cn

[R50] awk 求和
来源：http://xt.yuexingan06.cn

awk '{s += $2} END {print s}' a.txt
来源：http://id.gzmigu.cn

[R51] 排序去重取前几
来源：http://hk.newstarts.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://az.bookmarksfly.cn

[R52] 统计行数
来源：http://vo.jianghongdianzi.cn

wc -l a.txt
来源：http://nu.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://ri.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rc.bjjhwx.cn

[R54] 比较两个文件
来源：http://ar.jctech888.com.cn

diff a.txt b.txt
来源：http://jp.nszjky.cn

[R55] 压缩与解压
来源：http://gx.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jz.yuexingan06.cn

[R56] 远程拷贝
来源：http://xv.hnjuh.cn

scp file user@host:/path/
来源：http://cy.yuexingan06.cn

[R57] 远程执行命令
来源：http://dz.jctech888.com.cn

ssh user@host 'uptime'
来源：http://wv.haigaiapp.cn

[R58] 下载文件
来源：http://gf.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gj.nicolike.cn

[R59] 发 POST JSON
来源：http://bi.lnxyls.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ha.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://im.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aj.521024.cn

[R61] 磁盘占用
来源：http://xo.jianghongdianzi.cn

df -h;  du -sh *
来源：http://pg.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://uv.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://ur.jianghongdianzi.cn

[R63] 内存与进程
来源：http://fd.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://ew.bjjhwx.cn

[R64] 结束进程
来源：http://tn.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://hs.lnxyls.cn

[R65] 查看端口占用
来源：http://ew.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ca.haigaiapp.cn

[R66] 定时任务
来源：http://iv.colortex.cn

crontab -e;  crontab -l
来源：http://tt.nszjky.cn

[R67] 生成随机十六进制串
来源：http://bk.szxytkj.cn

openssl rand -hex 16
来源：http://my.haigaiapp.cn

[R68] 计算文件校验值
来源：http://wf.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ck.jctech888.com.cn

[R69] 生成随机密码
来源：http://ak.jianghongdianzi.cn

head -c 16 /dev/urandom | base64
来源：http://sn.hahajie.cn

[R70] 时间戳与互转
来源：http://yf.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://lc.bjjhwx.cn

[R71] 日期格式化
来源：http://he.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kx.bjjhwx.cn

[R72] 等待端口就绪
来源：http://sf.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://du.haigaiapp.cn

[R73] 分割大日志
来源：http://ed.shxzskj.cn

split -l 1000 big.log part_
来源：http://cp.chemitech.net.cn

[R74] 批量重命名
来源：http://cu.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ro.nicolike.cn

[R75] 导出环境变量
来源：http://fa.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.521024.cn

[R76] 使用临时文件
来源：http://op.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ao.colortex.cn

[R77] 读取用户输入
来源：http://lx.gzmigu.cn

read -rp "请输入: " ans
来源：http://fd.muxihuayi.cn

[R78] 交互式菜单
来源：http://ze.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sp.wgjwhj.cn

[R79] 解析命令行选项
来源：http://cf.bookmarksfly.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cg.colortex.cn

[R80] 查看脚本执行耗时
来源：http://ty.panjiajie.cn

time ./run.sh
来源：http://fk.yuexingan06.cn

================================================================================
来源：http://vf.yuntaijiaju.cn

S. C / C++ 专题
来源：http://em.asd995.cn

================================================================================
来源：http://th.asd995.cn

[S01] C：Hello World
来源：http://sl.yuexingan06.cn

#include <stdio.h>
来源：http://vg.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qu.szsharing.cn

[S02] C：变量与格式化输出
来源：http://il.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ll.szxytkj.cn

[S03] C：读入整数
来源：http://au.huanxung.cn

int x; scanf("%d", &x);
来源：http://uz.9csxet.cn

[S04] C：字符串复制
来源：http://cf.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qy.jianghongdianzi.cn

[S05] C：字符串长度
来源：http://xw.newstarts.cn

strlen(s)
来源：http://zf.hahajie.cn

[S06] C：字符串比较
来源：http://rk.huixiangedu.cn

strcmp(a, b) == 0
来源：http://kf.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://ml.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ln.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://gv.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qj.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://sn.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nk.szxytkj.cn

[S10] C：指针与解引用
来源：http://gn.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://xz.chemitech.net.cn

[S11] C：逐行读文件
来源：http://ez.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://mt.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ug.colortex.cn

fclose(f);
来源：http://mk.bookmarksfly.cn

[S12] C：写文件
来源：http://ox.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pk.lnxyls.cn

[S13] C：宏定义
来源：http://ji.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oz.bjjhwx.cn

[S14] C：枚举
来源：http://pl.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://dv.hnjuh.cn

[S15] C：类型转换
来源：http://ks.bjjhwx.cn

(double) a / b
来源：http://sg.wgjwhj.cn

[S16] C：位操作置位
来源：http://bj.newstarts.cn

x |= (1 << 3);
来源：http://vc.jctech888.com.cn

[S17] C：安全拼接字符串
来源：http://ln.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bh.szxytkj.cn

[S18] C：命令行参数
来源：http://jq.nszjky.cn

int main(int argc, char **argv)
来源：http://fo.shxzukj.cn

[S19] C：快速排序
来源：http://hq.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://si.nicolike.cn

[S20] C：二分查找
来源：http://vx.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ve.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://tr.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yx.szsharing.cn

[S22] C：字符串转数字
来源：http://ev.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ji.nszjky.cn

[S23] C：随机数
来源：http://dc.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wt.colortex.cn

[S24] C：获取本地时间
来源：http://ir.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ae.huanxung.cn

[S25] C：内存拷贝
来源：http://ha.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ig.huanxung.cn

[S26] C：内存清零
来源：http://nd.shxzukj.cn

memset(a, 0, sizeof a);
来源：http://xp.yuexingan06.cn

[S27] C：定义常量
来源：http://tw.muxihuayi.cn

const double PI = 3.14159;
来源：http://gq.hahajie.cn

[S28] C：静态变量
来源：http://fz.bookmarksfly.cn

static int counter = 0;
来源：http://fl.huixiangedu.cn

[S29] C：变参函数
来源：http://im.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mm.panjiajie.cn

[S30] C：头文件保护
来源：http://ba.lnxyls.cn

#ifndef X_H
来源：http://xk.nicolike.cn

#define X_H
来源：http://xt.shtwfgs.cn

#endif
来源：http://he.wgjwhj.cn

[S31] C++：Hello World
来源：http://ah.huixinmuqiang.cn

#include <iostream>
来源：http://la.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://ws.9csxet.cn

[S32] C++：字符串
来源：http://xw.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://ri.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://go.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tw.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ij.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://qe.shxzskj.cn


<!-- 参考信息 -->