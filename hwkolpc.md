代发 wailian999

ROLLBACK TO sp1;
来源：http://xp.colortex.cn

[Q69] 查看执行计划
来源：http://js.hnjuh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zz.lnxyls.cn

[Q70] 更新统计信息
来源：http://zq.nszjky.cn

ANALYZE TABLE users;
来源：http://ox.shtwfgs.cn

[Q71] 查看建表语句
来源：http://zl.haigaiapp.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sh.haigaiapp.cn

[Q72] 查看索引
来源：http://jo.lnxyls.cn

SHOW INDEX FROM users;
来源：http://if.shxzskj.cn

[Q73] 查看表状态
来源：http://ss.szsharing.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rh.muxihuayi.cn

[Q74] 强制使用索引
来源：http://ne.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ip.bjjhwx.cn

[Q75] 日期格式化
来源：http://vg.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xa.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pb.hnjuh.cn

[Q76] 按天统计
来源：http://xk.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ni.newstarts.cn

[Q77] 时间加减
来源：http://ck.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lw.shxzukj.cn

[Q78] 当前时间
来源：http://ix.gzmigu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dh.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://cg.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sw.muxihuayi.cn

[Q80] 字符串截取
来源：http://rr.nszjky.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://at.wgjwhj.cn

[Q81] 字符串替换
来源：http://nr.shxzukj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ci.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://wm.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gb.huixiangedu.cn

[Q83] 大小写转换
来源：http://dh.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oa.hahajie.cn

[Q84] 去除首尾空格
来源：http://vd.huanxung.cn

SELECT TRIM(name) FROM users;
来源：http://dt.9csxet.cn

[Q85] 数值取整
来源：http://wf.huixiangedu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.hnjuh.cn

[Q86] 读取 JSON 字段
来源：http://ov.muxihuayi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zu.colortex.cn

[Q87] JSON 字段做条件
来源：http://ox.asd995.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mo.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://mz.haigaiapp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fb.shxzskj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://us.lnxyls.cn

[Q89] 判断表是否存在
来源：http://ai.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://do.szxytkj.cn

[Q90] 生成序号列
来源：http://wa.muxihuayi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rj.huanxung.cn

================================================================================
来源：http://vj.haigaiapp.cn

R. Bash 专题
来源：http://rc.nicolike.cn

================================================================================
来源：http://wz.jctech888.com.cn

[R01] shebang 与严格模式
来源：http://yj.nicolike.cn

#!/usr/bin/env bash
来源：http://yi.shxzskj.cn

set -euo pipefail
来源：http://jf.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://rh.hahajie.cn

name="Tom"; echo "$name"
来源：http://tj.szxytkj.cn

[R03] 只读变量
来源：http://ap.hnjuh.cn

readonly PI=3.14
来源：http://ec.huixinmuqiang.cn

[R04] 位置参数
来源：http://fh.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kl.lnxyls.cn

[R05] 参数默认值
来源：http://pi.nicolike.cn

name="${1:-default}"
来源：http://gl.szxytkj.cn

[R06] 判断命令是否存在
来源：http://sy.szxytkj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ha.gzmigu.cn

[R07] if 判断文件
来源：http://ap.wgjwhj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xc.bookmarksfly.cn

[R08] 数值比较
来源：http://kt.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ig.huanxung.cn

[R09] 字符串比较
来源：http://xq.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fj.shxzukj.cn

[R10] 正则匹配
来源：http://yh.asd995.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pn.gzmigu.cn

[R11] case 多分支
来源：http://oi.bjjhwx.cn

case "$1" in
来源：http://tr.wgjwhj.cn

start) echo "启动" ;;
来源：http://rb.newstarts.cn

stop)  echo "停止" ;;
来源：http://nq.hahajie.cn

*)     echo "未知命令" ;;
来源：http://kq.hnjuh.cn

esac
来源：http://pi.521024.cn

[R12] for 遍历文件
来源：http://mk.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://jz.lnxyls.cn

[R13] for 计数循环
来源：http://gz.lnxyls.cn

for i in {1..10}; do echo "$i"; done
来源：http://au.muxihuayi.cn

[R14] C 风格 for
来源：http://dv.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rz.newstarts.cn

[R15] while 逐行读文件
来源：http://ag.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fh.asd995.cn

[R16] until 等待条件
来源：http://hu.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sh.lnxyls.cn

[R17] 数组定义与取值
来源：http://pr.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ef.shxzukj.cn

[R18] 遍历数组
来源：http://ox.yuexingan06.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mm.yuexingan06.cn

[R19] 数组长度
来源：http://tx.shxzukj.cn

echo "${#arr[@]}"
来源：http://um.asd995.cn

[R20] 关联数组（字典）
来源：http://ra.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ea.muxihuayi.cn

[R21] 字符串长度
来源：http://zd.wgjwhj.cn

echo "${#s}"
来源：http://oz.chemitech.net.cn

[R22] 截取子串
来源：http://xa.haigaiapp.cn

