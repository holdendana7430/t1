代发 wailian999

ROLLBACK TO sp1;
来源：http://gf.szxytkj.cn

[Q69] 查看执行计划
来源：http://tn.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uu.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://rk.yuntaijiaju.cn

ANALYZE TABLE users;
来源：http://qt.bjjhwx.cn

[Q71] 查看建表语句
来源：http://ce.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xo.nszjky.cn

[Q72] 查看索引
来源：http://py.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://ve.bjjhwx.cn

[Q73] 查看表状态
来源：http://vr.wgjwhj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ro.nszjky.cn

[Q74] 强制使用索引
来源：http://pb.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gk.wgjwhj.cn

[Q75] 日期格式化
来源：http://ky.huanxung.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xj.shtwfgs.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kt.bookmarksfly.cn

[Q76] 按天统计
来源：http://ys.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sc.bookmarksfly.cn

[Q77] 时间加减
来源：http://hj.nszjky.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lt.newstarts.cn

[Q78] 当前时间
来源：http://xt.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gz.hahajie.cn

[Q79] 字符串拼接
来源：http://nu.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sm.nszjky.cn

[Q80] 字符串截取
来源：http://rz.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qu.jctech888.com.cn

[Q81] 字符串替换
来源：http://fc.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ss.huixiangedu.cn

[Q82] 字符长度与字节长度
来源：http://vt.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gb.chemitech.net.cn

[Q83] 大小写转换
来源：http://gs.bookmarksfly.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ib.huixiangedu.cn

[Q84] 去除首尾空格
来源：http://px.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://mr.wgjwhj.cn

[Q85] 数值取整
来源：http://id.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gb.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://rc.szsharing.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ej.nicolike.cn

[Q87] JSON 字段做条件
来源：http://tl.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fw.newstarts.cn

[Q88] 行转列（条件聚合）
来源：http://nq.yuexingan06.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fa.muxihuayi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nb.yuntaijiaju.cn

[Q89] 判断表是否存在
来源：http://ia.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bv.szxytkj.cn

[Q90] 生成序号列
来源：http://kh.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dm.muxihuayi.cn

================================================================================
来源：http://qa.nszjky.cn

R. Bash 专题
来源：http://pl.nszjky.cn

================================================================================
来源：http://fa.panjiajie.cn

[R01] shebang 与严格模式
来源：http://es.yuntaijiaju.cn

#!/usr/bin/env bash
来源：http://mc.yuexingan06.cn

set -euo pipefail
来源：http://fz.hnjuh.cn

[R02] 变量赋值与使用
来源：http://xt.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://xb.jianghongdianzi.cn

[R03] 只读变量
来源：http://cx.asd995.cn

readonly PI=3.14
来源：http://pv.panjiajie.cn

[R04] 位置参数
来源：http://oi.newstarts.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lm.gzmigu.cn

[R05] 参数默认值
来源：http://bm.wgjwhj.cn

name="${1:-default}"
来源：http://sw.asd995.cn

[R06] 判断命令是否存在
来源：http://pz.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://um.gzmigu.cn

[R07] if 判断文件
来源：http://wd.hahajie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://um.newstarts.cn

[R08] 数值比较
来源：http://jt.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ky.gzmigu.cn

[R09] 字符串比较
来源：http://go.bookmarksfly.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fe.jianghongdianzi.cn

[R10] 正则匹配
来源：http://bk.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ay.szsharing.cn

[R11] case 多分支
来源：http://wf.haigaiapp.cn

case "$1" in
来源：http://bc.jctech888.com.cn

start) echo "启动" ;;
来源：http://lw.asd995.cn

stop)  echo "停止" ;;
来源：http://gd.huixiangedu.cn

*)     echo "未知命令" ;;
来源：http://wm.shxzskj.cn

esac
来源：http://sh.shtwfgs.cn

[R12] for 遍历文件
来源：http://vq.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://lr.newstarts.cn

[R13] for 计数循环
来源：http://ou.hnjuh.cn

for i in {1..10}; do echo "$i"; done
来源：http://yw.yuntaijiaju.cn

[R14] C 风格 for
来源：http://sk.nicolike.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pv.muxihuayi.cn

[R15] while 逐行读文件
来源：http://us.wgjwhj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mh.nicolike.cn

[R16] until 等待条件
来源：http://dl.chemitech.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qs.huanxung.cn

[R17] 数组定义与取值
来源：http://oa.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hm.asd995.cn

[R18] 遍历数组
来源：http://cv.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uf.colortex.cn

[R19] 数组长度
来源：http://xj.hnjuh.cn

echo "${#arr[@]}"
来源：http://ur.gzmigu.cn

[R20] 关联数组（字典）
来源：http://ut.huixiangedu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jo.haigaiapp.cn

[R21] 字符串长度
来源：http://zd.bookmarksfly.cn

echo "${#s}"
来源：http://rx.huanxung.cn

[R22] 截取子串
来源：http://pl.hnjuh.cn

