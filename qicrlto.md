代发 wailian999

ROLLBACK TO sp1;
来源：http://sg.huixinmuqiang.cn

[Q69] 查看执行计划
来源：http://gk.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bp.huixinmuqiang.cn

[Q70] 更新统计信息
来源：http://na.muxihuayi.cn

ANALYZE TABLE users;
来源：http://gi.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://nb.shxzukj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ct.huixinmuqiang.cn

[Q72] 查看索引
来源：http://bg.shtwfgs.cn

SHOW INDEX FROM users;
来源：http://gb.szsharing.cn

[Q73] 查看表状态
来源：http://nq.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bp.huixinmuqiang.cn

[Q74] 强制使用索引
来源：http://tz.nicolike.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bo.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://zw.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://js.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qb.wgjwhj.cn

[Q76] 按天统计
来源：http://lg.gzmigu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nx.yuntaijiaju.cn

[Q77] 时间加减
来源：http://yg.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mc.muxihuayi.cn

[Q78] 当前时间
来源：http://rp.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://er.jctech888.com.cn

[Q79] 字符串拼接
来源：http://hs.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gs.gzmigu.cn

[Q80] 字符串截取
来源：http://ol.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://za.colortex.cn

[Q81] 字符串替换
来源：http://aa.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://we.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://wu.bjjhwx.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://db.haigaiapp.cn

[Q83] 大小写转换
来源：http://oi.szxytkj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ct.shxzskj.cn

[Q84] 去除首尾空格
来源：http://qy.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://yx.szxytkj.cn

[Q85] 数值取整
来源：http://qq.jianghongdianzi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wm.muxihuayi.cn

[Q86] 读取 JSON 字段
来源：http://aw.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bi.bookmarksfly.cn

[Q87] JSON 字段做条件
来源：http://vu.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fc.shtwfgs.cn

[Q88] 行转列（条件聚合）
来源：http://wy.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uc.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ic.jctech888.com.cn

[Q89] 判断表是否存在
来源：http://zm.9csxet.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hx.yuexingan06.cn

[Q90] 生成序号列
来源：http://vf.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ss.szxytkj.cn

================================================================================
来源：http://yz.gzmigu.cn

R. Bash 专题
来源：http://hp.huixinmuqiang.cn

================================================================================
来源：http://qy.szsharing.cn

[R01] shebang 与严格模式
来源：http://er.szsharing.cn

#!/usr/bin/env bash
来源：http://wn.muxihuayi.cn

set -euo pipefail
来源：http://ew.szsharing.cn

[R02] 变量赋值与使用
来源：http://up.yuntaijiaju.cn

name="Tom"; echo "$name"
来源：http://jw.bjjhwx.cn

[R03] 只读变量
来源：http://qx.asd995.cn

readonly PI=3.14
来源：http://gp.panjiajie.cn

[R04] 位置参数
来源：http://oa.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://um.szxytkj.cn

[R05] 参数默认值
来源：http://xf.bjjhwx.cn

name="${1:-default}"
来源：http://gv.gzmigu.cn

[R06] 判断命令是否存在
来源：http://if.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bf.wgjwhj.cn

[R07] if 判断文件
来源：http://lh.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yn.yuexingan06.cn

[R08] 数值比较
来源：http://lt.521024.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dy.bjjhwx.cn

[R09] 字符串比较
来源：http://lm.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yh.colortex.cn

[R10] 正则匹配
来源：http://mz.huixinmuqiang.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://as.hnjuh.cn

[R11] case 多分支
来源：http://fa.szxytkj.cn

case "$1" in
来源：http://re.haigaiapp.cn

start) echo "启动" ;;
来源：http://xj.szsharing.cn

stop)  echo "停止" ;;
来源：http://rp.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://sp.huixinmuqiang.cn

esac
来源：http://qi.huixinmuqiang.cn

[R12] for 遍历文件
来源：http://jm.jctech888.com.cn

for f in *.txt; do echo "$f"; done
来源：http://ha.szsharing.cn

[R13] for 计数循环
来源：http://vd.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://db.nicolike.cn

[R14] C 风格 for
来源：http://wk.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wt.nszjky.cn

[R15] while 逐行读文件
来源：http://zo.9csxet.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gq.huanxung.cn

[R16] until 等待条件
来源：http://wu.nszjky.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ur.chemitech.net.cn

[R17] 数组定义与取值
来源：http://rw.nicolike.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dz.panjiajie.cn

[R18] 遍历数组
来源：http://pf.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ph.bookmarksfly.cn

[R19] 数组长度
来源：http://yo.huixiangedu.cn

echo "${#arr[@]}"
来源：http://mt.wgjwhj.cn

[R20] 关联数组（字典）
来源：http://os.chemitech.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://od.bookmarksfly.cn

[R21] 字符串长度
来源：http://wb.huanxung.cn

echo "${#s}"
来源：http://hc.shxzukj.cn

[R22] 截取子串
来源：http://rt.lnxyls.cn

