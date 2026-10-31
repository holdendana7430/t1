代发 wailian999

ANALYZE TABLE users;
来源：http://yf.szsharing.cn

[Q71] 查看建表语句
来源：http://nx.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ri.szsharing.cn

[Q72] 查看索引
来源：http://uy.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://gu.wgjwhj.cn

[Q73] 查看表状态
来源：http://bz.yuntaijiaju.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hv.panjiajie.cn

[Q74] 强制使用索引
来源：http://xp.shxzukj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rj.nszjky.cn

[Q75] 日期格式化
来源：http://pz.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hq.521024.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ui.newstarts.cn

[Q76] 按天统计
来源：http://di.lnxyls.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xg.muxihuayi.cn

[Q77] 时间加减
来源：http://ct.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ol.chemitech.net.cn

[Q78] 当前时间
来源：http://ss.muxihuayi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yi.colortex.cn

[Q79] 字符串拼接
来源：http://rj.colortex.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ph.jctech888.com.cn

[Q80] 字符串截取
来源：http://sq.gzmigu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ur.huixiangedu.cn

[Q81] 字符串替换
来源：http://cr.szsharing.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dq.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ah.shxzukj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ga.lnxyls.cn

[Q83] 大小写转换
来源：http://cq.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xs.hahajie.cn

[Q84] 去除首尾空格
来源：http://bl.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://ep.newstarts.cn

[Q85] 数值取整
来源：http://pd.haigaiapp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ch.wgjwhj.cn

[Q86] 读取 JSON 字段
来源：http://af.colortex.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ec.yuexingan06.cn

[Q87] JSON 字段做条件
来源：http://gv.szxytkj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://py.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://rs.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://to.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kd.521024.cn

[Q89] 判断表是否存在
来源：http://qk.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ea.panjiajie.cn

[Q90] 生成序号列
来源：http://qk.chemitech.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ec.panjiajie.cn

================================================================================
来源：http://bj.newstarts.cn

R. Bash 专题
来源：http://dy.muxihuayi.cn

================================================================================
来源：http://hh.colortex.cn

[R01] shebang 与严格模式
来源：http://rm.szxytkj.cn

#!/usr/bin/env bash
来源：http://nq.szsharing.cn

set -euo pipefail
来源：http://nl.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://kd.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://sc.colortex.cn

[R03] 只读变量
来源：http://ev.huixinmuqiang.cn

readonly PI=3.14
来源：http://lq.bjjhwx.cn

[R04] 位置参数
来源：http://jr.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ee.shtwfgs.cn

[R05] 参数默认值
来源：http://fo.panjiajie.cn

name="${1:-default}"
来源：http://mo.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://wq.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wf.yuexingan06.cn

[R07] if 判断文件
来源：http://xk.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oo.asd995.cn

[R08] 数值比较
来源：http://rs.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oj.newstarts.cn

[R09] 字符串比较
来源：http://je.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tw.wgjwhj.cn

[R10] 正则匹配
来源：http://qi.9csxet.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://el.szsharing.cn

[R11] case 多分支
来源：http://hp.panjiajie.cn

case "$1" in
来源：http://jx.gzmigu.cn

start) echo "启动" ;;
来源：http://pb.lnxyls.cn

stop)  echo "停止" ;;
来源：http://fp.shxzskj.cn

*)     echo "未知命令" ;;
来源：http://qj.bookmarksfly.cn

esac
来源：http://ru.wgjwhj.cn

[R12] for 遍历文件
来源：http://ey.bjjhwx.cn

for f in *.txt; do echo "$f"; done
来源：http://qn.chemitech.net.cn

[R13] for 计数循环
来源：http://kb.panjiajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://gp.haigaiapp.cn

[R14] C 风格 for
来源：http://lo.bookmarksfly.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ew.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://rd.jctech888.com.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jk.wgjwhj.cn

[R16] until 等待条件
来源：http://nm.shxzskj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xu.shxzskj.cn

[R17] 数组定义与取值
来源：http://or.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yu.nszjky.cn

[R18] 遍历数组
来源：http://xh.bookmarksfly.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vp.521024.cn

[R19] 数组长度
来源：http://ez.gzmigu.cn

echo "${#arr[@]}"
来源：http://lg.shxzskj.cn

[R20] 关联数组（字典）
来源：http://oe.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://it.panjiajie.cn

[R21] 字符串长度
来源：http://ds.shxzukj.cn

echo "${#s}"
来源：http://xy.yuexingan06.cn

[R22] 截取子串
来源：http://kb.bjjhwx.cn

echo "${s:0:5}"
来源：http://fp.shxzskj.cn

[R23] 字符串替换
来源：http://xf.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zq.szsharing.cn

