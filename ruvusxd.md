代发 wailian999

ROLLBACK TO sp1;
来源：http://qi.bjjhwx.cn

[Q69] 查看执行计划
来源：http://hi.jianghongdianzi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tx.shxzskj.cn

[Q70] 更新统计信息
来源：http://tq.bjjhwx.cn

ANALYZE TABLE users;
来源：http://cw.huixinmuqiang.cn

[Q71] 查看建表语句
来源：http://gu.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://my.hnjuh.cn

[Q72] 查看索引
来源：http://sv.shxzukj.cn

SHOW INDEX FROM users;
来源：http://dk.hnjuh.cn

[Q73] 查看表状态
来源：http://ei.521024.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fw.chemitech.net.cn

[Q74] 强制使用索引
来源：http://qo.jianghongdianzi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mv.nicolike.cn

[Q75] 日期格式化
来源：http://hg.bjjhwx.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fl.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ge.gzmigu.cn

[Q76] 按天统计
来源：http://ao.shxzukj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zp.nicolike.cn

[Q77] 时间加减
来源：http://wa.hahajie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qa.nicolike.cn

[Q78] 当前时间
来源：http://ho.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cg.gzmigu.cn

[Q79] 字符串拼接
来源：http://he.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fv.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://pa.jianghongdianzi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://of.hnjuh.cn

[Q81] 字符串替换
来源：http://jz.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vu.shxzskj.cn

[Q82] 字符长度与字节长度
来源：http://aj.shxzskj.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sf.asd995.cn

[Q83] 大小写转换
来源：http://jf.9csxet.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://va.nszjky.cn

[Q84] 去除首尾空格
来源：http://ix.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://wd.lnxyls.cn

[Q85] 数值取整
来源：http://qd.bjjhwx.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fb.jctech888.com.cn

[Q86] 读取 JSON 字段
来源：http://ey.haigaiapp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qw.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://kz.haigaiapp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lf.lnxyls.cn

[Q88] 行转列（条件聚合）
来源：http://yr.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://am.hahajie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uc.hnjuh.cn

[Q89] 判断表是否存在
来源：http://rs.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hv.szxytkj.cn

[Q90] 生成序号列
来源：http://oy.colortex.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oo.jctech888.com.cn

================================================================================
来源：http://nl.nicolike.cn

R. Bash 专题
来源：http://ci.asd995.cn

================================================================================
来源：http://wt.szxytkj.cn

[R01] shebang 与严格模式
来源：http://wk.jctech888.com.cn

#!/usr/bin/env bash
来源：http://xh.yuexingan06.cn

set -euo pipefail
来源：http://gc.panjiajie.cn

[R02] 变量赋值与使用
来源：http://if.szsharing.cn

name="Tom"; echo "$name"
来源：http://na.yuntaijiaju.cn

[R03] 只读变量
来源：http://cp.9csxet.cn

readonly PI=3.14
来源：http://jk.chemitech.net.cn

[R04] 位置参数
来源：http://fq.huixiangedu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ut.521024.cn

[R05] 参数默认值
来源：http://bi.yuntaijiaju.cn

name="${1:-default}"
来源：http://au.nicolike.cn

[R06] 判断命令是否存在
来源：http://vg.panjiajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nw.chemitech.net.cn

[R07] if 判断文件
来源：http://fa.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pd.jctech888.com.cn

[R08] 数值比较
来源：http://wr.colortex.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ey.newstarts.cn

[R09] 字符串比较
来源：http://ro.hahajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://te.szsharing.cn

[R10] 正则匹配
来源：http://ew.panjiajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://do.bjjhwx.cn

[R11] case 多分支
来源：http://vo.huanxung.cn

case "$1" in
来源：http://nw.lnxyls.cn

start) echo "启动" ;;
来源：http://xn.gzmigu.cn

stop)  echo "停止" ;;
来源：http://mc.9csxet.cn

*)     echo "未知命令" ;;
来源：http://hb.jctech888.com.cn

esac
来源：http://de.nicolike.cn

[R12] for 遍历文件
来源：http://mj.huixiangedu.cn

for f in *.txt; do echo "$f"; done
来源：http://wc.huanxung.cn

[R13] for 计数循环
来源：http://hu.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ug.shxzskj.cn

[R14] C 风格 for
来源：http://tg.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dg.jianghongdianzi.cn

[R15] while 逐行读文件
来源：http://ii.huixinmuqiang.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zd.shxzukj.cn

[R16] until 等待条件
来源：http://ru.lnxyls.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ox.panjiajie.cn

[R17] 数组定义与取值
来源：http://ln.muxihuayi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fy.nszjky.cn

[R18] 遍历数组
来源：http://uk.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://id.asd995.cn

[R19] 数组长度
来源：http://dl.9csxet.cn

echo "${#arr[@]}"
来源：http://my.lnxyls.cn

[R20] 关联数组（字典）
来源：http://bm.yuntaijiaju.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cp.huixinmuqiang.cn

[R21] 字符串长度
来源：http://lb.wgjwhj.cn

