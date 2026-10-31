代发 wailian999

ANALYZE TABLE users;
来源：http://wo.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://le.shtwfgs.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://so.szxytkj.cn

[Q72] 查看索引
来源：http://zx.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://wp.shxzukj.cn

[Q73] 查看表状态
来源：http://xx.yuexingan06.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sw.szxytkj.cn

[Q74] 强制使用索引
来源：http://wq.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zd.yuntaijiaju.cn

[Q75] 日期格式化
来源：http://jx.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iw.newstarts.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vd.asd995.cn

[Q76] 按天统计
来源：http://ko.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fx.gzmigu.cn

[Q77] 时间加减
来源：http://vr.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ec.szxytkj.cn

[Q78] 当前时间
来源：http://kr.lnxyls.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://km.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://wp.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sf.newstarts.cn

[Q80] 字符串截取
来源：http://sh.521024.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oy.lnxyls.cn

[Q81] 字符串替换
来源：http://io.nicolike.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wd.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://ru.yuntaijiaju.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gu.nicolike.cn

[Q83] 大小写转换
来源：http://pa.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://al.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://hx.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://ae.nszjky.cn

[Q85] 数值取整
来源：http://li.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iq.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://tx.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ku.colortex.cn

[Q87] JSON 字段做条件
来源：http://tz.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ow.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://tp.muxihuayi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zy.szsharing.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fz.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://um.panjiajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ve.muxihuayi.cn

[Q90] 生成序号列
来源：http://on.9csxet.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qg.wgjwhj.cn

================================================================================
来源：http://ai.panjiajie.cn

R. Bash 专题
来源：http://yt.bookmarksfly.cn

================================================================================
来源：http://zy.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ml.bookmarksfly.cn

#!/usr/bin/env bash
来源：http://jb.shtwfgs.cn

set -euo pipefail
来源：http://lj.hahajie.cn

[R02] 变量赋值与使用
来源：http://tt.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://rq.huanxung.cn

[R03] 只读变量
来源：http://gf.haigaiapp.cn

readonly PI=3.14
来源：http://mg.yuexingan06.cn

[R04] 位置参数
来源：http://za.521024.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wp.nicolike.cn

[R05] 参数默认值
来源：http://xz.muxihuayi.cn

name="${1:-default}"
来源：http://qg.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://at.hnjuh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ls.yuntaijiaju.cn

[R07] if 判断文件
来源：http://rm.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gh.bjjhwx.cn

[R08] 数值比较
来源：http://tt.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lk.hnjuh.cn

[R09] 字符串比较
来源：http://mh.muxihuayi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jl.szsharing.cn

[R10] 正则匹配
来源：http://xn.jctech888.com.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kd.521024.cn

[R11] case 多分支
来源：http://me.huixinmuqiang.cn

case "$1" in
来源：http://au.bookmarksfly.cn

start) echo "启动" ;;
来源：http://je.521024.cn

stop)  echo "停止" ;;
来源：http://jg.521024.cn

*)     echo "未知命令" ;;
来源：http://nf.newstarts.cn

esac
来源：http://lf.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://iz.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://dm.bjjhwx.cn

[R13] for 计数循环
来源：http://ne.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://dz.lnxyls.cn

[R14] C 风格 for
来源：http://cs.hahajie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zv.9csxet.cn

[R15] while 逐行读文件
来源：http://uf.huixiangedu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ho.huixinmuqiang.cn

[R16] until 等待条件
来源：http://rh.shxzukj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://at.shxzskj.cn

[R17] 数组定义与取值
来源：http://ec.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kn.muxihuayi.cn

[R18] 遍历数组
来源：http://sd.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kd.colortex.cn

[R19] 数组长度
来源：http://eb.hahajie.cn

echo "${#arr[@]}"
来源：http://zw.lnxyls.cn

[R20] 关联数组（字典）
来源：http://zx.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qw.nszjky.cn

[R21] 字符串长度
来源：http://cy.nszjky.cn

echo "${#s}"
来源：http://wg.gzmigu.cn

[R22] 截取子串
来源：http://cg.gzmigu.cn

echo "${s:0:5}"
来源：http://ru.shxzskj.cn

[R23] 字符串替换
来源：http://zx.yuntaijiaju.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yu.shxzskj.cn

[R24] 大小写转换
来源：http://hz.hahajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ag.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://tk.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gx.jianghongdianzi.cn

[R26] 命令替换
来源：http://ot.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://gr.shxzukj.cn

[R27] 算术展开
来源：http://ki.nszjky.cn

echo $((1 + 2 * 3))
来源：http://ob.hahajie.cn