[R24] 大小写转换
来源：http://tw.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://er.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://wz.huixiangedu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bc.chemitech.net.cn

[R26] 命令替换
来源：http://ji.hahajie.cn

now=$(date +%F); echo "$now"
来源：http://yz.huanxung.cn

[R27] 算术展开
来源：http://ak.huanxung.cn

echo $((1 + 2 * 3))
来源：http://mq.szxytkj.cn

[R28] 浮点运算
来源：http://mc.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://kd.lnxyls.cn

[R29] 定义函数
来源：http://ki.shxzukj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ej.haigaiapp.cn

[R30] 函数返回状态码
来源：http://ax.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://tq.huixiangedu.cn

[R31] 局部变量
来源：http://df.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://pc.colortex.cn

[R32] 参数个数校验
来源：http://zo.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rg.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://xw.bjjhwx.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xt.gzmigu.cn

[R34] 退出时清理
来源：http://pr.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aw.bjjhwx.cn

[R35] 后台执行并等待
来源：http://cm.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xk.szxytkj.cn

[R36] 并发执行多个任务
来源：http://bb.huixiangedu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yl.jctech888.com.cn

[R37] 把输出赋给变量
来源：http://uj.wgjwhj.cn

files=$(ls -1)
来源：http://tb.huixinmuqiang.cn

[R38] 管道串联
来源：http://vp.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://hd.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://nd.9csxet.cn

cmd > out.log 2>&1
来源：http://kj.hnjuh.cn

[R40] 追加写日志
来源：http://da.yuexingan06.cn

echo "log" >> out.log
来源：http://vo.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://ba.nicolike.cn

cmd >/dev/null 2>&1
来源：http://xr.huixinmuqiang.cn

[R42] 输入重定向
来源：http://kc.bjjhwx.cn

wc -l < a.txt
来源：http://kc.bjjhwx.cn

[R43] 按名字查找文件
来源：http://cl.wgjwhj.cn

find . -name "*.log" -type f
来源：http://lh.chemitech.net.cn

[R44] 按修改时间查找
来源：http://ge.jianghongdianzi.cn

find . -mtime -7 -type f
来源：http://qb.szsharing.cn

[R45] 批量删除
来源：http://yb.panjiajie.cn

find . -name "*.tmp" -delete
来源：http://ps.nicolike.cn

[R46] 递归替换文件内容
来源：http://na.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hc.shtwfgs.cn

[R47] sed 单行替换
来源：http://hh.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pz.yuexingan06.cn

[R48] awk 取指定列
来源：http://dn.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://mx.nszjky.cn

[R49] awk 带条件
来源：http://xe.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fa.nicolike.cn

[R50] awk 求和
来源：http://uk.haigaiapp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zt.521024.cn

[R51] 排序去重取前几
来源：http://zy.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yy.lnxyls.cn

[R52] 统计行数
来源：http://mv.asd995.cn

wc -l a.txt
来源：http://ho.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://js.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bm.yuexingan06.cn

[R54] 比较两个文件
来源：http://dc.huixiangedu.cn

diff a.txt b.txt
来源：http://uy.yuexingan06.cn

[R55] 压缩与解压
来源：http://uj.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://or.hnjuh.cn

[R56] 远程拷贝
来源：http://do.colortex.cn

scp file user@host:/path/
来源：http://xp.bjjhwx.cn

[R57] 远程执行命令
来源：http://sh.lnxyls.cn

ssh user@host 'uptime'
来源：http://by.chemitech.net.cn

[R58] 下载文件
来源：http://bo.gzmigu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ql.wgjwhj.cn

[R59] 发 POST JSON
来源：http://yn.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dj.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://pr.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bg.wgjwhj.cn

[R61] 磁盘占用
来源：http://xo.gzmigu.cn

df -h;  du -sh *
来源：http://by.9csxet.cn

[R62] 找最占空间的文件
来源：http://vq.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://hr.yuntaijiaju.cn

[R63] 内存与进程
来源：http://dv.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://ph.hahajie.cn

[R64] 结束进程
来源：http://th.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://td.shxzskj.cn

[R65] 查看端口占用
来源：http://nz.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oy.gzmigu.cn

[R66] 定时任务
来源：http://mp.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://ok.szsharing.cn

[R67] 生成随机十六进制串
来源：http://hm.bjjhwx.cn

openssl rand -hex 16
来源：http://of.bjjhwx.cn

[R68] 计算文件校验值
来源：http://gw.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jr.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://wg.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://dw.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ky.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://ap.huixiangedu.cn

[R71] 日期格式化
来源：http://ig.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hc.szxytkj.cn

[R72] 等待端口就绪
来源：http://cw.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hg.asd995.cn

[R73] 分割大日志
来源：http://ge.yuexingan06.cn