echo "${#s}"
来源：http://cg.shxzskj.cn

[R22] 截取子串
来源：http://bp.chemitech.net.cn

echo "${s:0:5}"
来源：http://rj.huixinmuqiang.cn

[R23] 字符串替换
来源：http://cm.newstarts.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dd.panjiajie.cn

[R24] 大小写转换
来源：http://io.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://es.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://dx.colortex.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wi.huanxung.cn

[R26] 命令替换
来源：http://zl.chemitech.net.cn

now=$(date +%F); echo "$now"
来源：http://lq.nicolike.cn

[R27] 算术展开
来源：http://ok.haigaiapp.cn

echo $((1 + 2 * 3))
来源：http://yx.asd995.cn

[R28] 浮点运算
来源：http://dm.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://mh.shtwfgs.cn

[R29] 定义函数
来源：http://bn.chemitech.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ge.hnjuh.cn

[R30] 函数返回状态码
来源：http://de.haigaiapp.cn

f() { return 0; }; f || echo "失败了"
来源：http://wi.muxihuayi.cn

[R31] 局部变量
来源：http://le.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://az.yuntaijiaju.cn

[R32] 参数个数校验
来源：http://kl.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rs.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://yr.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cq.huixiangedu.cn

[R34] 退出时清理
来源：http://xr.nicolike.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fl.newstarts.cn

[R35] 后台执行并等待
来源：http://ls.yuntaijiaju.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rp.hnjuh.cn

[R36] 并发执行多个任务
来源：http://yv.panjiajie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qh.gzmigu.cn

[R37] 把输出赋给变量
来源：http://kc.huixinmuqiang.cn

files=$(ls -1)
来源：http://yb.jctech888.com.cn

[R38] 管道串联
来源：http://hl.nszjky.cn

cat a.txt | grep -i error | wc -l
来源：http://ea.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://fh.521024.cn

cmd > out.log 2>&1
来源：http://gf.panjiajie.cn

[R40] 追加写日志
来源：http://wg.shxzukj.cn

echo "log" >> out.log
来源：http://ne.asd995.cn

[R41] 丢弃输出
来源：http://zv.asd995.cn

cmd >/dev/null 2>&1
来源：http://ip.hnjuh.cn

[R42] 输入重定向
来源：http://nh.nszjky.cn

wc -l < a.txt
来源：http://qt.szsharing.cn

[R43] 按名字查找文件
来源：http://pf.yuexingan06.cn

find . -name "*.log" -type f
来源：http://bg.hnjuh.cn

[R44] 按修改时间查找
来源：http://oj.bjjhwx.cn

find . -mtime -7 -type f
来源：http://ec.lnxyls.cn

[R45] 批量删除
来源：http://jb.wgjwhj.cn

find . -name "*.tmp" -delete
来源：http://es.lnxyls.cn

[R46] 递归替换文件内容
来源：http://yl.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dx.panjiajie.cn

[R47] sed 单行替换
来源：http://mp.521024.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rj.shxzskj.cn

[R48] awk 取指定列
来源：http://li.huixiangedu.cn

awk '{print $1, $3}' a.txt
来源：http://vt.newstarts.cn

[R49] awk 带条件
来源：http://ez.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yu.muxihuayi.cn

[R50] awk 求和
来源：http://bk.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://en.muxihuayi.cn

[R51] 排序去重取前几
来源：http://pb.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oa.shxzukj.cn

[R52] 统计行数
来源：http://ta.nszjky.cn

wc -l a.txt
来源：http://jk.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://ot.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nj.yuexingan06.cn

[R54] 比较两个文件
来源：http://au.huanxung.cn

diff a.txt b.txt
来源：http://sv.gzmigu.cn

[R55] 压缩与解压
来源：http://vq.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://es.shtwfgs.cn

[R56] 远程拷贝
来源：http://nc.haigaiapp.cn

scp file user@host:/path/
来源：http://oj.newstarts.cn

[R57] 远程执行命令
来源：http://tj.shxzukj.cn

ssh user@host 'uptime'
来源：http://ca.jianghongdianzi.cn

[R58] 下载文件
来源：http://vg.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sf.wgjwhj.cn

[R59] 发 POST JSON
来源：http://pv.nicolike.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dz.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://ou.bjjhwx.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dg.hnjuh.cn

[R61] 磁盘占用
来源：http://je.colortex.cn

df -h;  du -sh *
来源：http://kx.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://jn.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://vw.shxzskj.cn

[R63] 内存与进程
来源：http://hb.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://jc.asd995.cn

[R64] 结束进程
来源：http://ex.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://su.9csxet.cn

[R65] 查看端口占用
来源：http://jl.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ru.colortex.cn

[R66] 定时任务
来源：http://uy.bjjhwx.cn

crontab -e;  crontab -l
来源：http://up.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://bi.9csxet.cn

openssl rand -hex 16
来源：http://nm.nicolike.cn

[R68] 计算文件校验值
来源：http://xt.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qh.bjjhwx.cn

[R69] 生成随机密码
来源：http://mc.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://ue.colortex.cn

