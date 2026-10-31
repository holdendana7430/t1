代发 wailian999

ROLLBACK TO sp1;
来源：http://jc.bookmarksfly.cn

[Q69] 查看执行计划
来源：http://hm.szsharing.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ep.nicolike.cn

[Q70] 更新统计信息
来源：http://ni.asd995.cn

ANALYZE TABLE users;
来源：http://yh.huixiangedu.cn

[Q71] 查看建表语句
来源：http://at.hahajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nm.colortex.cn

[Q72] 查看索引
来源：http://lc.colortex.cn

SHOW INDEX FROM users;
来源：http://iu.nicolike.cn

[Q73] 查看表状态
来源：http://uh.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qw.huixiangedu.cn

[Q74] 强制使用索引
来源：http://to.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://um.nszjky.cn

[Q75] 日期格式化
来源：http://pa.szxytkj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xi.panjiajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cu.9csxet.cn

[Q76] 按天统计
来源：http://pe.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ov.shtwfgs.cn

[Q77] 时间加减
来源：http://nc.szsharing.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ls.bookmarksfly.cn

[Q78] 当前时间
来源：http://du.hahajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://it.lnxyls.cn

[Q79] 字符串拼接
来源：http://qd.bookmarksfly.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://co.haigaiapp.cn

[Q80] 字符串截取
来源：http://lm.bjjhwx.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vd.panjiajie.cn

[Q81] 字符串替换
来源：http://so.shtwfgs.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uq.yuntaijiaju.cn

[Q82] 字符长度与字节长度
来源：http://mp.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xu.huixinmuqiang.cn

[Q83] 大小写转换
来源：http://kk.521024.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tk.lnxyls.cn

[Q84] 去除首尾空格
来源：http://yo.panjiajie.cn

SELECT TRIM(name) FROM users;
来源：http://dn.gzmigu.cn

[Q85] 数值取整
来源：http://rv.bookmarksfly.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kw.colortex.cn

[Q86] 读取 JSON 字段
来源：http://bt.huanxung.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mi.asd995.cn

[Q87] JSON 字段做条件
来源：http://bw.nszjky.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ho.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://my.colortex.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yx.9csxet.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xv.muxihuayi.cn

[Q89] 判断表是否存在
来源：http://ka.nicolike.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ui.chemitech.net.cn

[Q90] 生成序号列
来源：http://um.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pi.nszjky.cn

================================================================================
来源：http://mh.wgjwhj.cn

R. Bash 专题
来源：http://qs.521024.cn

================================================================================
来源：http://no.szsharing.cn

[R01] shebang 与严格模式
来源：http://xg.chemitech.net.cn

#!/usr/bin/env bash
来源：http://bq.9csxet.cn

set -euo pipefail
来源：http://qv.szxytkj.cn

[R02] 变量赋值与使用
来源：http://mt.shxzukj.cn

name="Tom"; echo "$name"
来源：http://oa.chemitech.net.cn

[R03] 只读变量
来源：http://ap.jctech888.com.cn

readonly PI=3.14
来源：http://qj.yuntaijiaju.cn

[R04] 位置参数
来源：http://uo.huixinmuqiang.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xn.newstarts.cn

[R05] 参数默认值
来源：http://il.521024.cn

name="${1:-default}"
来源：http://gm.hahajie.cn

[R06] 判断命令是否存在
来源：http://qn.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ln.panjiajie.cn

[R07] if 判断文件
来源：http://sp.shxzukj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://do.jctech888.com.cn

[R08] 数值比较
来源：http://lr.9csxet.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dv.wgjwhj.cn

[R09] 字符串比较
来源：http://qu.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://li.colortex.cn

[R10] 正则匹配
来源：http://au.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ff.shtwfgs.cn

[R11] case 多分支
来源：http://nm.bjjhwx.cn

case "$1" in
来源：http://ip.colortex.cn

start) echo "启动" ;;
来源：http://lk.bookmarksfly.cn

stop)  echo "停止" ;;
来源：http://wb.panjiajie.cn

*)     echo "未知命令" ;;
来源：http://io.szsharing.cn

esac
来源：http://xh.521024.cn

[R12] for 遍历文件
来源：http://tc.szxytkj.cn

for f in *.txt; do echo "$f"; done
来源：http://gt.yuexingan06.cn

[R13] for 计数循环
来源：http://go.huixinmuqiang.cn

for i in {1..10}; do echo "$i"; done
来源：http://rf.newstarts.cn

[R14] C 风格 for
来源：http://aa.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fp.shtwfgs.cn

[R15] while 逐行读文件
来源：http://xs.asd995.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lc.gzmigu.cn

[R16] until 等待条件
来源：http://no.huixinmuqiang.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ul.chemitech.net.cn

[R17] 数组定义与取值
来源：http://mb.huanxung.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nf.asd995.cn

[R18] 遍历数组
来源：http://ox.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ek.gzmigu.cn

[R19] 数组长度
来源：http://fd.gzmigu.cn

echo "${#arr[@]}"
来源：http://oy.colortex.cn

[R20] 关联数组（字典）
来源：http://ip.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ds.nicolike.cn

