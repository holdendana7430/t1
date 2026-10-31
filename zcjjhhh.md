代发 wailian999

ANALYZE TABLE users;
来源：http://cd.huixiangedu.cn

[Q71] 查看建表语句
来源：http://kp.bjjhwx.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ja.jianghongdianzi.cn

[Q72] 查看索引
来源：http://jl.9csxet.cn

SHOW INDEX FROM users;
来源：http://wn.jctech888.com.cn

[Q73] 查看表状态
来源：http://az.huixinmuqiang.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cq.colortex.cn

[Q74] 强制使用索引
来源：http://fe.newstarts.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wk.jctech888.com.cn

[Q75] 日期格式化
来源：http://xb.shtwfgs.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hr.szsharing.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vr.hnjuh.cn

[Q76] 按天统计
来源：http://hl.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fr.yuntaijiaju.cn

[Q77] 时间加减
来源：http://cq.hnjuh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ne.newstarts.cn

[Q78] 当前时间
来源：http://if.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ix.nicolike.cn

[Q79] 字符串拼接
来源：http://wv.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qp.hnjuh.cn

[Q80] 字符串截取
来源：http://rz.asd995.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hm.shtwfgs.cn

[Q81] 字符串替换
来源：http://qm.asd995.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cq.asd995.cn

[Q82] 字符长度与字节长度
来源：http://ci.hnjuh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pg.jctech888.com.cn

[Q83] 大小写转换
来源：http://ux.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xi.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://sw.newstarts.cn

SELECT TRIM(name) FROM users;
来源：http://yc.colortex.cn

[Q85] 数值取整
来源：http://gd.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bj.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://mm.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ro.huanxung.cn

[Q87] JSON 字段做条件
来源：http://oi.chemitech.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pb.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://xv.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bv.chemitech.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wx.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://pj.shtwfgs.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zo.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ig.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ii.panjiajie.cn

================================================================================
来源：http://yg.yuntaijiaju.cn

R. Bash 专题
来源：http://ru.shxzskj.cn

================================================================================
来源：http://hi.jianghongdianzi.cn

[R01] shebang 与严格模式
来源：http://wk.hahajie.cn

#!/usr/bin/env bash
来源：http://bf.lnxyls.cn

set -euo pipefail
来源：http://sn.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://hr.bjjhwx.cn

name="Tom"; echo "$name"
来源：http://bo.huixiangedu.cn

[R03] 只读变量
来源：http://ak.jianghongdianzi.cn

readonly PI=3.14
来源：http://ws.muxihuayi.cn

[R04] 位置参数
来源：http://oy.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bv.nicolike.cn

[R05] 参数默认值
来源：http://fd.newstarts.cn

name="${1:-default}"
来源：http://zg.huanxung.cn

[R06] 判断命令是否存在
来源：http://fq.bookmarksfly.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nr.newstarts.cn

[R07] if 判断文件
来源：http://ui.newstarts.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nq.hahajie.cn

[R08] 数值比较
来源：http://zz.yuexingan06.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fd.colortex.cn

[R09] 字符串比较
来源：http://wz.newstarts.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ik.gzmigu.cn

[R10] 正则匹配
来源：http://uq.chemitech.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ck.gzmigu.cn

[R11] case 多分支
来源：http://ez.jianghongdianzi.cn

case "$1" in
来源：http://iu.nszjky.cn

start) echo "启动" ;;
来源：http://bt.gzmigu.cn

stop)  echo "停止" ;;
来源：http://xl.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://gh.huixiangedu.cn

esac
来源：http://us.jianghongdianzi.cn

[R12] for 遍历文件
来源：http://ot.jianghongdianzi.cn

for f in *.txt; do echo "$f"; done
来源：http://bc.shtwfgs.cn

[R13] for 计数循环
来源：http://tr.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://rh.jianghongdianzi.cn

[R14] C 风格 for
来源：http://py.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gh.colortex.cn

[R15] while 逐行读文件
来源：http://th.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vr.shxzukj.cn

[R16] until 等待条件
来源：http://is.521024.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ft.bjjhwx.cn

[R17] 数组定义与取值
来源：http://du.9csxet.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oe.szsharing.cn

[R18] 遍历数组
来源：http://kd.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jn.lnxyls.cn

[R19] 数组长度
来源：http://iq.shxzukj.cn

echo "${#arr[@]}"
来源：http://qd.gzmigu.cn

[R20] 关联数组（字典）
来源：http://ra.panjiajie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oj.muxihuayi.cn

[R21] 字符串长度
来源：http://os.huanxung.cn

echo "${#s}"
来源：http://wn.bjjhwx.cn

[R22] 截取子串
来源：http://vn.yuntaijiaju.cn

echo "${s:0:5}"
来源：http://aw.yuntaijiaju.cn

