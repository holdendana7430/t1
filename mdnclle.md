代发 wailian999

ANALYZE TABLE users;
来源：http://my.huixiangedu.cn

[Q71] 查看建表语句
来源：http://ui.nicolike.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ob.asd995.cn

[Q72] 查看索引
来源：http://ca.asd995.cn

SHOW INDEX FROM users;
来源：http://rh.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://bs.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rt.shxzskj.cn

[Q74] 强制使用索引
来源：http://is.yuexingan06.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jy.szxytkj.cn

[Q75] 日期格式化
来源：http://ug.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xn.wgjwhj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fy.hnjuh.cn

[Q76] 按天统计
来源：http://of.nicolike.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jh.szxytkj.cn

[Q77] 时间加减
来源：http://ce.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kl.yuexingan06.cn

[Q78] 当前时间
来源：http://jl.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ss.newstarts.cn

[Q79] 字符串拼接
来源：http://mo.shtwfgs.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://te.asd995.cn

[Q80] 字符串截取
来源：http://ug.szxytkj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://op.9csxet.cn

[Q81] 字符串替换
来源：http://ln.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lc.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://mh.panjiajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eg.wgjwhj.cn

[Q83] 大小写转换
来源：http://fx.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://go.haigaiapp.cn

[Q84] 去除首尾空格
来源：http://td.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ke.nicolike.cn

[Q85] 数值取整
来源：http://vk.colortex.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wj.szsharing.cn

[Q86] 读取 JSON 字段
来源：http://nj.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vd.huanxung.cn

[Q87] JSON 字段做条件
来源：http://qa.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sh.yuntaijiaju.cn

[Q88] 行转列（条件聚合）
来源：http://jj.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jr.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rm.nicolike.cn

[Q89] 判断表是否存在
来源：http://dk.yuntaijiaju.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ge.panjiajie.cn

[Q90] 生成序号列
来源：http://bm.lnxyls.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ev.yuntaijiaju.cn

================================================================================
来源：http://tl.gzmigu.cn

R. Bash 专题
来源：http://iq.shxzukj.cn

================================================================================
来源：http://cr.bookmarksfly.cn

[R01] shebang 与严格模式
来源：http://sh.lnxyls.cn

#!/usr/bin/env bash
来源：http://nm.521024.cn

set -euo pipefail
来源：http://cu.521024.cn

[R02] 变量赋值与使用
来源：http://dv.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://xx.521024.cn

[R03] 只读变量
来源：http://wl.asd995.cn

readonly PI=3.14
来源：http://zg.newstarts.cn

[R04] 位置参数
来源：http://bg.yuexingan06.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gf.nicolike.cn

[R05] 参数默认值
来源：http://wj.yuexingan06.cn

name="${1:-default}"
来源：http://ip.szsharing.cn

[R06] 判断命令是否存在
来源：http://lu.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tz.shtwfgs.cn

[R07] if 判断文件
来源：http://qr.asd995.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gv.huixiangedu.cn

[R08] 数值比较
来源：http://sm.shxzskj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ut.panjiajie.cn

[R09] 字符串比较
来源：http://oe.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://np.asd995.cn

[R10] 正则匹配
来源：http://lr.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ac.colortex.cn

[R11] case 多分支
来源：http://kr.lnxyls.cn

case "$1" in
来源：http://mp.wgjwhj.cn

start) echo "启动" ;;
来源：http://jg.gzmigu.cn

stop)  echo "停止" ;;
来源：http://ae.521024.cn

*)     echo "未知命令" ;;
来源：http://um.gzmigu.cn

esac
来源：http://rz.521024.cn

[R12] for 遍历文件
来源：http://pb.gzmigu.cn

for f in *.txt; do echo "$f"; done
来源：http://pc.huixiangedu.cn

[R13] for 计数循环
来源：http://hj.huanxung.cn

for i in {1..10}; do echo "$i"; done
来源：http://xo.yuexingan06.cn

[R14] C 风格 for
来源：http://pb.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gs.colortex.cn

[R15] while 逐行读文件
来源：http://ik.colortex.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cw.yuexingan06.cn

[R16] until 等待条件
来源：http://hy.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hd.nicolike.cn

[R17] 数组定义与取值
来源：http://mb.yuexingan06.cn

arr=(a b c); echo "${arr[0]}"
来源：http://js.newstarts.cn

[R18] 遍历数组
来源：http://qn.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ak.huanxung.cn

[R19] 数组长度
来源：http://rm.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://mh.szsharing.cn

[R20] 关联数组（字典）
来源：http://sl.shxzskj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ec.chemitech.net.cn

[R21] 字符串长度
来源：http://to.chemitech.net.cn

echo "${#s}"
来源：http://cf.huixiangedu.cn

[R22] 截取子串
来源：http://vn.shxzukj.cn

echo "${s:0:5}"
来源：http://sd.jctech888.com.cn

[R23] 字符串替换
来源：http://of.jianghongdianzi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cd.bookmarksfly.cn

[R24] 大小写转换
来源：http://fl.huixiangedu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iw.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://bq.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hl.asd995.cn

[R26] 命令替换
来源：http://xg.gzmigu.cn