[R21] 字符串长度
来源：http://zf.huixiangedu.cn

echo "${#s}"
来源：http://rz.newstarts.cn

[R22] 截取子串
来源：http://fd.gzmigu.cn

echo "${s:0:5}"
来源：http://to.yuntaijiaju.cn

[R23] 字符串替换
来源：http://pt.hnjuh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sd.nszjky.cn

[R24] 大小写转换
来源：http://yy.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://en.yuntaijiaju.cn

[R25] 去后缀 / 去前缀
来源：http://xp.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sv.shtwfgs.cn

[R26] 命令替换
来源：http://pv.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://fv.jianghongdianzi.cn

[R27] 算术展开
来源：http://nf.bjjhwx.cn

echo $((1 + 2 * 3))
来源：http://lf.gzmigu.cn

[R28] 浮点运算
来源：http://bw.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://zl.nicolike.cn

[R29] 定义函数
来源：http://uj.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hk.panjiajie.cn

[R30] 函数返回状态码
来源：http://cb.szsharing.cn

f() { return 0; }; f || echo "失败了"
来源：http://ar.bookmarksfly.cn

[R31] 局部变量
来源：http://vq.haigaiapp.cn

f() { local x=1; echo "$x"; }
来源：http://tg.jctech888.com.cn

[R32] 参数个数校验
来源：http://gb.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fx.hnjuh.cn

[R33] 捕获错误并提示行号
来源：http://up.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kp.wgjwhj.cn

[R34] 退出时清理
来源：http://bn.yuexingan06.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pv.huanxung.cn

[R35] 后台执行并等待
来源：http://bf.huanxung.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sm.lnxyls.cn

[R36] 并发执行多个任务
来源：http://pa.9csxet.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pc.hnjuh.cn

[R37] 把输出赋给变量
来源：http://hf.521024.cn

files=$(ls -1)
来源：http://je.jctech888.com.cn

[R38] 管道串联
来源：http://zq.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://qp.newstarts.cn

[R39] 重定向标准输出与错误
来源：http://is.yuexingan06.cn

cmd > out.log 2>&1
来源：http://dd.shxzskj.cn

[R40] 追加写日志
来源：http://qb.bjjhwx.cn

echo "log" >> out.log
来源：http://jl.yuntaijiaju.cn

[R41] 丢弃输出
来源：http://tl.jctech888.com.cn

cmd >/dev/null 2>&1
来源：http://lw.panjiajie.cn

[R42] 输入重定向
来源：http://yt.szxytkj.cn

wc -l < a.txt
来源：http://lv.haigaiapp.cn

[R43] 按名字查找文件
来源：http://aj.521024.cn

find . -name "*.log" -type f
来源：http://wd.chemitech.net.cn

[R44] 按修改时间查找
来源：http://zf.yuntaijiaju.cn

find . -mtime -7 -type f
来源：http://rk.hahajie.cn

[R45] 批量删除
来源：http://ce.muxihuayi.cn

find . -name "*.tmp" -delete
来源：http://os.shxzskj.cn

[R46] 递归替换文件内容
来源：http://po.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://th.huixiangedu.cn

[R47] sed 单行替换
来源：http://yw.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tw.szsharing.cn

[R48] awk 取指定列
来源：http://hd.lnxyls.cn

awk '{print $1, $3}' a.txt
来源：http://fy.9csxet.cn

[R49] awk 带条件
来源：http://vq.shxzskj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nw.521024.cn

[R50] awk 求和
来源：http://pk.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aj.hahajie.cn

[R51] 排序去重取前几
来源：http://ge.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ny.chemitech.net.cn

[R52] 统计行数
来源：http://km.muxihuayi.cn

wc -l a.txt
来源：http://lx.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://pc.bookmarksfly.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nh.yuexingan06.cn

[R54] 比较两个文件
来源：http://ut.shtwfgs.cn

diff a.txt b.txt
来源：http://to.chemitech.net.cn

[R55] 压缩与解压
来源：http://dd.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://me.521024.cn

[R56] 远程拷贝
来源：http://hf.huanxung.cn

scp file user@host:/path/
来源：http://ad.nszjky.cn

[R57] 远程执行命令
来源：http://qc.shtwfgs.cn

ssh user@host 'uptime'
来源：http://pf.yuexingan06.cn

[R58] 下载文件
来源：http://rd.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ng.9csxet.cn

[R59] 发 POST JSON
来源：http://jv.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eb.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://zm.9csxet.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://id.shtwfgs.cn

[R61] 磁盘占用
来源：http://tn.521024.cn

df -h;  du -sh *
来源：http://ue.szsharing.cn

[R62] 找最占空间的文件
来源：http://in.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://kv.muxihuayi.cn

[R63] 内存与进程
来源：http://pe.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://dk.bookmarksfly.cn

[R64] 结束进程
来源：http://mh.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://ll.colortex.cn

[R65] 查看端口占用
来源：http://rx.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://me.szxytkj.cn

[R66] 定时任务
来源：http://mg.hnjuh.cn

crontab -e;  crontab -l
来源：http://yt.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://ec.jianghongdianzi.cn