echo "${s:0:5}"
来源：http://ci.yuexingan06.cn

[R23] 字符串替换
来源：http://oi.huixinmuqiang.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lf.nicolike.cn

[R24] 大小写转换
来源：http://rg.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cr.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://fp.szsharing.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rf.yuexingan06.cn

[R26] 命令替换
来源：http://zy.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://rt.521024.cn

[R27] 算术展开
来源：http://nq.colortex.cn

echo $((1 + 2 * 3))
来源：http://vn.haigaiapp.cn

[R28] 浮点运算
来源：http://gh.panjiajie.cn

echo "scale=2; 10/3" | bc
来源：http://mk.shxzskj.cn

[R29] 定义函数
来源：http://mx.521024.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fb.shxzskj.cn

[R30] 函数返回状态码
来源：http://sl.chemitech.net.cn

f() { return 0; }; f || echo "失败了"
来源：http://sc.521024.cn

[R31] 局部变量
来源：http://pk.9csxet.cn

f() { local x=1; echo "$x"; }
来源：http://fw.shxzskj.cn

[R32] 参数个数校验
来源：http://jw.shxzskj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bv.asd995.cn

[R33] 捕获错误并提示行号
来源：http://aw.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rl.yuexingan06.cn

[R34] 退出时清理
来源：http://zc.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qb.yuexingan06.cn

[R35] 后台执行并等待
来源：http://qu.szsharing.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pc.bookmarksfly.cn

[R36] 并发执行多个任务
来源：http://yb.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yz.huixiangedu.cn

[R37] 把输出赋给变量
来源：http://go.gzmigu.cn

files=$(ls -1)
来源：http://dd.jianghongdianzi.cn

[R38] 管道串联
来源：http://wi.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://my.lnxyls.cn

[R39] 重定向标准输出与错误
来源：http://bc.gzmigu.cn

cmd > out.log 2>&1
来源：http://oy.shxzukj.cn

[R40] 追加写日志
来源：http://wo.gzmigu.cn

echo "log" >> out.log
来源：http://wh.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://dl.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://qp.521024.cn

[R42] 输入重定向
来源：http://tc.huanxung.cn

wc -l < a.txt
来源：http://fy.jctech888.com.cn

[R43] 按名字查找文件
来源：http://tf.nszjky.cn

find . -name "*.log" -type f
来源：http://gm.yuntaijiaju.cn

[R44] 按修改时间查找
来源：http://uh.colortex.cn

find . -mtime -7 -type f
来源：http://dc.nszjky.cn

[R45] 批量删除
来源：http://ya.szsharing.cn

find . -name "*.tmp" -delete
来源：http://la.hnjuh.cn

[R46] 递归替换文件内容
来源：http://nt.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wn.szsharing.cn

[R47] sed 单行替换
来源：http://rn.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qa.haigaiapp.cn

[R48] awk 取指定列
来源：http://lp.gzmigu.cn

awk '{print $1, $3}' a.txt
来源：http://oo.muxihuayi.cn

[R49] awk 带条件
来源：http://ff.jctech888.com.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yr.yuntaijiaju.cn

[R50] awk 求和
来源：http://tk.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ek.lnxyls.cn

[R51] 排序去重取前几
来源：http://ou.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tx.9csxet.cn

[R52] 统计行数
来源：http://bs.9csxet.cn

wc -l a.txt
来源：http://tm.haigaiapp.cn

[R53] 查看文件头与实时尾
来源：http://wx.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kc.nicolike.cn

[R54] 比较两个文件
来源：http://dg.haigaiapp.cn

diff a.txt b.txt
来源：http://ko.nicolike.cn

[R55] 压缩与解压
来源：http://ec.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pi.szsharing.cn

[R56] 远程拷贝
来源：http://oe.newstarts.cn

scp file user@host:/path/
来源：http://ia.lnxyls.cn

[R57] 远程执行命令
来源：http://dj.panjiajie.cn

ssh user@host 'uptime'
来源：http://wg.newstarts.cn

[R58] 下载文件
来源：http://ky.shtwfgs.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oc.newstarts.cn

[R59] 发 POST JSON
来源：http://af.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ia.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://by.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kt.yuexingan06.cn

[R61] 磁盘占用
来源：http://hw.chemitech.net.cn

df -h;  du -sh *
来源：http://nh.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ao.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://jp.newstarts.cn

[R63] 内存与进程
来源：http://wz.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://tu.jianghongdianzi.cn

[R64] 结束进程
来源：http://te.gzmigu.cn

kill -9 $(pgrep -f app.py)
来源：http://ci.colortex.cn

[R65] 查看端口占用
来源：http://sx.szxytkj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ln.nicolike.cn

[R66] 定时任务
来源：http://so.colortex.cn

crontab -e;  crontab -l
来源：http://gp.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://df.haigaiapp.cn

openssl rand -hex 16
来源：http://ab.hnjuh.cn

[R68] 计算文件校验值
来源：http://bs.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qt.9csxet.cn

[R69] 生成随机密码
来源：http://lh.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://bj.huixinmuqiang.cn

