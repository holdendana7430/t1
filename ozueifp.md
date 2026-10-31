代发 wailian999

ROLLBACK TO sp1;
来源：http://sy.hahajie.cn

[Q69] 查看执行计划
来源：http://lg.521024.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qq.wgjwhj.cn

[Q70] 更新统计信息
来源：http://px.hahajie.cn

ANALYZE TABLE users;
来源：http://jz.hahajie.cn

[Q71] 查看建表语句
来源：http://cq.huixinmuqiang.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://su.yuntaijiaju.cn

[Q72] 查看索引
来源：http://ug.colortex.cn

SHOW INDEX FROM users;
来源：http://ae.hahajie.cn

[Q73] 查看表状态
来源：http://xm.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ca.newstarts.cn

[Q74] 强制使用索引
来源：http://mc.lnxyls.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wm.huanxung.cn

[Q75] 日期格式化
来源：http://si.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ia.huanxung.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://im.shxzukj.cn

[Q76] 按天统计
来源：http://en.szsharing.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ft.hnjuh.cn

[Q77] 时间加减
来源：http://js.haigaiapp.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rx.colortex.cn

[Q78] 当前时间
来源：http://xb.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jw.huixinmuqiang.cn

[Q79] 字符串拼接
来源：http://vc.wgjwhj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://at.szsharing.cn

[Q80] 字符串截取
来源：http://ps.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mz.hahajie.cn

[Q81] 字符串替换
来源：http://kb.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iy.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://ri.521024.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cf.shxzukj.cn

[Q83] 大小写转换
来源：http://xq.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jv.nszjky.cn

[Q84] 去除首尾空格
来源：http://rp.yuntaijiaju.cn

SELECT TRIM(name) FROM users;
来源：http://ks.nszjky.cn

[Q85] 数值取整
来源：http://va.huanxung.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nc.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://kr.yuexingan06.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zj.huixiangedu.cn

[Q87] JSON 字段做条件
来源：http://lz.yuntaijiaju.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ri.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://js.asd995.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lx.jctech888.com.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pq.szxytkj.cn

[Q89] 判断表是否存在
来源：http://ht.hahajie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fh.lnxyls.cn

[Q90] 生成序号列
来源：http://sy.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://in.newstarts.cn

================================================================================
来源：http://ha.hnjuh.cn

R. Bash 专题
来源：http://ns.yuexingan06.cn

================================================================================
来源：http://ci.szsharing.cn

[R01] shebang 与严格模式
来源：http://sq.asd995.cn

#!/usr/bin/env bash
来源：http://vh.huixiangedu.cn

set -euo pipefail
来源：http://kp.lnxyls.cn

[R02] 变量赋值与使用
来源：http://mx.chemitech.net.cn

name="Tom"; echo "$name"
来源：http://iz.huixiangedu.cn

[R03] 只读变量
来源：http://lu.gzmigu.cn

readonly PI=3.14
来源：http://fr.bjjhwx.cn

[R04] 位置参数
来源：http://qc.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tl.haigaiapp.cn

[R05] 参数默认值
来源：http://ki.yuexingan06.cn

name="${1:-default}"
来源：http://es.muxihuayi.cn

[R06] 判断命令是否存在
来源：http://na.shxzskj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lp.yuntaijiaju.cn

[R07] if 判断文件
来源：http://rq.yuntaijiaju.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aj.szxytkj.cn

[R08] 数值比较
来源：http://sp.huixinmuqiang.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nk.asd995.cn

[R09] 字符串比较
来源：http://ex.lnxyls.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zg.chemitech.net.cn

[R10] 正则匹配
来源：http://zj.haigaiapp.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kg.nszjky.cn

[R11] case 多分支
来源：http://of.jianghongdianzi.cn

case "$1" in
来源：http://yw.huanxung.cn

start) echo "启动" ;;
来源：http://je.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://kg.szsharing.cn

*)     echo "未知命令" ;;
来源：http://so.yuexingan06.cn

esac
来源：http://bb.yuexingan06.cn

[R12] for 遍历文件
来源：http://cb.yuntaijiaju.cn

for f in *.txt; do echo "$f"; done
来源：http://oj.colortex.cn

[R13] for 计数循环
来源：http://qh.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://jy.huanxung.cn

[R14] C 风格 for
来源：http://en.newstarts.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://re.colortex.cn

[R15] while 逐行读文件
来源：http://up.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ti.colortex.cn

[R16] until 等待条件
来源：http://vm.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fg.yuexingan06.cn

[R17] 数组定义与取值
来源：http://pc.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kb.colortex.cn

[R18] 遍历数组
来源：http://fc.lnxyls.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://il.huixinmuqiang.cn

[R19] 数组长度
来源：http://mo.colortex.cn

echo "${#arr[@]}"
来源：http://ef.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://wu.jianghongdianzi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ii.huanxung.cn