[R23] 字符串替换
来源：http://gp.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xe.jianghongdianzi.cn

[R24] 大小写转换
来源：http://qx.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ff.bjjhwx.cn

[R25] 去后缀 / 去前缀
来源：http://lf.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yj.lnxyls.cn

[R26] 命令替换
来源：http://cu.shxzukj.cn

now=$(date +%F); echo "$now"
来源：http://xk.muxihuayi.cn

[R27] 算术展开
来源：http://yp.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://la.haigaiapp.cn

[R28] 浮点运算
来源：http://xx.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://sy.asd995.cn

[R29] 定义函数
来源：http://ln.szsharing.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ky.hahajie.cn

[R30] 函数返回状态码
来源：http://py.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://lj.haigaiapp.cn

[R31] 局部变量
来源：http://th.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://rc.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://dy.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qn.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://kb.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nw.bookmarksfly.cn

[R34] 退出时清理
来源：http://xq.521024.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sj.szxytkj.cn

[R35] 后台执行并等待
来源：http://pn.muxihuayi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gx.panjiajie.cn

[R36] 并发执行多个任务
来源：http://qp.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://va.521024.cn

[R37] 把输出赋给变量
来源：http://in.521024.cn

files=$(ls -1)
来源：http://eh.jianghongdianzi.cn

[R38] 管道串联
来源：http://ne.huanxung.cn

cat a.txt | grep -i error | wc -l
来源：http://sm.bjjhwx.cn

[R39] 重定向标准输出与错误
来源：http://ay.bjjhwx.cn

cmd > out.log 2>&1
来源：http://fr.shxzukj.cn

[R40] 追加写日志
来源：http://qw.shxzskj.cn

echo "log" >> out.log
来源：http://xg.hnjuh.cn

[R41] 丢弃输出
来源：http://px.asd995.cn

cmd >/dev/null 2>&1
来源：http://ij.huixiangedu.cn

[R42] 输入重定向
来源：http://qx.nicolike.cn

wc -l < a.txt
来源：http://fa.hahajie.cn

[R43] 按名字查找文件
来源：http://ns.hahajie.cn

find . -name "*.log" -type f
来源：http://nf.wgjwhj.cn

[R44] 按修改时间查找
来源：http://bh.szsharing.cn

find . -mtime -7 -type f
来源：http://cw.nszjky.cn

[R45] 批量删除
来源：http://ip.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://pz.bjjhwx.cn

[R46] 递归替换文件内容
来源：http://ws.jctech888.com.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://au.lnxyls.cn

[R47] sed 单行替换
来源：http://am.shxzukj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nr.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://ar.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ml.521024.cn

[R49] awk 带条件
来源：http://ml.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jw.muxihuayi.cn

[R50] awk 求和
来源：http://qj.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ls.bjjhwx.cn

[R51] 排序去重取前几
来源：http://px.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://if.panjiajie.cn

[R52] 统计行数
来源：http://fu.shxzukj.cn

wc -l a.txt
来源：http://xr.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://hw.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sb.bjjhwx.cn

[R54] 比较两个文件
来源：http://cx.hnjuh.cn

diff a.txt b.txt
来源：http://lh.haigaiapp.cn

[R55] 压缩与解压
来源：http://gf.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ng.jctech888.com.cn

[R56] 远程拷贝
来源：http://ad.yuntaijiaju.cn

scp file user@host:/path/
来源：http://te.muxihuayi.cn

[R57] 远程执行命令
来源：http://kp.hnjuh.cn

ssh user@host 'uptime'
来源：http://kv.bjjhwx.cn

[R58] 下载文件
来源：http://ye.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hw.hnjuh.cn

[R59] 发 POST JSON
来源：http://kp.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rn.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ep.shtwfgs.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fg.shxzukj.cn

[R61] 磁盘占用
来源：http://ui.nicolike.cn

df -h;  du -sh *
来源：http://yn.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://sa.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://kn.bookmarksfly.cn

[R63] 内存与进程
来源：http://dd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://oi.wgjwhj.cn

[R64] 结束进程
来源：http://de.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://ul.9csxet.cn

[R65] 查看端口占用
来源：http://ot.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nh.huixiangedu.cn

[R66] 定时任务
来源：http://oy.shxzukj.cn

crontab -e;  crontab -l
来源：http://fm.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://ui.szxytkj.cn

openssl rand -hex 16
来源：http://mq.gzmigu.cn

[R68] 计算文件校验值
来源：http://pn.colortex.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pq.lnxyls.cn

[R69] 生成随机密码
来源：http://mt.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://au.jctech888.com.cn

[R70] 时间戳与互转
来源：http://kk.szsharing.cn

date +%s;  date -d @1700000000
来源：http://fa.nicolike.cn

[R71] 日期格式化
来源：http://ub.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://js.shtwfgs.cn

