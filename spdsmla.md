代发 wailian999

ROLLBACK TO sp1;
来源：http://uc.haigaiapp.cn

[Q69] 查看执行计划
来源：http://xg.bjjhwx.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cp.panjiajie.cn

[Q70] 更新统计信息
来源：http://zp.gzmigu.cn

ANALYZE TABLE users;
来源：http://ju.szxytkj.cn

[Q71] 查看建表语句
来源：http://ex.chemitech.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bf.shxzskj.cn

[Q72] 查看索引
来源：http://fi.szsharing.cn

SHOW INDEX FROM users;
来源：http://fc.jianghongdianzi.cn

[Q73] 查看表状态
来源：http://gh.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rm.521024.cn

[Q74] 强制使用索引
来源：http://kn.hnjuh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ip.shtwfgs.cn

[Q75] 日期格式化
来源：http://wp.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://em.shxzskj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qg.newstarts.cn

[Q76] 按天统计
来源：http://kk.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wk.colortex.cn

[Q77] 时间加减
来源：http://xg.521024.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kj.szsharing.cn

[Q78] 当前时间
来源：http://za.shxzskj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pi.shxzskj.cn

[Q79] 字符串拼接
来源：http://ep.shxzskj.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yu.nicolike.cn

[Q80] 字符串截取
来源：http://rn.yuntaijiaju.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fs.haigaiapp.cn

[Q81] 字符串替换
来源：http://cg.yuexingan06.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dy.huixinmuqiang.cn

[Q82] 字符长度与字节长度
来源：http://db.asd995.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ns.jctech888.com.cn

[Q83] 大小写转换
来源：http://nl.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qx.nicolike.cn

[Q84] 去除首尾空格
来源：http://dh.muxihuayi.cn

SELECT TRIM(name) FROM users;
来源：http://cx.asd995.cn

[Q85] 数值取整
来源：http://zu.shxzukj.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ad.521024.cn

[Q86] 读取 JSON 字段
来源：http://bm.szxytkj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vo.bjjhwx.cn

[Q87] JSON 字段做条件
来源：http://ek.hahajie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wd.hnjuh.cn

[Q88] 行转列（条件聚合）
来源：http://ox.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ia.panjiajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nd.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://rk.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cx.yuexingan06.cn

[Q90] 生成序号列
来源：http://lz.521024.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zp.panjiajie.cn

================================================================================
来源：http://he.panjiajie.cn

R. Bash 专题
来源：http://ik.szsharing.cn

================================================================================
来源：http://iw.huixiangedu.cn

[R01] shebang 与严格模式
来源：http://rf.gzmigu.cn

#!/usr/bin/env bash
来源：http://dy.panjiajie.cn

set -euo pipefail
来源：http://fk.nszjky.cn

[R02] 变量赋值与使用
来源：http://bl.jctech888.com.cn

name="Tom"; echo "$name"
来源：http://qy.newstarts.cn

[R03] 只读变量
来源：http://rr.hnjuh.cn

readonly PI=3.14
来源：http://th.szxytkj.cn

[R04] 位置参数
来源：http://tz.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pl.huixiangedu.cn

[R05] 参数默认值
来源：http://pg.shtwfgs.cn

name="${1:-default}"
来源：http://ut.lnxyls.cn

[R06] 判断命令是否存在
来源：http://gw.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xx.huixinmuqiang.cn

[R07] if 判断文件
来源：http://fl.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ym.chemitech.net.cn

[R08] 数值比较
来源：http://ea.asd995.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mk.bookmarksfly.cn

[R09] 字符串比较
来源：http://yw.yuexingan06.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://io.szsharing.cn

[R10] 正则匹配
来源：http://bv.hnjuh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vw.shtwfgs.cn

[R11] case 多分支
来源：http://df.huixinmuqiang.cn

case "$1" in
来源：http://rt.wgjwhj.cn

start) echo "启动" ;;
来源：http://rm.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://rm.bjjhwx.cn

*)     echo "未知命令" ;;
来源：http://xd.newstarts.cn

esac
来源：http://ru.lnxyls.cn

[R12] for 遍历文件
来源：http://in.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://dc.nszjky.cn

[R13] for 计数循环
来源：http://is.hahajie.cn

for i in {1..10}; do echo "$i"; done
来源：http://wn.hahajie.cn

[R14] C 风格 for
来源：http://ti.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dj.shtwfgs.cn

[R15] while 逐行读文件
来源：http://wn.hnjuh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ux.huanxung.cn

[R16] until 等待条件
来源：http://il.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://al.colortex.cn

[R17] 数组定义与取值
来源：http://jr.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pf.nszjky.cn

[R18] 遍历数组
来源：http://wp.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kz.shxzskj.cn

[R19] 数组长度
来源：http://ph.yuntaijiaju.cn

echo "${#arr[@]}"
来源：http://fq.bjjhwx.cn

[R20] 关联数组（字典）
来源：http://yy.9csxet.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jo.jianghongdianzi.cn

[R21] 字符串长度
来源：http://kp.nszjky.cn

