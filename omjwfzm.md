代发 wailian999

[Q67] 设置隔离级别
来源：http://rp.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cu.shxzskj.cn

[Q68] 保存点
来源：http://ls.huixiangedu.cn

SAVEPOINT sp1;
来源：http://su.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://mt.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://ns.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ov.panjiajie.cn

[Q70] 更新统计信息
来源：http://sx.bjjhwx.cn

ANALYZE TABLE users;
来源：http://zx.asd995.cn

[Q71] 查看建表语句
来源：http://bh.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://am.bjjhwx.cn

[Q72] 查看索引
来源：http://ay.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://au.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://sr.chemitech.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oy.chemitech.net.cn

[Q74] 强制使用索引
来源：http://hi.colortex.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://no.huixinmuqiang.cn

[Q75] 日期格式化
来源：http://xy.bookmarksfly.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xo.huixiangedu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bh.nicolike.cn

[Q76] 按天统计
来源：http://il.hahajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wr.shxzskj.cn

[Q77] 时间加减
来源：http://vk.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vp.colortex.cn

[Q78] 当前时间
来源：http://xs.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lh.jctech888.com.cn

[Q79] 字符串拼接
来源：http://ma.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gv.bookmarksfly.cn

[Q80] 字符串截取
来源：http://it.bookmarksfly.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ft.lnxyls.cn

[Q81] 字符串替换
来源：http://ze.521024.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yw.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://cw.wgjwhj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sx.hahajie.cn

[Q83] 大小写转换
来源：http://fh.nicolike.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wc.muxihuayi.cn

[Q84] 去除首尾空格
来源：http://pv.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://tw.chemitech.net.cn

[Q85] 数值取整
来源：http://iz.jctech888.com.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://el.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://gz.hnjuh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rq.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://ds.shxzskj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ea.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://ga.chemitech.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ku.szxytkj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rm.shxzskj.cn

[Q89] 判断表是否存在
来源：http://iv.muxihuayi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qv.shtwfgs.cn

[Q90] 生成序号列
来源：http://ib.shxzskj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nw.nszjky.cn

================================================================================
来源：http://pk.haigaiapp.cn

R. Bash 专题
来源：http://qi.shtwfgs.cn

================================================================================
来源：http://jr.szsharing.cn

[R01] shebang 与严格模式
来源：http://ga.wgjwhj.cn

#!/usr/bin/env bash
来源：http://il.asd995.cn

set -euo pipefail
来源：http://vi.panjiajie.cn

[R02] 变量赋值与使用
来源：http://oh.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://oq.haigaiapp.cn

[R03] 只读变量
来源：http://wh.shxzskj.cn

readonly PI=3.14
来源：http://qn.nicolike.cn

[R04] 位置参数
来源：http://jn.shxzskj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ka.nszjky.cn

[R05] 参数默认值
来源：http://gx.yuexingan06.cn

name="${1:-default}"
来源：http://yc.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://xj.nicolike.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wp.huixiangedu.cn

[R07] if 判断文件
来源：http://mh.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qn.shxzskj.cn

[R08] 数值比较
来源：http://qg.hahajie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vk.9csxet.cn

[R09] 字符串比较
来源：http://xk.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wl.szxytkj.cn

[R10] 正则匹配
来源：http://pz.521024.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qn.jianghongdianzi.cn

[R11] case 多分支
来源：http://wc.bjjhwx.cn

case "$1" in
来源：http://lo.gzmigu.cn

start) echo "启动" ;;
来源：http://dc.colortex.cn

stop)  echo "停止" ;;
来源：http://gh.muxihuayi.cn

*)     echo "未知命令" ;;
来源：http://dq.muxihuayi.cn

esac
来源：http://gk.hahajie.cn

[R12] for 遍历文件
来源：http://ty.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://wx.521024.cn

[R13] for 计数循环
来源：http://ay.huixiangedu.cn

for i in {1..10}; do echo "$i"; done
来源：http://vw.colortex.cn

[R14] C 风格 for
来源：http://ps.hnjuh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xk.shxzskj.cn

[R15] while 逐行读文件
来源：http://pd.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xy.huanxung.cn

[R16] until 等待条件
来源：http://aq.muxihuayi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aj.yuexingan06.cn

[R17] 数组定义与取值
来源：http://ma.haigaiapp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iq.hahajie.cn

[R18] 遍历数组
来源：http://yj.jctech888.com.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jp.hnjuh.cn

[R19] 数组长度
来源：http://ce.asd995.cn

echo "${#arr[@]}"
来源：http://jt.hnjuh.cn

[R20] 关联数组（字典）
来源：http://td.haigaiapp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mr.panjiajie.cn

[R21] 字符串长度
来源：http://ch.521024.cn

echo "${#s}"
来源：http://xf.szsharing.cn