echo "${s:0:5}"
来源：http://er.shxzukj.cn

[R23] 字符串替换
来源：http://pd.shxzukj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.haigaiapp.cn

[R24] 大小写转换
来源：http://hs.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oc.shxzukj.cn

[R25] 去后缀 / 去前缀
来源：http://nj.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wk.panjiajie.cn

[R26] 命令替换
来源：http://zq.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://ty.shtwfgs.cn

[R27] 算术展开
来源：http://hn.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://nx.yuexingan06.cn

[R28] 浮点运算
来源：http://cs.huanxung.cn

echo "scale=2; 10/3" | bc
来源：http://ia.nicolike.cn

[R29] 定义函数
来源：http://ub.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vg.yuexingan06.cn

[R30] 函数返回状态码
来源：http://qk.lnxyls.cn

f() { return 0; }; f || echo "失败了"
来源：http://rj.muxihuayi.cn

[R31] 局部变量
来源：http://hp.huanxung.cn

f() { local x=1; echo "$x"; }
来源：http://db.shxzukj.cn

[R32] 参数个数校验
来源：http://uc.hnjuh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://un.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://hg.jctech888.com.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jq.shxzskj.cn

[R34] 退出时清理
来源：http://nl.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yn.hnjuh.cn

[R35] 后台执行并等待
来源：http://cd.newstarts.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cn.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://em.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ex.9csxet.cn

[R37] 把输出赋给变量
来源：http://sm.hahajie.cn

files=$(ls -1)
来源：http://vr.521024.cn

[R38] 管道串联
来源：http://gl.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://ud.shxzskj.cn

[R39] 重定向标准输出与错误
来源：http://pj.muxihuayi.cn

cmd > out.log 2>&1
来源：http://sx.jctech888.com.cn

[R40] 追加写日志
来源：http://ep.bookmarksfly.cn

echo "log" >> out.log
来源：http://vn.newstarts.cn

[R41] 丢弃输出
来源：http://dy.lnxyls.cn

cmd >/dev/null 2>&1
来源：http://nj.shtwfgs.cn

[R42] 输入重定向
来源：http://do.gzmigu.cn

wc -l < a.txt
来源：http://es.asd995.cn

[R43] 按名字查找文件
来源：http://zu.huixinmuqiang.cn

find . -name "*.log" -type f
来源：http://gb.nicolike.cn

[R44] 按修改时间查找
来源：http://hh.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://wd.huanxung.cn

[R45] 批量删除
来源：http://px.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://gk.haigaiapp.cn

[R46] 递归替换文件内容
来源：http://ea.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tk.shxzukj.cn

[R47] sed 单行替换
来源：http://vs.yuexingan06.cn

sed -i 's/foo/bar/g' a.txt
来源：http://da.szsharing.cn

[R48] awk 取指定列
来源：http://ge.yuntaijiaju.cn

awk '{print $1, $3}' a.txt
来源：http://hi.muxihuayi.cn

[R49] awk 带条件
来源：http://yu.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rz.jctech888.com.cn

[R50] awk 求和
来源：http://hm.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://av.shxzukj.cn

[R51] 排序去重取前几
来源：http://bw.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yo.newstarts.cn

[R52] 统计行数
来源：http://ci.bjjhwx.cn

wc -l a.txt
来源：http://gs.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://hw.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vu.shxzukj.cn

[R54] 比较两个文件
来源：http://jz.shxzskj.cn

diff a.txt b.txt
来源：http://ro.shxzskj.cn

[R55] 压缩与解压
来源：http://hi.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ed.nicolike.cn

[R56] 远程拷贝
来源：http://vt.asd995.cn

scp file user@host:/path/
来源：http://kf.chemitech.net.cn

[R57] 远程执行命令
来源：http://yt.bookmarksfly.cn

ssh user@host 'uptime'
来源：http://wv.shxzskj.cn

[R58] 下载文件
来源：http://jv.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ed.9csxet.cn

[R59] 发 POST JSON
来源：http://co.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://io.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://sl.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hw.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://nb.colortex.cn

df -h;  du -sh *
来源：http://wr.521024.cn

[R62] 找最占空间的文件
来源：http://pm.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://bs.521024.cn

[R63] 内存与进程
来源：http://rr.asd995.cn

free -h;  ps aux | grep nginx
来源：http://za.hahajie.cn

[R64] 结束进程
来源：http://pt.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://nr.9csxet.cn

[R65] 查看端口占用
来源：http://yv.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://io.colortex.cn

[R66] 定时任务
来源：http://en.lnxyls.cn

crontab -e;  crontab -l
来源：http://tq.colortex.cn

[R67] 生成随机十六进制串
来源：http://zf.huixinmuqiang.cn

openssl rand -hex 16
来源：http://jm.yuexingan06.cn

[R68] 计算文件校验值
来源：http://xe.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ow.asd995.cn

[R69] 生成随机密码
来源：http://gd.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://qq.hahajie.cn

