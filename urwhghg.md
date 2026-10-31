代发 wailian999

[Q67] 设置隔离级别
来源：http://ws.521024.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ba.lnxyls.cn

[Q68] 保存点
来源：http://pk.nicolike.cn

SAVEPOINT sp1;
来源：http://oj.shxzukj.cn

ROLLBACK TO sp1;
来源：http://bi.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://as.muxihuayi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://te.huixiangedu.cn

[Q70] 更新统计信息
来源：http://wh.colortex.cn

ANALYZE TABLE users;
来源：http://jx.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://cl.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ox.wgjwhj.cn

[Q72] 查看索引
来源：http://oe.bjjhwx.cn

SHOW INDEX FROM users;
来源：http://lq.panjiajie.cn

[Q73] 查看表状态
来源：http://uk.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ln.shxzukj.cn

[Q74] 强制使用索引
来源：http://xu.521024.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cv.huanxung.cn

[Q75] 日期格式化
来源：http://jq.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ao.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hf.huanxung.cn

[Q76] 按天统计
来源：http://lz.newstarts.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://er.panjiajie.cn

[Q77] 时间加减
来源：http://kb.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://md.yuntaijiaju.cn

[Q78] 当前时间
来源：http://ny.szsharing.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bi.9csxet.cn

[Q79] 字符串拼接
来源：http://vw.asd995.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gw.shtwfgs.cn

[Q80] 字符串截取
来源：http://nj.shxzskj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uz.nszjky.cn

[Q81] 字符串替换
来源：http://fo.huixiangedu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qh.szxytkj.cn

[Q82] 字符长度与字节长度
来源：http://nn.szsharing.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bc.szxytkj.cn

[Q83] 大小写转换
来源：http://ef.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pl.nszjky.cn

[Q84] 去除首尾空格
来源：http://gn.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://sl.shxzskj.cn

[Q85] 数值取整
来源：http://fy.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zm.9csxet.cn

[Q86] 读取 JSON 字段
来源：http://ct.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cg.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://ov.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wo.colortex.cn

[Q88] 行转列（条件聚合）
来源：http://dc.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iv.haigaiapp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pp.hnjuh.cn

[Q89] 判断表是否存在
来源：http://jx.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tr.panjiajie.cn

[Q90] 生成序号列
来源：http://eu.szsharing.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uq.asd995.cn

================================================================================
来源：http://ss.asd995.cn

R. Bash 专题
来源：http://he.jianghongdianzi.cn

================================================================================
来源：http://yi.shxzukj.cn

[R01] shebang 与严格模式
来源：http://zv.szxytkj.cn

#!/usr/bin/env bash
来源：http://in.wgjwhj.cn

set -euo pipefail
来源：http://dr.shxzukj.cn

[R02] 变量赋值与使用
来源：http://jm.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://ps.huixiangedu.cn

[R03] 只读变量
来源：http://rg.panjiajie.cn

readonly PI=3.14
来源：http://hh.yuntaijiaju.cn

[R04] 位置参数
来源：http://xp.jianghongdianzi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nw.hnjuh.cn

[R05] 参数默认值
来源：http://zh.shxzukj.cn

name="${1:-default}"
来源：http://ny.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://vo.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yp.wgjwhj.cn

[R07] if 判断文件
来源：http://ao.huanxung.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ke.szxytkj.cn

[R08] 数值比较
来源：http://dj.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ie.521024.cn

[R09] 字符串比较
来源：http://bm.gzmigu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zk.panjiajie.cn

[R10] 正则匹配
来源：http://rc.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cq.gzmigu.cn

[R11] case 多分支
来源：http://bk.shtwfgs.cn

case "$1" in
来源：http://hs.yuexingan06.cn

start) echo "启动" ;;
来源：http://lq.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://zu.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://so.muxihuayi.cn

esac
来源：http://jd.hnjuh.cn

[R12] for 遍历文件
来源：http://ez.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://rb.shtwfgs.cn

[R13] for 计数循环
来源：http://ow.nicolike.cn

for i in {1..10}; do echo "$i"; done
来源：http://qm.shtwfgs.cn

[R14] C 风格 for
来源：http://ho.huixinmuqiang.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lb.yuntaijiaju.cn

[R15] while 逐行读文件
来源：http://jg.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wo.asd995.cn

[R16] until 等待条件
来源：http://oa.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://np.huixinmuqiang.cn

[R17] 数组定义与取值
来源：http://zz.lnxyls.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bn.nszjky.cn

[R18] 遍历数组
来源：http://pt.haigaiapp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ms.yuexingan06.cn

[R19] 数组长度
来源：http://ch.panjiajie.cn

echo "${#arr[@]}"
来源：http://ct.521024.cn

[R20] 关联数组（字典）
来源：http://gy.shtwfgs.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uj.shtwfgs.cn

[R21] 字符串长度
来源：http://vq.huanxung.cn

echo "${#s}"
来源：http://sz.bookmarksfly.cn

[R22] 截取子串
来源：http://qd.panjiajie.cn