[R21] 字符串长度
来源：http://cj.521024.cn

echo "${#s}"
来源：http://sx.yuntaijiaju.cn

[R22] 截取子串
来源：http://ec.huixiangedu.cn

echo "${s:0:5}"
来源：http://kv.huixiangedu.cn

[R23] 字符串替换
来源：http://ub.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://th.shxzukj.cn

[R24] 大小写转换
来源：http://ng.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cm.huixinmuqiang.cn

[R25] 去后缀 / 去前缀
来源：http://od.chemitech.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xp.chemitech.net.cn

[R26] 命令替换
来源：http://hp.colortex.cn

now=$(date +%F); echo "$now"
来源：http://aa.lnxyls.cn

[R27] 算术展开
来源：http://fg.chemitech.net.cn

echo $((1 + 2 * 3))
来源：http://zp.jianghongdianzi.cn

[R28] 浮点运算
来源：http://fl.jctech888.com.cn

echo "scale=2; 10/3" | bc
来源：http://xw.yuexingan06.cn

[R29] 定义函数
来源：http://le.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lh.shtwfgs.cn

[R30] 函数返回状态码
来源：http://nh.panjiajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://tu.shtwfgs.cn

[R31] 局部变量
来源：http://jk.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://oz.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://dd.szxytkj.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xy.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://rf.asd995.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eg.nicolike.cn

[R34] 退出时清理
来源：http://ge.jianghongdianzi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ya.nszjky.cn

[R35] 后台执行并等待
来源：http://ux.colortex.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vq.hnjuh.cn

[R36] 并发执行多个任务
来源：http://gp.shtwfgs.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xe.shxzskj.cn

[R37] 把输出赋给变量
来源：http://qv.shtwfgs.cn

files=$(ls -1)
来源：http://mi.hnjuh.cn

[R38] 管道串联
来源：http://tl.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://sc.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://iw.jianghongdianzi.cn

cmd > out.log 2>&1
来源：http://yj.wgjwhj.cn

[R40] 追加写日志
来源：http://bv.lnxyls.cn

echo "log" >> out.log
来源：http://wb.shxzskj.cn

[R41] 丢弃输出
来源：http://eo.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://xk.yuntaijiaju.cn

[R42] 输入重定向
来源：http://kw.yuntaijiaju.cn

wc -l < a.txt
来源：http://xq.colortex.cn

[R43] 按名字查找文件
来源：http://da.9csxet.cn

find . -name "*.log" -type f
来源：http://pw.szxytkj.cn

[R44] 按修改时间查找
来源：http://xq.haigaiapp.cn

find . -mtime -7 -type f
来源：http://oi.521024.cn

[R45] 批量删除
来源：http://qb.lnxyls.cn

find . -name "*.tmp" -delete
来源：http://ac.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://xj.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xk.bookmarksfly.cn

[R47] sed 单行替换
来源：http://ew.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rn.shtwfgs.cn

[R48] awk 取指定列
来源：http://ib.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://re.bookmarksfly.cn

[R49] awk 带条件
来源：http://xt.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wt.newstarts.cn

[R50] awk 求和
来源：http://qi.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sg.haigaiapp.cn

[R51] 排序去重取前几
来源：http://gb.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fv.9csxet.cn

[R52] 统计行数
来源：http://cb.521024.cn

wc -l a.txt
来源：http://lz.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://xw.hnjuh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jf.huixiangedu.cn

[R54] 比较两个文件
来源：http://pc.szsharing.cn

diff a.txt b.txt
来源：http://yt.9csxet.cn

[R55] 压缩与解压
来源：http://rc.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fe.shxzukj.cn

[R56] 远程拷贝
来源：http://bl.hahajie.cn

scp file user@host:/path/
来源：http://pq.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://lx.wgjwhj.cn

ssh user@host 'uptime'
来源：http://bu.huanxung.cn

[R58] 下载文件
来源：http://dn.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vu.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://mk.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rl.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://xj.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fs.huixinmuqiang.cn

[R61] 磁盘占用
来源：http://oj.panjiajie.cn

df -h;  du -sh *
来源：http://cu.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://lt.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://so.huanxung.cn

[R63] 内存与进程
来源：http://gw.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://nl.wgjwhj.cn

[R64] 结束进程
来源：http://ix.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://je.jctech888.com.cn

[R65] 查看端口占用
来源：http://tv.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ar.yuexingan06.cn

[R66] 定时任务
来源：http://hj.hahajie.cn

crontab -e;  crontab -l
来源：http://ry.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://an.asd995.cn

openssl rand -hex 16
来源：http://jb.9csxet.cn

[R68] 计算文件校验值
来源：http://ru.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ld.shxzukj.cn

[R69] 生成随机密码
来源：http://ph.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://iy.9csxet.cn

[R70] 时间戳与互转
来源：http://lk.yuntaijiaju.cn