[R22] 截取子串
来源：http://dn.jctech888.com.cn

echo "${s:0:5}"
来源：http://gr.haigaiapp.cn

[R23] 字符串替换
来源：http://zc.lnxyls.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xt.gzmigu.cn

[R24] 大小写转换
来源：http://ia.shtwfgs.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tc.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://ri.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nq.shxzskj.cn

[R26] 命令替换
来源：http://sf.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://fq.lnxyls.cn

[R27] 算术展开
来源：http://zx.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://pl.huanxung.cn

[R28] 浮点运算
来源：http://bi.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://ar.szsharing.cn

[R29] 定义函数
来源：http://rb.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tk.huanxung.cn

[R30] 函数返回状态码
来源：http://os.shxzskj.cn

f() { return 0; }; f || echo "失败了"
来源：http://ij.gzmigu.cn

[R31] 局部变量
来源：http://ux.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://js.bookmarksfly.cn

[R32] 参数个数校验
来源：http://gp.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pj.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://sn.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qz.szxytkj.cn

[R34] 退出时清理
来源：http://sp.panjiajie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uw.nszjky.cn

[R35] 后台执行并等待
来源：http://eu.hnjuh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zt.gzmigu.cn

[R36] 并发执行多个任务
来源：http://xd.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xe.shtwfgs.cn

[R37] 把输出赋给变量
来源：http://bi.521024.cn

files=$(ls -1)
来源：http://wt.yuexingan06.cn

[R38] 管道串联
来源：http://ux.wgjwhj.cn

cat a.txt | grep -i error | wc -l
来源：http://az.szsharing.cn

[R39] 重定向标准输出与错误
来源：http://vd.yuexingan06.cn

cmd > out.log 2>&1
来源：http://at.yuexingan06.cn

[R40] 追加写日志
来源：http://xp.huanxung.cn

echo "log" >> out.log
来源：http://ns.lnxyls.cn

[R41] 丢弃输出
来源：http://pd.haigaiapp.cn

cmd >/dev/null 2>&1
来源：http://xe.lnxyls.cn

[R42] 输入重定向
来源：http://vp.hahajie.cn

wc -l < a.txt
来源：http://em.haigaiapp.cn

[R43] 按名字查找文件
来源：http://pm.wgjwhj.cn

find . -name "*.log" -type f
来源：http://hk.muxihuayi.cn

[R44] 按修改时间查找
来源：http://sg.muxihuayi.cn

find . -mtime -7 -type f
来源：http://bc.bookmarksfly.cn

[R45] 批量删除
来源：http://pf.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://jn.shxzukj.cn

[R46] 递归替换文件内容
来源：http://jv.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://et.yuntaijiaju.cn

[R47] sed 单行替换
来源：http://om.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://et.szxytkj.cn

[R48] awk 取指定列
来源：http://fs.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://on.bookmarksfly.cn

[R49] awk 带条件
来源：http://vt.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uk.hahajie.cn

[R50] awk 求和
来源：http://fu.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aa.gzmigu.cn

[R51] 排序去重取前几
来源：http://ms.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghongdianzi.cn

[R52] 统计行数
来源：http://pg.hahajie.cn

wc -l a.txt
来源：http://zc.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://ph.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sy.lnxyls.cn

[R54] 比较两个文件
来源：http://vg.haigaiapp.cn

diff a.txt b.txt
来源：http://nu.hahajie.cn

[R55] 压缩与解压
来源：http://ku.gzmigu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fz.bjjhwx.cn

[R56] 远程拷贝
来源：http://ts.wgjwhj.cn

scp file user@host:/path/
来源：http://rm.colortex.cn

[R57] 远程执行命令
来源：http://cj.szxytkj.cn

ssh user@host 'uptime'
来源：http://tu.bjjhwx.cn

[R58] 下载文件
来源：http://mr.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ky.huanxung.cn

[R59] 发 POST JSON
来源：http://tf.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zd.colortex.cn

[R60] 只看 HTTP 状态码
来源：http://oz.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hh.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://xb.muxihuayi.cn

df -h;  du -sh *
来源：http://zv.asd995.cn

[R62] 找最占空间的文件
来源：http://xm.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://sb.lnxyls.cn

[R63] 内存与进程
来源：http://ya.521024.cn

free -h;  ps aux | grep nginx
来源：http://nd.chemitech.net.cn

[R64] 结束进程
来源：http://qj.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://xd.nicolike.cn

[R65] 查看端口占用
来源：http://cj.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nn.nicolike.cn

[R66] 定时任务
来源：http://sg.wgjwhj.cn

crontab -e;  crontab -l
来源：http://mi.huixinmuqiang.cn

[R67] 生成随机十六进制串
来源：http://ou.panjiajie.cn

openssl rand -hex 16
来源：http://rp.newstarts.cn

[R68] 计算文件校验值
来源：http://yp.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sq.chemitech.net.cn