[R70] 时间戳与互转
来源：http://ab.521024.cn

date +%s;  date -d @1700000000
来源：http://ja.szxytkj.cn

[R71] 日期格式化
来源：http://tb.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ye.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://av.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kc.gzmigu.cn

[R73] 分割大日志
来源：http://vu.nicolike.cn

split -l 1000 big.log part_
来源：http://lh.newstarts.cn

[R74] 批量重命名
来源：http://fu.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jn.asd995.cn

[R75] 导出环境变量
来源：http://ve.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://xo.szxytkj.cn

[R76] 使用临时文件
来源：http://gj.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eb.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://pr.szsharing.cn

read -rp "请输入: " ans
来源：http://tq.chemitech.net.cn

[R78] 交互式菜单
来源：http://uu.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sx.nicolike.cn

[R79] 解析命令行选项
来源：http://hu.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wl.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://wn.shxzukj.cn

time ./run.sh
来源：http://hl.nszjky.cn

================================================================================
来源：http://sq.hahajie.cn

S. C / C++ 专题
来源：http://fy.chemitech.net.cn

================================================================================
来源：http://jb.9csxet.cn

[S01] C：Hello World
来源：http://wn.bookmarksfly.cn

#include <stdio.h>
来源：http://ie.lnxyls.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rq.9csxet.cn

[S02] C：变量与格式化输出
来源：http://er.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://ci.jianghongdianzi.cn

[S03] C：读入整数
来源：http://wf.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://ef.9csxet.cn

[S04] C：字符串复制
来源：http://kx.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nd.9csxet.cn

[S05] C：字符串长度
来源：http://pr.szxytkj.cn

strlen(s)
来源：http://rz.hnjuh.cn

[S06] C：字符串比较
来源：http://lc.9csxet.cn

strcmp(a, b) == 0
来源：http://yg.asd995.cn

[S07] C：数组遍历求和
来源：http://zx.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ll.nicolike.cn

[S08] C：动态内存分配与释放
来源：http://ct.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cz.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://fn.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ol.yuexingan06.cn

[S10] C：指针与解引用
来源：http://mj.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://ji.hahajie.cn

[S11] C：逐行读文件
来源：http://wu.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://bk.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://by.szxytkj.cn

fclose(f);
来源：http://pa.panjiajie.cn

[S12] C：写文件
来源：http://ur.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lg.newstarts.cn

[S13] C：宏定义
来源：http://rm.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ah.bjjhwx.cn

[S14] C：枚举
来源：http://nn.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://qo.lnxyls.cn

[S15] C：类型转换
来源：http://qu.hnjuh.cn

(double) a / b
来源：http://mz.haigaiapp.cn

[S16] C：位操作置位
来源：http://xz.szxytkj.cn

x |= (1 << 3);
来源：http://tb.nicolike.cn

[S17] C：安全拼接字符串
来源：http://pm.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qt.yuexingan06.cn

[S18] C：命令行参数
来源：http://aa.huixiangedu.cn

int main(int argc, char **argv)
来源：http://hn.shxzskj.cn

[S19] C：快速排序
来源：http://hz.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fz.wgjwhj.cn

[S20] C：二分查找
来源：http://so.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wh.bjjhwx.cn

[S21] C：字符类别判断
来源：http://bb.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ta.szsharing.cn

[S22] C：字符串转数字
来源：http://es.szsharing.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sa.shxzskj.cn

[S23] C：随机数
来源：http://mi.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bb.shxzukj.cn

[S24] C：获取本地时间
来源：http://fi.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ey.shtwfgs.cn

[S25] C：内存拷贝
来源：http://qk.hahajie.cn

memcpy(dst, src, n);
来源：http://qe.nszjky.cn

[S26] C：内存清零
来源：http://yr.nicolike.cn

memset(a, 0, sizeof a);
来源：http://tr.chemitech.net.cn

[S27] C：定义常量
来源：http://co.jctech888.com.cn

const double PI = 3.14159;
来源：http://ip.colortex.cn

[S28] C：静态变量
来源：http://hv.jctech888.com.cn

static int counter = 0;
来源：http://xz.newstarts.cn

[S29] C：变参函数
来源：http://ma.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dk.chemitech.net.cn

[S30] C：头文件保护
来源：http://ab.lnxyls.cn

#ifndef X_H
来源：http://gv.huixiangedu.cn

#define X_H
来源：http://yz.wgjwhj.cn

#endif
来源：http://sd.hnjuh.cn

[S31] C++：Hello World
来源：http://ke.yuexingan06.cn

#include <iostream>
来源：http://ur.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://cd.huixiangedu.cn

[S32] C++：字符串
来源：http://ke.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://ha.yuexingan06.cn

[S33] C++：vector 增删
来源：http://vp.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ao.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://ne.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://bx.gzmigu.cn

[S35] C++：map
来源：http://zn.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tj.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://in.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bw.shxzskj.cn

[S37] C++：set
来源：http://mm.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hr.asd995.cn

[S38] C++：排序
来源：http://sm.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ye.szsharing.cn


<!-- 参考信息 -->