echo "${s:0:5}"
来源：http://du.panjiajie.cn

[R23] 字符串替换
来源：http://yk.szxytkj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hr.panjiajie.cn

[R24] 大小写转换
来源：http://il.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ls.lnxyls.cn

[R25] 去后缀 / 去前缀
来源：http://pu.haigaiapp.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nk.jctech888.com.cn

[R26] 命令替换
来源：http://by.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://ab.nicolike.cn

[R27] 算术展开
来源：http://au.huixinmuqiang.cn

echo $((1 + 2 * 3))
来源：http://tb.9csxet.cn

[R28] 浮点运算
来源：http://vx.wgjwhj.cn

echo "scale=2; 10/3" | bc
来源：http://im.szsharing.cn

[R29] 定义函数
来源：http://si.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qt.shtwfgs.cn

[R30] 函数返回状态码
来源：http://eo.hnjuh.cn

f() { return 0; }; f || echo "失败了"
来源：http://yd.521024.cn

[R31] 局部变量
来源：http://ll.newstarts.cn

f() { local x=1; echo "$x"; }
来源：http://qo.chemitech.net.cn

[R32] 参数个数校验
来源：http://xq.nszjky.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nz.9csxet.cn

[R33] 捕获错误并提示行号
来源：http://ya.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://do.haigaiapp.cn

[R34] 退出时清理
来源：http://ze.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nj.asd995.cn

[R35] 后台执行并等待
来源：http://yc.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ob.chemitech.net.cn

[R36] 并发执行多个任务
来源：http://nj.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sv.szxytkj.cn

[R37] 把输出赋给变量
来源：http://me.hahajie.cn

files=$(ls -1)
来源：http://ui.yuexingan06.cn

[R38] 管道串联
来源：http://mz.bookmarksfly.cn

cat a.txt | grep -i error | wc -l
来源：http://ap.chemitech.net.cn

[R39] 重定向标准输出与错误
来源：http://zf.yuexingan06.cn

cmd > out.log 2>&1
来源：http://fm.yuexingan06.cn

[R40] 追加写日志
来源：http://ug.huanxung.cn

echo "log" >> out.log
来源：http://qs.panjiajie.cn

[R41] 丢弃输出
来源：http://kj.colortex.cn

cmd >/dev/null 2>&1
来源：http://cp.nicolike.cn

[R42] 输入重定向
来源：http://gz.huixinmuqiang.cn

wc -l < a.txt
来源：http://iv.huixiangedu.cn

[R43] 按名字查找文件
来源：http://wj.lnxyls.cn

find . -name "*.log" -type f
来源：http://en.asd995.cn

[R44] 按修改时间查找
来源：http://yw.bjjhwx.cn

find . -mtime -7 -type f
来源：http://lq.panjiajie.cn

[R45] 批量删除
来源：http://vz.huanxung.cn

find . -name "*.tmp" -delete
来源：http://vr.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://zd.shxzskj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://df.jctech888.com.cn

[R47] sed 单行替换
来源：http://zv.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oi.huanxung.cn

[R48] awk 取指定列
来源：http://su.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://ni.lnxyls.cn

[R49] awk 带条件
来源：http://vy.jianghongdianzi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cr.hahajie.cn

[R50] awk 求和
来源：http://zo.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ls.521024.cn

[R51] 排序去重取前几
来源：http://kg.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zk.szxytkj.cn

[R52] 统计行数
来源：http://vv.chemitech.net.cn

wc -l a.txt
来源：http://wf.bookmarksfly.cn

[R53] 查看文件头与实时尾
来源：http://xd.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://st.521024.cn

[R54] 比较两个文件
来源：http://rk.newstarts.cn

diff a.txt b.txt
来源：http://lt.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://lp.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ug.bookmarksfly.cn

[R56] 远程拷贝
来源：http://bx.chemitech.net.cn

scp file user@host:/path/
来源：http://zt.521024.cn

[R57] 远程执行命令
来源：http://uv.muxihuayi.cn

ssh user@host 'uptime'
来源：http://nd.muxihuayi.cn

[R58] 下载文件
来源：http://iq.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bb.shxzukj.cn

[R59] 发 POST JSON
来源：http://zv.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xc.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://za.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gj.gzmigu.cn

[R61] 磁盘占用
来源：http://zm.chemitech.net.cn

df -h;  du -sh *
来源：http://rm.hahajie.cn

[R62] 找最占空间的文件
来源：http://zb.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://ws.hnjuh.cn

[R63] 内存与进程
来源：http://fb.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://jg.hahajie.cn

[R64] 结束进程
来源：http://kx.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://kx.jianghongdianzi.cn

[R65] 查看端口占用
来源：http://xh.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nz.shtwfgs.cn

[R66] 定时任务
来源：http://dx.hnjuh.cn

crontab -e;  crontab -l
来源：http://im.huanxung.cn

[R67] 生成随机十六进制串
来源：http://de.szxytkj.cn

openssl rand -hex 16
来源：http://yn.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://te.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rj.9csxet.cn