[R69] 生成随机密码
来源：http://dc.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://nf.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ot.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://ew.haigaiapp.cn

[R71] 日期格式化
来源：http://ji.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mw.szxytkj.cn

[R72] 等待端口就绪
来源：http://pw.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ig.huixinmuqiang.cn

[R73] 分割大日志
来源：http://py.szxytkj.cn

split -l 1000 big.log part_
来源：http://sc.shtwfgs.cn

[R74] 批量重命名
来源：http://qr.lnxyls.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gh.shtwfgs.cn

[R75] 导出环境变量
来源：http://hc.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://yx.muxihuayi.cn

[R76] 使用临时文件
来源：http://dt.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rt.hahajie.cn

[R77] 读取用户输入
来源：http://ut.9csxet.cn

read -rp "请输入: " ans
来源：http://gj.shtwfgs.cn

[R78] 交互式菜单
来源：http://ax.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tb.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://ru.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://jh.hnjuh.cn

time ./run.sh
来源：http://vu.521024.cn

================================================================================
来源：http://yl.haigaiapp.cn

S. C / C++ 专题
来源：http://dy.chemitech.net.cn

================================================================================
来源：http://yd.haigaiapp.cn

[S01] C：Hello World
来源：http://nu.bjjhwx.cn

#include <stdio.h>
来源：http://ks.szsharing.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hy.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://ga.521024.cn

int a = 10; printf("%d\n", a);
来源：http://fh.yuntaijiaju.cn

[S03] C：读入整数
来源：http://if.colortex.cn

int x; scanf("%d", &x);
来源：http://ey.asd995.cn

[S04] C：字符串复制
来源：http://yf.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uf.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://lj.huanxung.cn

strlen(s)
来源：http://pg.bjjhwx.cn

[S06] C：字符串比较
来源：http://bx.szsharing.cn

strcmp(a, b) == 0
来源：http://re.colortex.cn

[S07] C：数组遍历求和
来源：http://qu.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dv.asd995.cn

[S08] C：动态内存分配与释放
来源：http://kf.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xp.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://uu.asd995.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ka.9csxet.cn

[S10] C：指针与解引用
来源：http://kn.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://bo.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://rj.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ea.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zn.newstarts.cn

fclose(f);
来源：http://jn.yuntaijiaju.cn

[S12] C：写文件
来源：http://mc.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xe.newstarts.cn

[S13] C：宏定义
来源：http://jb.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ly.haigaiapp.cn

[S14] C：枚举
来源：http://qc.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://nl.bookmarksfly.cn

[S15] C：类型转换
来源：http://wq.hahajie.cn

(double) a / b
来源：http://qr.chemitech.net.cn

[S16] C：位操作置位
来源：http://jn.jctech888.com.cn

x |= (1 << 3);
来源：http://av.huanxung.cn

[S17] C：安全拼接字符串
来源：http://kx.panjiajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://di.lnxyls.cn

[S18] C：命令行参数
来源：http://lk.nszjky.cn

int main(int argc, char **argv)
来源：http://ec.wgjwhj.cn

[S19] C：快速排序
来源：http://nz.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lh.shtwfgs.cn

[S20] C：二分查找
来源：http://gb.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ru.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ns.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qv.asd995.cn

[S22] C：字符串转数字
来源：http://ps.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sv.asd995.cn

[S23] C：随机数
来源：http://qf.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xb.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ik.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tx.shtwfgs.cn

[S25] C：内存拷贝
来源：http://dw.yuexingan06.cn

memcpy(dst, src, n);
来源：http://am.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ag.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://zg.jianghongdianzi.cn

[S27] C：定义常量
来源：http://zw.shxzukj.cn

const double PI = 3.14159;
来源：http://hm.asd995.cn

[S28] C：静态变量
来源：http://lj.shxzskj.cn

static int counter = 0;
来源：http://ry.newstarts.cn

[S29] C：变参函数
来源：http://ns.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ng.wgjwhj.cn

[S30] C：头文件保护
来源：http://fw.nszjky.cn

#ifndef X_H
来源：http://py.szxytkj.cn

#define X_H
来源：http://nd.newstarts.cn

#endif
来源：http://kv.shxzskj.cn

[S31] C++：Hello World
来源：http://om.chemitech.net.cn

#include <iostream>
来源：http://rw.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://tu.bookmarksfly.cn

[S32] C++：字符串
来源：http://av.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://gw.huanxung.cn

[S33] C++：vector 增删
来源：http://xk.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vt.9csxet.cn

[S34] C++：遍历 vector
来源：http://dz.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://vf.haigaiapp.cn

[S35] C++：map
来源：http://bm.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kk.haigaiapp.cn

[S36] C++：unordered_map
来源：http://hr.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qk.521024.cn


<!-- 参考信息 -->