openssl rand -hex 16
来源：http://wk.jctech888.com.cn

[R68] 计算文件校验值
来源：http://cd.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ff.asd995.cn

[R69] 生成随机密码
来源：http://bq.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://bd.lnxyls.cn

[R70] 时间戳与互转
来源：http://rn.haigaiapp.cn

date +%s;  date -d @1700000000
来源：http://ny.chemitech.net.cn

[R71] 日期格式化
来源：http://eo.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oq.jctech888.com.cn

[R72] 等待端口就绪
来源：http://ly.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rh.bookmarksfly.cn

[R73] 分割大日志
来源：http://jy.521024.cn

split -l 1000 big.log part_
来源：http://aa.shxzukj.cn

[R74] 批量重命名
来源：http://rr.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zh.huixiangedu.cn

[R75] 导出环境变量
来源：http://ci.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://ei.asd995.cn

[R76] 使用临时文件
来源：http://ru.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ap.shxzukj.cn

[R77] 读取用户输入
来源：http://ai.hahajie.cn

read -rp "请输入: " ans
来源：http://wc.shtwfgs.cn

[R78] 交互式菜单
来源：http://he.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xs.hahajie.cn

[R79] 解析命令行选项
来源：http://aj.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zz.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://tm.521024.cn

time ./run.sh
来源：http://is.szsharing.cn

================================================================================
来源：http://dz.huixiangedu.cn

S. C / C++ 专题
来源：http://dx.lnxyls.cn

================================================================================
来源：http://kp.huixinmuqiang.cn

[S01] C：Hello World
来源：http://cv.muxihuayi.cn

#include <stdio.h>
来源：http://kw.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dx.huanxung.cn

[S02] C：变量与格式化输出
来源：http://vd.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://mh.yuexingan06.cn

[S03] C：读入整数
来源：http://fl.9csxet.cn

int x; scanf("%d", &x);
来源：http://oo.chemitech.net.cn

[S04] C：字符串复制
来源：http://bd.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vy.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://sm.shxzskj.cn

strlen(s)
来源：http://uv.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://py.lnxyls.cn

strcmp(a, b) == 0
来源：http://di.szxytkj.cn

[S07] C：数组遍历求和
来源：http://il.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qa.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://ud.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fe.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://op.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pa.wgjwhj.cn

[S10] C：指针与解引用
来源：http://qw.hahajie.cn

int *p = &a;  *p = 5;
来源：http://qu.newstarts.cn

[S11] C：逐行读文件
来源：http://fq.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://dn.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lz.gzmigu.cn

fclose(f);
来源：http://px.chemitech.net.cn

[S12] C：写文件
来源：http://dp.haigaiapp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mc.panjiajie.cn

[S13] C：宏定义
来源：http://ye.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hw.bjjhwx.cn

[S14] C：枚举
来源：http://mf.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://xa.lnxyls.cn

[S15] C：类型转换
来源：http://il.chemitech.net.cn

(double) a / b
来源：http://bg.colortex.cn

[S16] C：位操作置位
来源：http://kd.bjjhwx.cn

x |= (1 << 3);
来源：http://fp.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://ga.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://os.bjjhwx.cn

[S18] C：命令行参数
来源：http://yt.haigaiapp.cn

int main(int argc, char **argv)
来源：http://jp.shtwfgs.cn

[S19] C：快速排序
来源：http://av.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ru.nszjky.cn

[S20] C：二分查找
来源：http://fs.hahajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tc.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://tn.wgjwhj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lb.hahajie.cn

[S22] C：字符串转数字
来源：http://fk.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://px.colortex.cn

[S23] C：随机数
来源：http://tn.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eq.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://xg.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tg.huanxung.cn

[S25] C：内存拷贝
来源：http://sf.hnjuh.cn

memcpy(dst, src, n);
来源：http://dz.huixiangedu.cn

[S26] C：内存清零
来源：http://ur.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://ie.lnxyls.cn

[S27] C：定义常量
来源：http://ox.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://db.nicolike.cn

[S28] C：静态变量
来源：http://ma.newstarts.cn

static int counter = 0;
来源：http://th.bookmarksfly.cn

[S29] C：变参函数
来源：http://go.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ez.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://id.colortex.cn

#ifndef X_H
来源：http://hk.shtwfgs.cn

#define X_H
来源：http://ol.bjjhwx.cn

#endif
来源：http://bt.nicolike.cn

[S31] C++：Hello World
来源：http://aa.asd995.cn

#include <iostream>
来源：http://sm.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://yy.lnxyls.cn

[S32] C++：字符串
来源：http://qw.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://ay.haigaiapp.cn

[S33] C++：vector 增删
来源：http://nd.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xy.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://vg.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://yp.newstarts.cn

[S35] C++：map
来源：http://tx.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jm.panjiajie.cn

[S36] C++：unordered_map
来源：http://up.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sg.nszjky.cn

[S37] C++：set
来源：http://cn.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://io.521024.cn

[S38] C++：排序
来源：http://tp.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://lq.newstarts.cn


<!-- 参考信息 -->