[R69] 生成随机密码
来源：http://me.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://dd.huixiangedu.cn

[R70] 时间戳与互转
来源：http://tb.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://kl.9csxet.cn

[R71] 日期格式化
来源：http://hu.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ej.9csxet.cn

[R72] 等待端口就绪
来源：http://dz.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://il.shtwfgs.cn

[R73] 分割大日志
来源：http://mh.yuexingan06.cn

split -l 1000 big.log part_
来源：http://ub.haigaiapp.cn

[R74] 批量重命名
来源：http://ms.jianghongdianzi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qd.shxzskj.cn

[R75] 导出环境变量
来源：http://yf.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://nu.shtwfgs.cn

[R76] 使用临时文件
来源：http://ur.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ht.gzmigu.cn

[R77] 读取用户输入
来源：http://bd.asd995.cn

read -rp "请输入: " ans
来源：http://ws.nicolike.cn

[R78] 交互式菜单
来源：http://ud.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wj.bjjhwx.cn

[R79] 解析命令行选项
来源：http://co.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ze.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://yn.haigaiapp.cn

time ./run.sh
来源：http://vx.chemitech.net.cn

================================================================================
来源：http://kl.521024.cn

S. C / C++ 专题
来源：http://df.jianghongdianzi.cn

================================================================================
来源：http://my.shxzskj.cn

[S01] C：Hello World
来源：http://ej.nszjky.cn

#include <stdio.h>
来源：http://xt.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ah.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://py.szxytkj.cn

int a = 10; printf("%d\n", a);
来源：http://dn.haigaiapp.cn

[S03] C：读入整数
来源：http://gm.panjiajie.cn

int x; scanf("%d", &x);
来源：http://fx.hahajie.cn

[S04] C：字符串复制
来源：http://im.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://up.9csxet.cn

[S05] C：字符串长度
来源：http://jr.asd995.cn

strlen(s)
来源：http://hz.szxytkj.cn

[S06] C：字符串比较
来源：http://zx.gzmigu.cn

strcmp(a, b) == 0
来源：http://kj.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://tv.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hc.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://vu.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bo.asd995.cn

[S09] C：结构体定义与初始化
来源：http://ig.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gz.shxzskj.cn

[S10] C：指针与解引用
来源：http://ml.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://aa.gzmigu.cn

[S11] C：逐行读文件
来源：http://ii.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://eu.panjiajie.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nz.jianghongdianzi.cn

fclose(f);
来源：http://ou.lnxyls.cn

[S12] C：写文件
来源：http://dv.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cz.wgjwhj.cn

[S13] C：宏定义
来源：http://xm.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ap.hnjuh.cn

[S14] C：枚举
来源：http://aw.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://gg.shtwfgs.cn

[S15] C：类型转换
来源：http://wl.szxytkj.cn

(double) a / b
来源：http://yj.shxzskj.cn

[S16] C：位操作置位
来源：http://ug.chemitech.net.cn

x |= (1 << 3);
来源：http://xu.szsharing.cn

[S17] C：安全拼接字符串
来源：http://ci.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ee.asd995.cn

[S18] C：命令行参数
来源：http://sn.newstarts.cn

int main(int argc, char **argv)
来源：http://hp.jctech888.com.cn

[S19] C：快速排序
来源：http://on.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nz.huixinmuqiang.cn

[S20] C：二分查找
来源：http://xl.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mu.bjjhwx.cn

[S21] C：字符类别判断
来源：http://bn.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wu.shxzukj.cn

[S22] C：字符串转数字
来源：http://ab.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ik.jctech888.com.cn

[S23] C：随机数
来源：http://ab.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mn.hahajie.cn

[S24] C：获取本地时间
来源：http://qs.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pt.szxytkj.cn

[S25] C：内存拷贝
来源：http://zn.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://od.newstarts.cn

[S26] C：内存清零
来源：http://di.huanxung.cn

memset(a, 0, sizeof a);
来源：http://dc.chemitech.net.cn

[S27] C：定义常量
来源：http://vt.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://bo.asd995.cn

[S28] C：静态变量
来源：http://lf.bookmarksfly.cn

static int counter = 0;
来源：http://km.shxzskj.cn

[S29] C：变参函数
来源：http://tp.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xu.huanxung.cn

[S30] C：头文件保护
来源：http://ju.hahajie.cn

#ifndef X_H
来源：http://hg.colortex.cn

#define X_H
来源：http://eb.yuexingan06.cn

#endif
来源：http://dg.9csxet.cn

[S31] C++：Hello World
来源：http://vu.colortex.cn

#include <iostream>
来源：http://wl.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://kl.newstarts.cn

[S32] C++：字符串
来源：http://sy.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://ke.jctech888.com.cn

[S33] C++：vector 增删
来源：http://mf.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lf.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://yu.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://xc.szsharing.cn

[S35] C++：map
来源：http://cy.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kd.huanxung.cn

[S36] C++：unordered_map
来源：http://sj.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ky.panjiajie.cn


<!-- 参考信息 -->