date +%s;  date -d @1700000000
来源：http://ln.shtwfgs.cn

[R71] 日期格式化
来源：http://yo.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dk.shtwfgs.cn

[R72] 等待端口就绪
来源：http://fv.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tt.asd995.cn

[R73] 分割大日志
来源：http://vq.colortex.cn

split -l 1000 big.log part_
来源：http://cp.haigaiapp.cn

[R74] 批量重命名
来源：http://pw.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pe.huanxung.cn

[R75] 导出环境变量
来源：http://dm.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://tj.lnxyls.cn

[R76] 使用临时文件
来源：http://rk.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aw.szxytkj.cn

[R77] 读取用户输入
来源：http://hs.shtwfgs.cn

read -rp "请输入: " ans
来源：http://hr.bjjhwx.cn

[R78] 交互式菜单
来源：http://at.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ml.521024.cn

[R79] 解析命令行选项
来源：http://ud.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tj.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ap.wgjwhj.cn

time ./run.sh
来源：http://ya.bjjhwx.cn

================================================================================
来源：http://vw.bjjhwx.cn

S. C / C++ 专题
来源：http://dr.bookmarksfly.cn

================================================================================
来源：http://bv.shxzskj.cn

[S01] C：Hello World
来源：http://wk.jianghongdianzi.cn

#include <stdio.h>
来源：http://wc.yuexingan06.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oe.asd995.cn

[S02] C：变量与格式化输出
来源：http://en.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://sg.shxzukj.cn

[S03] C：读入整数
来源：http://hu.szxytkj.cn

int x; scanf("%d", &x);
来源：http://vj.521024.cn

[S04] C：字符串复制
来源：http://sb.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.shtwfgs.cn

[S05] C：字符串长度
来源：http://el.shxzskj.cn

strlen(s)
来源：http://qe.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://yu.nicolike.cn

strcmp(a, b) == 0
来源：http://oe.panjiajie.cn

[S07] C：数组遍历求和
来源：http://uy.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://em.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://vg.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rv.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://io.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lp.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://lr.huixiangedu.cn

int *p = &a;  *p = 5;
来源：http://ha.yuexingan06.cn

[S11] C：逐行读文件
来源：http://bi.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://us.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qd.shxzukj.cn

fclose(f);
来源：http://eu.jctech888.com.cn

[S12] C：写文件
来源：http://pd.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uo.9csxet.cn

[S13] C：宏定义
来源：http://dq.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jl.shtwfgs.cn

[S14] C：枚举
来源：http://jn.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://bl.chemitech.net.cn

[S15] C：类型转换
来源：http://nq.newstarts.cn

(double) a / b
来源：http://yc.haigaiapp.cn

[S16] C：位操作置位
来源：http://ie.wgjwhj.cn

x |= (1 << 3);
来源：http://oe.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://me.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ra.yuexingan06.cn

[S18] C：命令行参数
来源：http://en.shtwfgs.cn

int main(int argc, char **argv)
来源：http://cp.wgjwhj.cn

[S19] C：快速排序
来源：http://xz.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cq.shxzukj.cn

[S20] C：二分查找
来源：http://qf.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://im.huixiangedu.cn

[S21] C：字符类别判断
来源：http://gx.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sw.wgjwhj.cn

[S22] C：字符串转数字
来源：http://pe.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aq.szsharing.cn

[S23] C：随机数
来源：http://bb.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bf.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://ky.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vr.hnjuh.cn

[S25] C：内存拷贝
来源：http://za.szxytkj.cn

memcpy(dst, src, n);
来源：http://ed.asd995.cn

[S26] C：内存清零
来源：http://dd.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://db.gzmigu.cn

[S27] C：定义常量
来源：http://ki.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://zu.jctech888.com.cn

[S28] C：静态变量
来源：http://rt.shtwfgs.cn

static int counter = 0;
来源：http://ek.wgjwhj.cn

[S29] C：变参函数
来源：http://ly.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fv.panjiajie.cn

[S30] C：头文件保护
来源：http://sp.yuntaijiaju.cn

#ifndef X_H
来源：http://ke.szsharing.cn

#define X_H
来源：http://lr.nicolike.cn

#endif
来源：http://tz.huixiangedu.cn

[S31] C++：Hello World
来源：http://hy.nszjky.cn

#include <iostream>
来源：http://ih.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://vp.newstarts.cn

[S32] C++：字符串
来源：http://do.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://km.hnjuh.cn

[S33] C++：vector 增删
来源：http://da.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qy.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://ne.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://up.yuntaijiaju.cn

[S35] C++：map
来源：http://gf.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sl.bjjhwx.cn

[S36] C++：unordered_map
来源：http://ch.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kt.jianghongdianzi.cn

[S37] C++：set
来源：http://eh.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bv.hahajie.cn

[S38] C++：排序
来源：http://xc.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://vs.521024.cn


<!-- 参考信息 -->