[R28] 浮点运算
来源：http://me.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://cc.gzmigu.cn

[R29] 定义函数
来源：http://pl.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yz.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://pn.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://iw.gzmigu.cn

[R31] 局部变量
来源：http://co.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://lb.colortex.cn

[R32] 参数个数校验
来源：http://jo.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jy.nicolike.cn

[R33] 捕获错误并提示行号
来源：http://jl.shxzukj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bq.huixinmuqiang.cn

[R34] 退出时清理
来源：http://qg.hahajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://py.shxzukj.cn

[R35] 后台执行并等待
来源：http://mc.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pd.colortex.cn

[R36] 并发执行多个任务
来源：http://vr.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sj.nszjky.cn

[R37] 把输出赋给变量
来源：http://kf.huanxung.cn

files=$(ls -1)
来源：http://rm.huixinmuqiang.cn

[R38] 管道串联
来源：http://uy.yuexingan06.cn

cat a.txt | grep -i error | wc -l
来源：http://gx.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://dw.hahajie.cn

cmd > out.log 2>&1
来源：http://dm.yuexingan06.cn

[R40] 追加写日志
来源：http://xg.9csxet.cn

echo "log" >> out.log
来源：http://go.nicolike.cn

[R41] 丢弃输出
来源：http://bn.bookmarksfly.cn

cmd >/dev/null 2>&1
来源：http://jw.asd995.cn

[R42] 输入重定向
来源：http://pp.jianghongdianzi.cn

wc -l < a.txt
来源：http://ns.bjjhwx.cn

[R43] 按名字查找文件
来源：http://bf.lnxyls.cn

find . -name "*.log" -type f
来源：http://md.shtwfgs.cn

[R44] 按修改时间查找
来源：http://jn.asd995.cn

find . -mtime -7 -type f
来源：http://iq.chemitech.net.cn

[R45] 批量删除
来源：http://hm.hahajie.cn

find . -name "*.tmp" -delete
来源：http://hn.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://ta.huixinmuqiang.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://js.shxzukj.cn

[R47] sed 单行替换
来源：http://ab.colortex.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ei.shxzskj.cn

[R48] awk 取指定列
来源：http://hv.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://fx.yuntaijiaju.cn

[R49] awk 带条件
来源：http://wi.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ce.shtwfgs.cn

[R50] awk 求和
来源：http://be.shxzskj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mf.szsharing.cn

[R51] 排序去重取前几
来源：http://an.bjjhwx.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ai.jctech888.com.cn

[R52] 统计行数
来源：http://rm.asd995.cn

wc -l a.txt
来源：http://ft.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://ey.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rn.shxzskj.cn

[R54] 比较两个文件
来源：http://mi.huixinmuqiang.cn

diff a.txt b.txt
来源：http://vc.szxytkj.cn

[R55] 压缩与解压
来源：http://ry.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tl.newstarts.cn

[R56] 远程拷贝
来源：http://pi.lnxyls.cn

scp file user@host:/path/
来源：http://yc.haigaiapp.cn

[R57] 远程执行命令
来源：http://lp.chemitech.net.cn

ssh user@host 'uptime'
来源：http://xh.shxzskj.cn

[R58] 下载文件
来源：http://wa.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vt.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://oc.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pi.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://xh.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://da.szxytkj.cn

[R61] 磁盘占用
来源：http://ys.yuntaijiaju.cn

df -h;  du -sh *
来源：http://mq.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://qd.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://xt.asd995.cn

[R63] 内存与进程
来源：http://xi.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://li.nszjky.cn

[R64] 结束进程
来源：http://ed.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://iv.shxzskj.cn

[R65] 查看端口占用
来源：http://iw.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eo.wgjwhj.cn

[R66] 定时任务
来源：http://li.nszjky.cn

crontab -e;  crontab -l
来源：http://on.colortex.cn

[R67] 生成随机十六进制串
来源：http://my.wgjwhj.cn

openssl rand -hex 16
来源：http://il.lnxyls.cn

[R68] 计算文件校验值
来源：http://wv.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dk.colortex.cn

[R69] 生成随机密码
来源：http://am.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://il.huanxung.cn

[R70] 时间戳与互转
来源：http://qj.colortex.cn

date +%s;  date -d @1700000000
来源：http://ti.muxihuayi.cn

[R71] 日期格式化
来源：http://jy.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hx.521024.cn

[R72] 等待端口就绪
来源：http://tw.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cc.shtwfgs.cn

[R73] 分割大日志
来源：http://va.shxzukj.cn

split -l 1000 big.log part_
来源：http://cf.nicolike.cn

[R74] 批量重命名
来源：http://yq.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ql.wgjwhj.cn