[R70] 时间戳与互转
来源：http://cz.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://tj.521024.cn

[R71] 日期格式化
来源：http://vf.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bq.colortex.cn

[R72] 等待端口就绪
来源：http://wl.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lo.szsharing.cn

[R73] 分割大日志
来源：http://qk.shxzskj.cn

split -l 1000 big.log part_
来源：http://hx.szxytkj.cn

[R74] 批量重命名
来源：http://df.hnjuh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dj.haigaiapp.cn

[R75] 导出环境变量
来源：http://kj.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://fc.bookmarksfly.cn

[R76] 使用临时文件
来源：http://tg.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pk.shxzskj.cn

[R77] 读取用户输入
来源：http://ai.shxzskj.cn

read -rp "请输入: " ans
来源：http://nv.shxzukj.cn

[R78] 交互式菜单
来源：http://ok.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nw.jctech888.com.cn

[R79] 解析命令行选项
来源：http://xi.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yx.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://zk.yuexingan06.cn

time ./run.sh
来源：http://qw.nszjky.cn

================================================================================
来源：http://gd.shtwfgs.cn

S. C / C++ 专题
来源：http://kl.shxzskj.cn

================================================================================
来源：http://gl.jianghongdianzi.cn

[S01] C：Hello World
来源：http://ca.yuntaijiaju.cn

#include <stdio.h>
来源：http://um.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iz.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://jt.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://jt.asd995.cn

[S03] C：读入整数
来源：http://ac.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://cz.9csxet.cn

[S04] C：字符串复制
来源：http://rs.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ae.huixiangedu.cn

[S05] C：字符串长度
来源：http://dj.shxzskj.cn

strlen(s)
来源：http://he.szxytkj.cn

[S06] C：字符串比较
来源：http://au.9csxet.cn

strcmp(a, b) == 0
来源：http://em.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://gr.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rn.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://jl.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fp.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://fn.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ih.szxytkj.cn

[S10] C：指针与解引用
来源：http://km.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://bm.haigaiapp.cn

[S11] C：逐行读文件
来源：http://fb.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://qi.shxzukj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wk.bookmarksfly.cn

fclose(f);
来源：http://si.huanxung.cn

[S12] C：写文件
来源：http://cp.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ax.shxzukj.cn

[S13] C：宏定义
来源：http://qo.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://se.szxytkj.cn

[S14] C：枚举
来源：http://su.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://gj.bookmarksfly.cn

[S15] C：类型转换
来源：http://oj.muxihuayi.cn

(double) a / b
来源：http://ij.nicolike.cn

[S16] C：位操作置位
来源：http://op.yuntaijiaju.cn

x |= (1 << 3);
来源：http://fx.521024.cn

[S17] C：安全拼接字符串
来源：http://py.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zv.chemitech.net.cn

[S18] C：命令行参数
来源：http://ov.521024.cn

int main(int argc, char **argv)
来源：http://hd.szxytkj.cn

[S19] C：快速排序
来源：http://mu.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cq.shxzukj.cn

[S20] C：二分查找
来源：http://yk.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sh.huanxung.cn

[S21] C：字符类别判断
来源：http://oj.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ub.lnxyls.cn

[S22] C：字符串转数字
来源：http://lj.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://au.wgjwhj.cn

[S23] C：随机数
来源：http://bm.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fh.panjiajie.cn

[S24] C：获取本地时间
来源：http://xx.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yb.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ej.hahajie.cn

memcpy(dst, src, n);
来源：http://mt.wgjwhj.cn

[S26] C：内存清零
来源：http://fj.colortex.cn

memset(a, 0, sizeof a);
来源：http://wi.9csxet.cn

[S27] C：定义常量
来源：http://lw.panjiajie.cn

const double PI = 3.14159;
来源：http://vb.jctech888.com.cn

[S28] C：静态变量
来源：http://io.jctech888.com.cn

static int counter = 0;
来源：http://ul.huixinmuqiang.cn

[S29] C：变参函数
来源：http://uo.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://te.huixiangedu.cn

[S30] C：头文件保护
来源：http://ss.szxytkj.cn

#ifndef X_H
来源：http://vl.9csxet.cn

#define X_H
来源：http://ba.shxzskj.cn

#endif
来源：http://gg.bjjhwx.cn

[S31] C++：Hello World
来源：http://ub.bjjhwx.cn

#include <iostream>
来源：http://pz.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://zk.nszjky.cn

[S32] C++：字符串
来源：http://yi.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://mn.shxzskj.cn

[S33] C++：vector 增删
来源：http://dk.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bc.lnxyls.cn

[S34] C++：遍历 vector
来源：http://gv.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://rz.huixinmuqiang.cn

[S35] C++：map
来源：http://ej.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pe.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://xx.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jp.yuntaijiaju.cn

[S37] C++：set
来源：http://xn.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ji.huanxung.cn

[S38] C++：排序
来源：http://eo.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://pz.szxytkj.cn


<!-- 参考信息 -->