split -l 1000 big.log part_
来源：http://dc.huixinmuqiang.cn

[R74] 批量重命名
来源：http://yu.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dq.asd995.cn

[R75] 导出环境变量
来源：http://ja.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://sj.hahajie.cn

[R76] 使用临时文件
来源：http://tf.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fd.panjiajie.cn

[R77] 读取用户输入
来源：http://dz.shxzukj.cn

read -rp "请输入: " ans
来源：http://qw.bookmarksfly.cn

[R78] 交互式菜单
来源：http://li.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ps.haigaiapp.cn

[R79] 解析命令行选项
来源：http://mo.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rj.newstarts.cn

[R80] 查看脚本执行耗时
来源：http://qc.nicolike.cn

time ./run.sh
来源：http://om.jctech888.com.cn

================================================================================
来源：http://zp.yuntaijiaju.cn

S. C / C++ 专题
来源：http://pw.nszjky.cn

================================================================================
来源：http://lj.jianghongdianzi.cn

[S01] C：Hello World
来源：http://ln.9csxet.cn

#include <stdio.h>
来源：http://pv.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ee.521024.cn

[S02] C：变量与格式化输出
来源：http://mq.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://lz.asd995.cn

[S03] C：读入整数
来源：http://jg.wgjwhj.cn

int x; scanf("%d", &x);
来源：http://ff.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://an.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oy.hnjuh.cn

[S05] C：字符串长度
来源：http://hv.jianghongdianzi.cn

strlen(s)
来源：http://eq.nszjky.cn

[S06] C：字符串比较
来源：http://vh.muxihuayi.cn

strcmp(a, b) == 0
来源：http://rm.lnxyls.cn

[S07] C：数组遍历求和
来源：http://ay.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tn.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://bq.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zv.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://zk.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oi.shxzukj.cn

[S10] C：指针与解引用
来源：http://iq.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://rq.haigaiapp.cn

[S11] C：逐行读文件
来源：http://hs.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://gj.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.bookmarksfly.cn

fclose(f);
来源：http://jf.szsharing.cn

[S12] C：写文件
来源：http://sv.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ub.bjjhwx.cn

[S13] C：宏定义
来源：http://ft.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ux.szxytkj.cn

[S14] C：枚举
来源：http://ig.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://js.haigaiapp.cn

[S15] C：类型转换
来源：http://hg.9csxet.cn

(double) a / b
来源：http://kb.huixiangedu.cn

[S16] C：位操作置位
来源：http://of.shtwfgs.cn

x |= (1 << 3);
来源：http://qc.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://df.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lm.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://lx.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://ui.shtwfgs.cn

[S19] C：快速排序
来源：http://cz.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://us.521024.cn

[S20] C：二分查找
来源：http://rk.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qc.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://lz.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kz.gzmigu.cn

[S22] C：字符串转数字
来源：http://yp.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yu.shxzskj.cn

[S23] C：随机数
来源：http://tf.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://la.shxzskj.cn

[S24] C：获取本地时间
来源：http://uj.huixiangedu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pz.chemitech.net.cn

[S25] C：内存拷贝
来源：http://pv.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://wp.asd995.cn

[S26] C：内存清零
来源：http://du.szsharing.cn

memset(a, 0, sizeof a);
来源：http://lg.huanxung.cn

[S27] C：定义常量
来源：http://fi.asd995.cn

const double PI = 3.14159;
来源：http://ce.shxzskj.cn

[S28] C：静态变量
来源：http://ds.bookmarksfly.cn

static int counter = 0;
来源：http://ky.panjiajie.cn

[S29] C：变参函数
来源：http://io.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tz.521024.cn

[S30] C：头文件保护
来源：http://yx.muxihuayi.cn

#ifndef X_H
来源：http://kx.9csxet.cn

#define X_H
来源：http://wz.asd995.cn

#endif
来源：http://hl.newstarts.cn

[S31] C++：Hello World
来源：http://ar.szxytkj.cn

#include <iostream>
来源：http://kj.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://yv.521024.cn

[S32] C++：字符串
来源：http://rz.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://uc.521024.cn

[S33] C++：vector 增删
来源：http://xx.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xp.panjiajie.cn

[S34] C++：遍历 vector
来源：http://xp.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ab.colortex.cn

[S35] C++：map
来源：http://dm.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fo.gzmigu.cn

[S36] C++：unordered_map
来源：http://ro.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yv.szsharing.cn

[S37] C++：set
来源：http://vm.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sv.huixiangedu.cn

[S38] C++：排序
来源：http://bp.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://hj.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://ya.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hm.521024.cn

[S40] C++：查找元素
来源：http://sw.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lu.asd995.cn


<!-- 参考信息 -->