now=$(date +%F); echo "$now"
来源：http://on.9csxet.cn

[R27] 算术展开
来源：http://yf.huanxung.cn

echo $((1 + 2 * 3))
来源：http://vr.huixiangedu.cn

[R28] 浮点运算
来源：http://mj.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://yo.huixiangedu.cn

[R29] 定义函数
来源：http://yy.lnxyls.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tb.huixiangedu.cn

[R30] 函数返回状态码
来源：http://ys.muxihuayi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ot.lnxyls.cn

[R31] 局部变量
来源：http://ov.lnxyls.cn

f() { local x=1; echo "$x"; }
来源：http://ov.yuexingan06.cn

[R32] 参数个数校验
来源：http://vi.huanxung.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qi.shtwfgs.cn

[R33] 捕获错误并提示行号
来源：http://ym.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hh.gzmigu.cn

[R34] 退出时清理
来源：http://ej.yuntaijiaju.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rd.yuexingan06.cn

[R35] 后台执行并等待
来源：http://yp.nicolike.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ya.panjiajie.cn

[R36] 并发执行多个任务
来源：http://jx.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gv.chemitech.net.cn

[R37] 把输出赋给变量
来源：http://as.szsharing.cn

files=$(ls -1)
来源：http://ht.szsharing.cn

[R38] 管道串联
来源：http://sl.hahajie.cn

cat a.txt | grep -i error | wc -l
来源：http://ow.9csxet.cn

[R39] 重定向标准输出与错误
来源：http://qp.shxzskj.cn

cmd > out.log 2>&1
来源：http://er.huanxung.cn

[R40] 追加写日志
来源：http://zn.szxytkj.cn

echo "log" >> out.log
来源：http://pk.jianghongdianzi.cn

[R41] 丢弃输出
来源：http://kh.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://nd.lnxyls.cn

[R42] 输入重定向
来源：http://ce.szsharing.cn

wc -l < a.txt
来源：http://az.huixinmuqiang.cn

[R43] 按名字查找文件
来源：http://jc.yuntaijiaju.cn

find . -name "*.log" -type f
来源：http://go.bjjhwx.cn

[R44] 按修改时间查找
来源：http://hr.jctech888.com.cn

find . -mtime -7 -type f
来源：http://cm.huixinmuqiang.cn

[R45] 批量删除
来源：http://lw.yuexingan06.cn

find . -name "*.tmp" -delete
来源：http://ci.shtwfgs.cn

[R46] 递归替换文件内容
来源：http://uy.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hi.asd995.cn

[R47] sed 单行替换
来源：http://vw.szsharing.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fe.wgjwhj.cn

[R48] awk 取指定列
来源：http://tz.bjjhwx.cn

awk '{print $1, $3}' a.txt
来源：http://my.colortex.cn

[R49] awk 带条件
来源：http://ln.haigaiapp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iu.gzmigu.cn

[R50] awk 求和
来源：http://gu.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://og.521024.cn

[R51] 排序去重取前几
来源：http://kd.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fk.muxihuayi.cn

[R52] 统计行数
来源：http://xr.huixinmuqiang.cn

wc -l a.txt
来源：http://an.asd995.cn

[R53] 查看文件头与实时尾
来源：http://kg.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ms.yuexingan06.cn

[R54] 比较两个文件
来源：http://kw.huixinmuqiang.cn

diff a.txt b.txt
来源：http://zj.huanxung.cn

[R55] 压缩与解压
来源：http://fc.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wt.muxihuayi.cn

[R56] 远程拷贝
来源：http://pd.muxihuayi.cn

scp file user@host:/path/
来源：http://dt.shxzskj.cn

[R57] 远程执行命令
来源：http://lo.chemitech.net.cn

ssh user@host 'uptime'
来源：http://sv.hnjuh.cn

[R58] 下载文件
来源：http://qr.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tq.nicolike.cn

[R59] 发 POST JSON
来源：http://tg.521024.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gh.panjiajie.cn

[R60] 只看 HTTP 状态码
来源：http://rv.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ta.hahajie.cn

[R61] 磁盘占用
来源：http://if.shxzskj.cn

df -h;  du -sh *
来源：http://oj.newstarts.cn

[R62] 找最占空间的文件
来源：http://ry.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ry.9csxet.cn

[R63] 内存与进程
来源：http://zz.asd995.cn

free -h;  ps aux | grep nginx
来源：http://ux.panjiajie.cn

[R64] 结束进程
来源：http://ny.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://xm.muxihuayi.cn

[R65] 查看端口占用
来源：http://un.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oi.jctech888.com.cn

[R66] 定时任务
来源：http://gq.haigaiapp.cn

crontab -e;  crontab -l
来源：http://gb.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://ki.521024.cn

openssl rand -hex 16
来源：http://ke.521024.cn

[R68] 计算文件校验值
来源：http://vp.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tf.asd995.cn

[R69] 生成随机密码
来源：http://ps.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://ia.nszjky.cn

[R70] 时间戳与互转
来源：http://ug.huixiangedu.cn

date +%s;  date -d @1700000000
来源：http://lh.huixiangedu.cn