[R72] 等待端口就绪
来源：http://jk.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dh.chemitech.net.cn

[R73] 分割大日志
来源：http://gb.asd995.cn

split -l 1000 big.log part_
来源：http://ar.chemitech.net.cn

[R74] 批量重命名
来源：http://cu.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bb.hnjuh.cn

[R75] 导出环境变量
来源：http://ra.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://ee.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://fl.bjjhwx.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qk.hahajie.cn

[R77] 读取用户输入
来源：http://ut.shxzukj.cn

read -rp "请输入: " ans
来源：http://jm.bookmarksfly.cn

[R78] 交互式菜单
来源：http://pb.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ob.szsharing.cn

[R79] 解析命令行选项
来源：http://oe.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hb.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://lx.jctech888.com.cn

time ./run.sh
来源：http://qe.panjiajie.cn

================================================================================
来源：http://hv.huanxung.cn

S. C / C++ 专题
来源：http://fp.haigaiapp.cn

================================================================================
来源：http://xz.shxzukj.cn

[S01] C：Hello World
来源：http://oy.yuexingan06.cn

#include <stdio.h>
来源：http://ub.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aj.colortex.cn

[S02] C：变量与格式化输出
来源：http://lv.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ba.panjiajie.cn

[S03] C：读入整数
来源：http://lm.newstarts.cn

int x; scanf("%d", &x);
来源：http://up.lnxyls.cn

[S04] C：字符串复制
来源：http://xb.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eu.nszjky.cn

[S05] C：字符串长度
来源：http://pn.9csxet.cn

strlen(s)
来源：http://cu.szsharing.cn

[S06] C：字符串比较
来源：http://ot.nicolike.cn

strcmp(a, b) == 0
来源：http://es.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://xz.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ts.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://df.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zi.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://hb.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mt.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://fl.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://lw.hahajie.cn

[S11] C：逐行读文件
来源：http://gk.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://fi.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qc.huixiangedu.cn

fclose(f);
来源：http://ub.wgjwhj.cn

[S12] C：写文件
来源：http://mt.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rm.nszjky.cn

[S13] C：宏定义
来源：http://ck.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eg.yuntaijiaju.cn

[S14] C：枚举
来源：http://wk.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://zw.huixiangedu.cn

[S15] C：类型转换
来源：http://lv.yuntaijiaju.cn

(double) a / b
来源：http://gf.wgjwhj.cn

[S16] C：位操作置位
来源：http://ub.chemitech.net.cn

x |= (1 << 3);
来源：http://jv.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://qe.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bf.shxzukj.cn

[S18] C：命令行参数
来源：http://mr.hahajie.cn

int main(int argc, char **argv)
来源：http://pb.huixinmuqiang.cn

[S19] C：快速排序
来源：http://gx.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://db.gzmigu.cn

[S20] C：二分查找
来源：http://gl.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ww.haigaiapp.cn

[S21] C：字符类别判断
来源：http://pa.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pr.hnjuh.cn

[S22] C：字符串转数字
来源：http://uc.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xl.huixiangedu.cn

[S23] C：随机数
来源：http://si.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://an.szxytkj.cn

[S24] C：获取本地时间
来源：http://ed.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zm.haigaiapp.cn

[S25] C：内存拷贝
来源：http://fd.521024.cn

memcpy(dst, src, n);
来源：http://ey.hahajie.cn

[S26] C：内存清零
来源：http://us.521024.cn

memset(a, 0, sizeof a);
来源：http://cl.nicolike.cn

[S27] C：定义常量
来源：http://sf.lnxyls.cn

const double PI = 3.14159;
来源：http://er.yuexingan06.cn

[S28] C：静态变量
来源：http://ro.szsharing.cn

static int counter = 0;
来源：http://cf.yuexingan06.cn

[S29] C：变参函数
来源：http://qz.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rk.chemitech.net.cn

[S30] C：头文件保护
来源：http://rq.9csxet.cn

#ifndef X_H
来源：http://ux.nicolike.cn

#define X_H
来源：http://up.jianghongdianzi.cn

#endif
来源：http://pp.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://hl.nicolike.cn

#include <iostream>
来源：http://ix.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://sq.yuexingan06.cn

[S32] C++：字符串
来源：http://yg.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://vh.szsharing.cn

[S33] C++：vector 增删
来源：http://ni.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oh.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://bo.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://kv.lnxyls.cn

[S35] C++：map
来源：http://mu.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fs.szsharing.cn

[S36] C++：unordered_map
来源：http://po.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uc.9csxet.cn

[S37] C++：set
来源：http://ik.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bv.wgjwhj.cn

[S38] C++：排序
来源：http://zs.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://jk.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://df.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://an.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://tz.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bb.huanxung.cn


<!-- 参考信息 -->