echo "${s:0:5}"
来源：http://ch.szxytkj.cn

[R23] 字符串替换
来源：http://un.chemitech.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bb.hahajie.cn

[R24] 大小写转换
来源：http://dg.bjjhwx.cn

echo "${s^^}"; echo "${s,,}"
来源：http://in.hahajie.cn

[R25] 去后缀 / 去前缀
来源：http://yn.gzmigu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://av.521024.cn

[R26] 命令替换
来源：http://im.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://xb.panjiajie.cn

[R27] 算术展开
来源：http://di.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://vd.gzmigu.cn

[R28] 浮点运算
来源：http://tz.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://ml.huanxung.cn

[R29] 定义函数
来源：http://td.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pg.nicolike.cn

[R30] 函数返回状态码
来源：http://hr.huixiangedu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lo.huixinmuqiang.cn

[R31] 局部变量
来源：http://nf.shxzskj.cn

f() { local x=1; echo "$x"; }
来源：http://qh.colortex.cn

[R32] 参数个数校验
来源：http://jm.huixiangedu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xw.wgjwhj.cn

[R33] 捕获错误并提示行号
来源：http://lx.shxzskj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xt.huixinmuqiang.cn

[R34] 退出时清理
来源：http://cn.jctech888.com.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hj.jianghongdianzi.cn

[R35] 后台执行并等待
来源：http://wu.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sh.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://he.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nb.shxzukj.cn

[R37] 把输出赋给变量
来源：http://tj.szxytkj.cn

files=$(ls -1)
来源：http://ix.panjiajie.cn

[R38] 管道串联
来源：http://qs.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://sc.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ca.yuexingan06.cn

cmd > out.log 2>&1
来源：http://vv.panjiajie.cn

[R40] 追加写日志
来源：http://er.521024.cn

echo "log" >> out.log
来源：http://ol.nszjky.cn

[R41] 丢弃输出
来源：http://cz.asd995.cn

cmd >/dev/null 2>&1
来源：http://pn.jctech888.com.cn

[R42] 输入重定向
来源：http://cg.szxytkj.cn

wc -l < a.txt
来源：http://gs.jctech888.com.cn

[R43] 按名字查找文件
来源：http://vy.colortex.cn

find . -name "*.log" -type f
来源：http://bs.521024.cn

[R44] 按修改时间查找
来源：http://dk.asd995.cn

find . -mtime -7 -type f
来源：http://uc.gzmigu.cn

[R45] 批量删除
来源：http://zp.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://lx.shxzskj.cn

[R46] 递归替换文件内容
来源：http://bn.jianghongdianzi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tj.9csxet.cn

[R47] sed 单行替换
来源：http://fz.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gr.hnjuh.cn

[R48] awk 取指定列
来源：http://sz.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://rs.yuexingan06.cn

[R49] awk 带条件
来源：http://vu.gzmigu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wj.lnxyls.cn

[R50] awk 求和
来源：http://hn.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hp.yuntaijiaju.cn

[R51] 排序去重取前几
来源：http://vg.wgjwhj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mn.521024.cn

[R52] 统计行数
来源：http://ub.huanxung.cn

wc -l a.txt
来源：http://pf.9csxet.cn

[R53] 查看文件头与实时尾
来源：http://tv.huanxung.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://df.muxihuayi.cn

[R54] 比较两个文件
来源：http://qh.jianghongdianzi.cn

diff a.txt b.txt
来源：http://th.bookmarksfly.cn

[R55] 压缩与解压
来源：http://xg.shxzskj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bp.nszjky.cn

[R56] 远程拷贝
来源：http://yr.szxytkj.cn

scp file user@host:/path/
来源：http://iu.panjiajie.cn

[R57] 远程执行命令
来源：http://dt.bjjhwx.cn

ssh user@host 'uptime'
来源：http://vj.haigaiapp.cn

[R58] 下载文件
来源：http://zu.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vt.hnjuh.cn

[R59] 发 POST JSON
来源：http://yt.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xl.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://vv.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jr.huixiangedu.cn

[R61] 磁盘占用
来源：http://nl.wgjwhj.cn

df -h;  du -sh *
来源：http://nm.hnjuh.cn

[R62] 找最占空间的文件
来源：http://qq.521024.cn

du -ah . | sort -rh | head -10
来源：http://ly.yuntaijiaju.cn

[R63] 内存与进程
来源：http://fw.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://ac.szsharing.cn

[R64] 结束进程
来源：http://ko.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://jw.newstarts.cn

[R65] 查看端口占用
来源：http://yf.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yf.shtwfgs.cn

[R66] 定时任务
来源：http://fx.szxytkj.cn

crontab -e;  crontab -l
来源：http://rt.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://md.hnjuh.cn

openssl rand -hex 16
来源：http://db.wgjwhj.cn

[R68] 计算文件校验值
来源：http://il.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vk.nicolike.cn

[R69] 生成随机密码
来源：http://hi.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://ss.muxihuayi.cn

[R70] 时间戳与互转
来源：http://kx.szsharing.cn