echo "${#s}"
来源：http://ed.hahajie.cn

[R22] 截取子串
来源：http://ka.shtwfgs.cn

echo "${s:0:5}"
来源：http://gv.huanxung.cn

[R23] 字符串替换
来源：http://jn.gzmigu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ga.huixinmuqiang.cn

[R24] 大小写转换
来源：http://xa.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lf.wgjwhj.cn

[R25] 去后缀 / 去前缀
来源：http://tq.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ox.nicolike.cn

[R26] 命令替换
来源：http://yd.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://sr.jctech888.com.cn

[R27] 算术展开
来源：http://fa.asd995.cn

echo $((1 + 2 * 3))
来源：http://at.shxzukj.cn

[R28] 浮点运算
来源：http://pq.nicolike.cn

echo "scale=2; 10/3" | bc
来源：http://sc.yuexingan06.cn

[R29] 定义函数
来源：http://hn.asd995.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yv.chemitech.net.cn

[R30] 函数返回状态码
来源：http://ka.huanxung.cn

f() { return 0; }; f || echo "失败了"
来源：http://zh.gzmigu.cn

[R31] 局部变量
来源：http://ua.szxytkj.cn

f() { local x=1; echo "$x"; }
来源：http://dm.gzmigu.cn

[R32] 参数个数校验
来源：http://jd.jctech888.com.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pz.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://yf.newstarts.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ij.shxzskj.cn

[R34] 退出时清理
来源：http://fx.huixiangedu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ob.muxihuayi.cn

[R35] 后台执行并等待
来源：http://ak.huixiangedu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zc.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://ig.jctech888.com.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xp.hahajie.cn

[R37] 把输出赋给变量
来源：http://ar.nicolike.cn

files=$(ls -1)
来源：http://sv.yuntaijiaju.cn

[R38] 管道串联
来源：http://ne.nicolike.cn

cat a.txt | grep -i error | wc -l
来源：http://kr.colortex.cn

[R39] 重定向标准输出与错误
来源：http://ke.haigaiapp.cn

cmd > out.log 2>&1
来源：http://hb.yuexingan06.cn

[R40] 追加写日志
来源：http://ud.szxytkj.cn

echo "log" >> out.log
来源：http://pa.asd995.cn

[R41] 丢弃输出
来源：http://tx.jianghongdianzi.cn

cmd >/dev/null 2>&1
来源：http://oe.hahajie.cn

[R42] 输入重定向
来源：http://kt.asd995.cn

wc -l < a.txt
来源：http://mq.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://di.521024.cn

find . -name "*.log" -type f
来源：http://zy.wgjwhj.cn

[R44] 按修改时间查找
来源：http://fk.colortex.cn

find . -mtime -7 -type f
来源：http://gg.szsharing.cn

[R45] 批量删除
来源：http://lq.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://zk.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://kh.bookmarksfly.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hr.shtwfgs.cn

[R47] sed 单行替换
来源：http://on.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uk.asd995.cn

[R48] awk 取指定列
来源：http://te.yuexingan06.cn

awk '{print $1, $3}' a.txt
来源：http://ps.521024.cn

[R49] awk 带条件
来源：http://vo.szsharing.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qr.shtwfgs.cn

[R50] awk 求和
来源：http://rf.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yt.szsharing.cn

[R51] 排序去重取前几
来源：http://uc.jctech888.com.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qf.521024.cn

[R52] 统计行数
来源：http://jd.shtwfgs.cn

wc -l a.txt
来源：http://tg.colortex.cn

[R53] 查看文件头与实时尾
来源：http://pd.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wt.gzmigu.cn

[R54] 比较两个文件
来源：http://na.lnxyls.cn

diff a.txt b.txt
来源：http://vk.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://pv.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xn.panjiajie.cn

[R56] 远程拷贝
来源：http://zg.bookmarksfly.cn

scp file user@host:/path/
来源：http://ot.shxzskj.cn

[R57] 远程执行命令
来源：http://fw.newstarts.cn

ssh user@host 'uptime'
来源：http://rq.9csxet.cn

[R58] 下载文件
来源：http://jj.bookmarksfly.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ve.huixiangedu.cn

[R59] 发 POST JSON
来源：http://uf.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bv.hnjuh.cn

[R60] 只看 HTTP 状态码
来源：http://up.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jx.jctech888.com.cn

[R61] 磁盘占用
来源：http://ty.yuntaijiaju.cn

df -h;  du -sh *
来源：http://kc.shxzukj.cn

[R62] 找最占空间的文件
来源：http://dv.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ew.chemitech.net.cn

[R63] 内存与进程
来源：http://dk.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://bz.asd995.cn

[R64] 结束进程
来源：http://yy.wgjwhj.cn

kill -9 $(pgrep -f app.py)
来源：http://vs.9csxet.cn

[R65] 查看端口占用
来源：http://mw.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ko.jctech888.com.cn

[R66] 定时任务
来源：http://xg.colortex.cn

crontab -e;  crontab -l
来源：http://am.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://li.gzmigu.cn