[R75] 导出环境变量
来源：http://bt.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ew.lnxyls.cn

[R76] 使用临时文件
来源：http://uo.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mt.hnjuh.cn

[R77] 读取用户输入
来源：http://bn.jctech888.com.cn

read -rp "请输入: " ans
来源：http://ex.szxytkj.cn

[R78] 交互式菜单
来源：http://km.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pg.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://bv.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cv.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ut.shtwfgs.cn

time ./run.sh
来源：http://om.nszjky.cn

================================================================================
来源：http://yf.huanxung.cn

S. C / C++ 专题
来源：http://vx.newstarts.cn

================================================================================
来源：http://mn.shtwfgs.cn

[S01] C：Hello World
来源：http://uh.hahajie.cn

#include <stdio.h>
来源：http://oz.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wu.nszjky.cn

[S02] C：变量与格式化输出
来源：http://wf.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://wd.521024.cn

[S03] C：读入整数
来源：http://aq.szsharing.cn

int x; scanf("%d", &x);
来源：http://jv.asd995.cn

[S04] C：字符串复制
来源：http://lq.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rz.bookmarksfly.cn

[S05] C：字符串长度
来源：http://ld.jctech888.com.cn

strlen(s)
来源：http://vf.asd995.cn

[S06] C：字符串比较
来源：http://fk.wgjwhj.cn

strcmp(a, b) == 0
来源：http://cf.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://sn.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dd.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://lh.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bn.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://jo.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hq.hahajie.cn

[S10] C：指针与解引用
来源：http://fe.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://dc.yuexingan06.cn

[S11] C：逐行读文件
来源：http://zt.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://vw.newstarts.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ox.wgjwhj.cn

fclose(f);
来源：http://hi.shtwfgs.cn

[S12] C：写文件
来源：http://gf.yuexingan06.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zq.wgjwhj.cn

[S13] C：宏定义
来源：http://xz.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mv.muxihuayi.cn

[S14] C：枚举
来源：http://jt.huanxung.cn

enum Color { RED, GREEN, BLUE };
来源：http://vu.huixinmuqiang.cn

[S15] C：类型转换
来源：http://id.wgjwhj.cn

(double) a / b
来源：http://rn.newstarts.cn

[S16] C：位操作置位
来源：http://kj.panjiajie.cn

x |= (1 << 3);
来源：http://lt.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://cw.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pv.colortex.cn

[S18] C：命令行参数
来源：http://lf.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://me.panjiajie.cn

[S19] C：快速排序
来源：http://an.newstarts.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rw.bjjhwx.cn

[S20] C：二分查找
来源：http://sx.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ua.szsharing.cn

[S21] C：字符类别判断
来源：http://ux.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sd.bjjhwx.cn

[S22] C：字符串转数字
来源：http://wb.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dc.colortex.cn

[S23] C：随机数
来源：http://kn.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wv.gzmigu.cn

[S24] C：获取本地时间
来源：http://sf.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eq.huanxung.cn

[S25] C：内存拷贝
来源：http://ub.521024.cn

memcpy(dst, src, n);
来源：http://io.hnjuh.cn

[S26] C：内存清零
来源：http://hg.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://qw.gzmigu.cn

[S27] C：定义常量
来源：http://xf.szsharing.cn

const double PI = 3.14159;
来源：http://qt.huanxung.cn

[S28] C：静态变量
来源：http://fq.colortex.cn

static int counter = 0;
来源：http://ha.shxzukj.cn

[S29] C：变参函数
来源：http://ij.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qn.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://sq.muxihuayi.cn

#ifndef X_H
来源：http://bu.hahajie.cn

#define X_H
来源：http://xm.huanxung.cn

#endif
来源：http://hv.nicolike.cn

[S31] C++：Hello World
来源：http://sv.hnjuh.cn

#include <iostream>
来源：http://re.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://tj.jctech888.com.cn

[S32] C++：字符串
来源：http://ss.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ni.haigaiapp.cn

[S33] C++：vector 增删
来源：http://gg.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cb.nicolike.cn

[S34] C++：遍历 vector
来源：http://rh.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://cq.muxihuayi.cn

[S35] C++：map
来源：http://lr.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jp.muxihuayi.cn

[S36] C++：unordered_map
来源：http://kh.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zx.muxihuayi.cn

[S37] C++：set
来源：http://ze.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nn.shxzukj.cn

[S38] C++：排序
来源：http://ak.colortex.cn

std::sort(v.begin(), v.end());
来源：http://he.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://tv.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mm.chemitech.net.cn

[S40] C++：查找元素
来源：http://vk.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ge.huixiangedu.cn


<!-- 参考信息 -->