date +%s;  date -d @1700000000
来源：http://nt.jianghongdianzi.cn

[R71] 日期格式化
来源：http://uz.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dy.chemitech.net.cn

[R72] 等待端口就绪
来源：http://ft.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zf.huixiangedu.cn

[R73] 分割大日志
来源：http://di.yuexingan06.cn

split -l 1000 big.log part_
来源：http://pn.muxihuayi.cn

[R74] 批量重命名
来源：http://as.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hq.newstarts.cn

[R75] 导出环境变量
来源：http://fm.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://oe.newstarts.cn

[R76] 使用临时文件
来源：http://cr.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ds.hahajie.cn

[R77] 读取用户输入
来源：http://oz.nszjky.cn

read -rp "请输入: " ans
来源：http://jp.huixiangedu.cn

[R78] 交互式菜单
来源：http://yn.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yw.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://kz.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yc.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://dc.yuexingan06.cn

time ./run.sh
来源：http://no.yuntaijiaju.cn

================================================================================
来源：http://ja.hnjuh.cn

S. C / C++ 专题
来源：http://jy.newstarts.cn

================================================================================
来源：http://ed.hnjuh.cn

[S01] C：Hello World
来源：http://nc.nicolike.cn

#include <stdio.h>
来源：http://vx.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wk.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://py.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://gi.jctech888.com.cn

[S03] C：读入整数
来源：http://sx.shxzukj.cn

int x; scanf("%d", &x);
来源：http://py.yuexingan06.cn

[S04] C：字符串复制
来源：http://ci.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jk.wgjwhj.cn

[S05] C：字符串长度
来源：http://ma.chemitech.net.cn

strlen(s)
来源：http://yu.colortex.cn

[S06] C：字符串比较
来源：http://nj.muxihuayi.cn

strcmp(a, b) == 0
来源：http://zc.panjiajie.cn

[S07] C：数组遍历求和
来源：http://nw.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ry.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://fo.nszjky.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://ou.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bk.huixiangedu.cn

[S10] C：指针与解引用
来源：http://yc.colortex.cn

int *p = &a;  *p = 5;
来源：http://ab.bjjhwx.cn

[S11] C：逐行读文件
来源：http://po.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://zg.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xk.521024.cn

fclose(f);
来源：http://sg.huixiangedu.cn

[S12] C：写文件
来源：http://jl.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mp.haigaiapp.cn

[S13] C：宏定义
来源：http://lq.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sm.szxytkj.cn

[S14] C：枚举
来源：http://mt.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://pc.shtwfgs.cn

[S15] C：类型转换
来源：http://fp.9csxet.cn

(double) a / b
来源：http://hc.521024.cn

[S16] C：位操作置位
来源：http://yf.gzmigu.cn

x |= (1 << 3);
来源：http://mp.asd995.cn

[S17] C：安全拼接字符串
来源：http://uh.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rm.lnxyls.cn

[S18] C：命令行参数
来源：http://kx.lnxyls.cn

int main(int argc, char **argv)
来源：http://sq.huixinmuqiang.cn

[S19] C：快速排序
来源：http://nj.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qa.521024.cn

[S20] C：二分查找
来源：http://hi.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jz.521024.cn

[S21] C：字符类别判断
来源：http://ul.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xr.shxzskj.cn

[S22] C：字符串转数字
来源：http://pb.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sg.muxihuayi.cn

[S23] C：随机数
来源：http://hx.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oi.asd995.cn

[S24] C：获取本地时间
来源：http://ll.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gq.huanxung.cn

[S25] C：内存拷贝
来源：http://cs.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://gd.9csxet.cn

[S26] C：内存清零
来源：http://yo.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://rq.chemitech.net.cn

[S27] C：定义常量
来源：http://mz.9csxet.cn

const double PI = 3.14159;
来源：http://nt.asd995.cn

[S28] C：静态变量
来源：http://vr.shxzukj.cn

static int counter = 0;
来源：http://dk.haigaiapp.cn

[S29] C：变参函数
来源：http://wz.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sn.9csxet.cn

[S30] C：头文件保护
来源：http://lm.hnjuh.cn

#ifndef X_H
来源：http://qy.newstarts.cn

#define X_H
来源：http://ku.yuntaijiaju.cn

#endif
来源：http://qq.newstarts.cn

[S31] C++：Hello World
来源：http://ae.szsharing.cn

#include <iostream>
来源：http://pi.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://kz.nicolike.cn

[S32] C++：字符串
来源：http://bh.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://tv.asd995.cn

[S33] C++：vector 增删
来源：http://eh.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wr.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://bq.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://kr.9csxet.cn

[S35] C++：map
来源：http://mv.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jb.jctech888.com.cn

[S36] C++：unordered_map
来源：http://aa.muxihuayi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wr.jianghongdianzi.cn

[S37] C++：set
来源：http://zp.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tf.hnjuh.cn

[S38] C++：排序
来源：http://mk.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://hm.gzmigu.cn


<!-- 参考信息 -->