[R71] 日期格式化
来源：http://kz.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zz.jianghongdianzi.cn

[R72] 等待端口就绪
来源：http://cp.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zr.muxihuayi.cn

[R73] 分割大日志
来源：http://tc.huixiangedu.cn

split -l 1000 big.log part_
来源：http://og.bjjhwx.cn

[R74] 批量重命名
来源：http://to.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nv.huixiangedu.cn

[R75] 导出环境变量
来源：http://sm.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://xo.asd995.cn

[R76] 使用临时文件
来源：http://vi.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xh.hnjuh.cn

[R77] 读取用户输入
来源：http://sn.shxzskj.cn

read -rp "请输入: " ans
来源：http://qw.wgjwhj.cn

[R78] 交互式菜单
来源：http://pb.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bh.shxzskj.cn

[R79] 解析命令行选项
来源：http://cr.hahajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://me.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://zz.muxihuayi.cn

time ./run.sh
来源：http://he.panjiajie.cn

================================================================================
来源：http://wq.jianghongdianzi.cn

S. C / C++ 专题
来源：http://sx.bjjhwx.cn

================================================================================
来源：http://jk.nicolike.cn

[S01] C：Hello World
来源：http://sn.9csxet.cn

#include <stdio.h>
来源：http://zi.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kw.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ys.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://yq.huixinmuqiang.cn

[S03] C：读入整数
来源：http://zf.521024.cn

int x; scanf("%d", &x);
来源：http://qg.lnxyls.cn

[S04] C：字符串复制
来源：http://mp.hnjuh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://se.gzmigu.cn

[S05] C：字符串长度
来源：http://ek.shtwfgs.cn

strlen(s)
来源：http://jn.bookmarksfly.cn

[S06] C：字符串比较
来源：http://gy.yuntaijiaju.cn

strcmp(a, b) == 0
来源：http://yk.huanxung.cn

[S07] C：数组遍历求和
来源：http://hd.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zm.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://ui.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zj.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://hv.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yn.bjjhwx.cn

[S10] C：指针与解引用
来源：http://nv.huixinmuqiang.cn

int *p = &a;  *p = 5;
来源：http://gk.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://zx.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://yv.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sv.haigaiapp.cn

fclose(f);
来源：http://qq.asd995.cn

[S12] C：写文件
来源：http://ja.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pk.nszjky.cn

[S13] C：宏定义
来源：http://qy.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bh.bjjhwx.cn

[S14] C：枚举
来源：http://to.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ki.hnjuh.cn

[S15] C：类型转换
来源：http://sb.huixinmuqiang.cn

(double) a / b
来源：http://jp.hnjuh.cn

[S16] C：位操作置位
来源：http://ck.521024.cn

x |= (1 << 3);
来源：http://wl.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://rx.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pw.huixinmuqiang.cn

[S18] C：命令行参数
来源：http://th.shxzukj.cn

int main(int argc, char **argv)
来源：http://sm.panjiajie.cn

[S19] C：快速排序
来源：http://wx.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ww.bookmarksfly.cn

[S20] C：二分查找
来源：http://el.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jk.wgjwhj.cn

[S21] C：字符类别判断
来源：http://er.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fg.9csxet.cn

[S22] C：字符串转数字
来源：http://dk.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zz.bjjhwx.cn

[S23] C：随机数
来源：http://id.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qo.shxzukj.cn

[S24] C：获取本地时间
来源：http://bo.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hc.huanxung.cn

[S25] C：内存拷贝
来源：http://fb.hahajie.cn

memcpy(dst, src, n);
来源：http://rt.yuexingan06.cn

[S26] C：内存清零
来源：http://xa.asd995.cn

memset(a, 0, sizeof a);
来源：http://dp.nicolike.cn

[S27] C：定义常量
来源：http://so.bjjhwx.cn

const double PI = 3.14159;
来源：http://ei.521024.cn

[S28] C：静态变量
来源：http://dz.bjjhwx.cn

static int counter = 0;
来源：http://nt.szxytkj.cn

[S29] C：变参函数
来源：http://sv.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fc.9csxet.cn

[S30] C：头文件保护
来源：http://kb.huanxung.cn

#ifndef X_H
来源：http://jc.shtwfgs.cn

#define X_H
来源：http://zy.nicolike.cn

#endif
来源：http://wl.haigaiapp.cn

[S31] C++：Hello World
来源：http://ob.huixinmuqiang.cn

#include <iostream>
来源：http://qx.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://zx.asd995.cn

[S32] C++：字符串
来源：http://fk.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://kt.colortex.cn

[S33] C++：vector 增删
来源：http://vf.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nx.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://fl.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://os.hahajie.cn

[S35] C++：map
来源：http://et.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nk.muxihuayi.cn

[S36] C++：unordered_map
来源：http://hz.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vp.bookmarksfly.cn

[S37] C++：set
来源：http://mr.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ll.bookmarksfly.cn

[S38] C++：排序
来源：http://nr.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://qi.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://nu.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kl.shtwfgs.cn

[S40] C++：查找元素
来源：http://zd.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bo.jianghongdianzi.cn


<!-- 参考信息 -->