openssl rand -hex 16
来源：http://nc.521024.cn

[R68] 计算文件校验值
来源：http://mr.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pz.huanxung.cn

[R69] 生成随机密码
来源：http://bb.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://lb.9csxet.cn

[R70] 时间戳与互转
来源：http://ab.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://ue.jctech888.com.cn

[R71] 日期格式化
来源：http://qs.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vc.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://vc.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sw.haigaiapp.cn

[R73] 分割大日志
来源：http://pv.9csxet.cn

split -l 1000 big.log part_
来源：http://jg.huixinmuqiang.cn

[R74] 批量重命名
来源：http://tw.huixiangedu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xw.asd995.cn

[R75] 导出环境变量
来源：http://dj.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://sx.bookmarksfly.cn

[R76] 使用临时文件
来源：http://pt.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://so.szsharing.cn

[R77] 读取用户输入
来源：http://jq.huanxung.cn

read -rp "请输入: " ans
来源：http://bl.asd995.cn

[R78] 交互式菜单
来源：http://of.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://to.muxihuayi.cn

[R79] 解析命令行选项
来源：http://cq.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nv.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://nl.bjjhwx.cn

time ./run.sh
来源：http://lu.nszjky.cn

================================================================================
来源：http://oa.hnjuh.cn

S. C / C++ 专题
来源：http://hp.wgjwhj.cn

================================================================================
来源：http://qj.newstarts.cn

[S01] C：Hello World
来源：http://eu.bookmarksfly.cn

#include <stdio.h>
来源：http://jl.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ac.nszjky.cn

[S02] C：变量与格式化输出
来源：http://xu.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ry.jianghongdianzi.cn

[S03] C：读入整数
来源：http://lc.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://ue.bookmarksfly.cn

[S04] C：字符串复制
来源：http://nb.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ah.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://zv.bjjhwx.cn

strlen(s)
来源：http://te.bjjhwx.cn

[S06] C：字符串比较
来源：http://xk.szxytkj.cn

strcmp(a, b) == 0
来源：http://pk.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://de.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ox.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://kz.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tn.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://cz.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qd.colortex.cn

[S10] C：指针与解引用
来源：http://bp.nicolike.cn

int *p = &a;  *p = 5;
来源：http://rh.shxzskj.cn

[S11] C：逐行读文件
来源：http://xy.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://gr.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hs.haigaiapp.cn

fclose(f);
来源：http://vp.szsharing.cn

[S12] C：写文件
来源：http://ld.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yf.newstarts.cn

[S13] C：宏定义
来源：http://pv.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fj.yuntaijiaju.cn

[S14] C：枚举
来源：http://ou.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://vd.hnjuh.cn

[S15] C：类型转换
来源：http://ko.9csxet.cn

(double) a / b
来源：http://ly.szxytkj.cn

[S16] C：位操作置位
来源：http://ht.hahajie.cn

x |= (1 << 3);
来源：http://gx.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://ed.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vo.nicolike.cn

[S18] C：命令行参数
来源：http://lh.colortex.cn

int main(int argc, char **argv)
来源：http://va.yuexingan06.cn

[S19] C：快速排序
来源：http://ek.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ur.szxytkj.cn

[S20] C：二分查找
来源：http://fl.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gc.nszjky.cn

[S21] C：字符类别判断
来源：http://bj.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mz.muxihuayi.cn

[S22] C：字符串转数字
来源：http://vg.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hs.gzmigu.cn

[S23] C：随机数
来源：http://lb.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yr.wgjwhj.cn

[S24] C：获取本地时间
来源：http://pq.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bu.muxihuayi.cn

[S25] C：内存拷贝
来源：http://sf.521024.cn

memcpy(dst, src, n);
来源：http://em.bjjhwx.cn

[S26] C：内存清零
来源：http://ps.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://hc.yuntaijiaju.cn

[S27] C：定义常量
来源：http://fv.jctech888.com.cn

const double PI = 3.14159;
来源：http://te.shxzskj.cn

[S28] C：静态变量
来源：http://gt.bookmarksfly.cn

static int counter = 0;
来源：http://uo.521024.cn

[S29] C：变参函数
来源：http://pf.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tz.jctech888.com.cn

[S30] C：头文件保护
来源：http://cu.shtwfgs.cn

#ifndef X_H
来源：http://xg.nicolike.cn

#define X_H
来源：http://uy.bookmarksfly.cn

#endif
来源：http://sm.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://ft.muxihuayi.cn

#include <iostream>
来源：http://re.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://nb.shxzskj.cn

[S32] C++：字符串
来源：http://oz.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://tu.huixiangedu.cn

[S33] C++：vector 增删
来源：http://qg.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://by.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://cm.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://yv.muxihuayi.cn

[S35] C++：map
来源：http://tc.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mf.muxihuayi.cn

[S36] C++：unordered_map
来源：http://eb.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://du.bjjhwx.cn

[S37] C++：set
来源：http://dj.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kp.szxytkj.cn

[S38] C++：排序
来源：http://mu.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ou.jctech888.com.cn


<!-- 参考信息 -->