[R70] 时间戳与互转
来源：http://sa.nicolike.cn

date +%s;  date -d @1700000000
来源：http://ga.9csxet.cn

[R71] 日期格式化
来源：http://fn.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://us.lnxyls.cn

[R72] 等待端口就绪
来源：http://yy.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fq.muxihuayi.cn

[R73] 分割大日志
来源：http://vt.gzmigu.cn

split -l 1000 big.log part_
来源：http://df.shtwfgs.cn

[R74] 批量重命名
来源：http://lj.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tf.9csxet.cn

[R75] 导出环境变量
来源：http://tb.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://ak.hahajie.cn

[R76] 使用临时文件
来源：http://wi.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wu.9csxet.cn

[R77] 读取用户输入
来源：http://vd.szxytkj.cn

read -rp "请输入: " ans
来源：http://fd.nicolike.cn

[R78] 交互式菜单
来源：http://cv.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qo.yuexingan06.cn

[R79] 解析命令行选项
来源：http://gg.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://rw.jctech888.com.cn

time ./run.sh
来源：http://vf.nszjky.cn

================================================================================
来源：http://wa.521024.cn

S. C / C++ 专题
来源：http://jh.nicolike.cn

================================================================================
来源：http://vr.shtwfgs.cn

[S01] C：Hello World
来源：http://wm.huanxung.cn

#include <stdio.h>
来源：http://ke.haigaiapp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dp.nszjky.cn

[S02] C：变量与格式化输出
来源：http://lb.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://fe.huixinmuqiang.cn

[S03] C：读入整数
来源：http://eq.9csxet.cn

int x; scanf("%d", &x);
来源：http://cx.nszjky.cn

[S04] C：字符串复制
来源：http://zk.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yk.haigaiapp.cn

[S05] C：字符串长度
来源：http://ql.haigaiapp.cn

strlen(s)
来源：http://ix.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pa.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://ak.asd995.cn

[S07] C：数组遍历求和
来源：http://nn.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gq.521024.cn

[S08] C：动态内存分配与释放
来源：http://wz.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://my.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://fx.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wp.asd995.cn

[S10] C：指针与解引用
来源：http://uw.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://jm.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://uo.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ff.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dl.jctech888.com.cn

fclose(f);
来源：http://xn.nszjky.cn

[S12] C：写文件
来源：http://qm.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xk.colortex.cn

[S13] C：宏定义
来源：http://tk.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hy.muxihuayi.cn

[S14] C：枚举
来源：http://jn.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ba.521024.cn

[S15] C：类型转换
来源：http://mk.shxzukj.cn

(double) a / b
来源：http://ct.yuexingan06.cn

[S16] C：位操作置位
来源：http://vj.asd995.cn

x |= (1 << 3);
来源：http://uh.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://zx.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vj.hahajie.cn

[S18] C：命令行参数
来源：http://xu.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://ui.colortex.cn

[S19] C：快速排序
来源：http://zb.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jl.panjiajie.cn

[S20] C：二分查找
来源：http://ny.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fp.9csxet.cn

[S21] C：字符类别判断
来源：http://hj.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rn.szxytkj.cn

[S22] C：字符串转数字
来源：http://fv.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xf.jctech888.com.cn

[S23] C：随机数
来源：http://fy.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ta.hnjuh.cn

[S24] C：获取本地时间
来源：http://jz.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pt.nszjky.cn

[S25] C：内存拷贝
来源：http://mr.colortex.cn

memcpy(dst, src, n);
来源：http://au.huixinmuqiang.cn

[S26] C：内存清零
来源：http://hr.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://by.jctech888.com.cn

[S27] C：定义常量
来源：http://fb.jctech888.com.cn

const double PI = 3.14159;
来源：http://sp.muxihuayi.cn

[S28] C：静态变量
来源：http://mc.nszjky.cn

static int counter = 0;
来源：http://gt.shxzskj.cn

[S29] C：变参函数
来源：http://ye.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sf.nicolike.cn

[S30] C：头文件保护
来源：http://ac.asd995.cn

#ifndef X_H
来源：http://iu.bookmarksfly.cn

#define X_H
来源：http://ta.shxzukj.cn

#endif
来源：http://df.haigaiapp.cn

[S31] C++：Hello World
来源：http://dp.hahajie.cn

#include <iostream>
来源：http://bl.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://dn.9csxet.cn

[S32] C++：字符串
来源：http://nv.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ve.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ij.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jh.newstarts.cn

[S34] C++：遍历 vector
来源：http://wk.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://my.yuntaijiaju.cn

[S35] C++：map
来源：http://bd.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hh.521024.cn

[S36] C++：unordered_map
来源：http://bx.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iw.muxihuayi.cn

[S37] C++：set
来源：http://tw.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zl.shxzukj.cn

[S38] C++：排序
来源：http://lt.colortex.cn

std::sort(v.begin(), v.end());
来源：http://aa.huixiangedu.cn


<!-- 参考信息 -->