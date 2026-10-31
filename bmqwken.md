代发 wailian999

ROLLBACK TO sp1;
来源：http://ql.newstarts.cn

[Q69] 查看执行计划
来源：http://pl.bookmarksfly.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pn.lnxyls.cn

[Q70] 更新统计信息
来源：http://wq.szsharing.cn

ANALYZE TABLE users;
来源：http://we.jianghongdianzi.cn

[Q71] 查看建表语句
来源：http://kb.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nd.yuexingan06.cn

[Q72] 查看索引
来源：http://sf.nicolike.cn

SHOW INDEX FROM users;
来源：http://dq.9csxet.cn

[Q73] 查看表状态
来源：http://jn.gzmigu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bh.nszjky.cn

[Q74] 强制使用索引
来源：http://tm.haigaiapp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xn.lnxyls.cn

[Q75] 日期格式化
来源：http://ef.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ed.asd995.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vl.haigaiapp.cn

[Q76] 按天统计
来源：http://ab.panjiajie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xp.jianghongdianzi.cn

[Q77] 时间加减
来源：http://wj.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://no.muxihuayi.cn

[Q78] 当前时间
来源：http://oe.nicolike.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kp.panjiajie.cn

[Q79] 字符串拼接
来源：http://qa.hahajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wu.shxzskj.cn

[Q80] 字符串截取
来源：http://je.szsharing.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ik.asd995.cn

[Q81] 字符串替换
来源：http://iz.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bd.bookmarksfly.cn

[Q82] 字符长度与字节长度
来源：http://hd.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cy.chemitech.net.cn

[Q83] 大小写转换
来源：http://ig.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ol.lnxyls.cn

[Q84] 去除首尾空格
来源：http://ck.bjjhwx.cn

SELECT TRIM(name) FROM users;
来源：http://el.bjjhwx.cn

[Q85] 数值取整
来源：http://mv.yuexingan06.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vv.huixinmuqiang.cn

[Q86] 读取 JSON 字段
来源：http://ut.bjjhwx.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xe.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://eo.szsharing.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mf.nicolike.cn

[Q88] 行转列（条件聚合）
来源：http://tn.huanxung.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pv.huixiangedu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://em.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://mi.gzmigu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yc.jianghongdianzi.cn

[Q90] 生成序号列
来源：http://ev.shxzukj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dt.yuexingan06.cn

================================================================================
来源：http://as.shtwfgs.cn

R. Bash 专题
来源：http://mq.bookmarksfly.cn

================================================================================
来源：http://sy.shxzskj.cn

[R01] shebang 与严格模式
来源：http://cj.jctech888.com.cn

#!/usr/bin/env bash
来源：http://xl.nszjky.cn

set -euo pipefail
来源：http://zj.nszjky.cn

[R02] 变量赋值与使用
来源：http://op.521024.cn

name="Tom"; echo "$name"
来源：http://xl.yuntaijiaju.cn

[R03] 只读变量
来源：http://af.shtwfgs.cn

readonly PI=3.14
来源：http://co.bjjhwx.cn

[R04] 位置参数
来源：http://pi.yuntaijiaju.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ld.huixiangedu.cn

[R05] 参数默认值
来源：http://im.nicolike.cn

name="${1:-default}"
来源：http://nh.newstarts.cn

[R06] 判断命令是否存在
来源：http://fa.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nl.shtwfgs.cn

[R07] if 判断文件
来源：http://rd.szsharing.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ze.jctech888.com.cn

[R08] 数值比较
来源：http://ii.haigaiapp.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hm.bookmarksfly.cn

[R09] 字符串比较
来源：http://fw.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hm.chemitech.net.cn

[R10] 正则匹配
来源：http://nc.shxzskj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://io.shxzukj.cn

[R11] case 多分支
来源：http://sk.yuntaijiaju.cn

case "$1" in
来源：http://fp.hnjuh.cn

start) echo "启动" ;;
来源：http://kl.muxihuayi.cn

stop)  echo "停止" ;;
来源：http://bx.huanxung.cn

*)     echo "未知命令" ;;
来源：http://rf.9csxet.cn

esac
来源：http://hp.wgjwhj.cn

[R12] for 遍历文件
来源：http://cs.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://jf.yuexingan06.cn

[R13] for 计数循环
来源：http://jw.shtwfgs.cn

for i in {1..10}; do echo "$i"; done
来源：http://sh.shxzskj.cn

[R14] C 风格 for
来源：http://co.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xx.521024.cn

[R15] while 逐行读文件
来源：http://xs.muxihuayi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ay.panjiajie.cn

[R16] until 等待条件
来源：http://xw.jctech888.com.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lt.521024.cn

[R17] 数组定义与取值
来源：http://vs.wgjwhj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kd.nicolike.cn

[R18] 遍历数组
来源：http://ww.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tf.gzmigu.cn

[R19] 数组长度
来源：http://ys.colortex.cn

echo "${#arr[@]}"
来源：http://am.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://aq.huixinmuqiang.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lz.shtwfgs.cn

[R21] 字符串长度
来源：http://no.shtwfgs.cn

echo "${#s}"
来源：http://uc.yuexingan06.cn

[R22] 截取子串
来源：http://dz.shxzskj.cn

echo "${s:0:5}"
来源：http://ii.hahajie.cn

[R23] 字符串替换
来源：http://jg.panjiajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ep.colortex.cn

[R24] 大小写转换
来源：http://zl.gzmigu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ps.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://oq.shtwfgs.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ic.jctech888.com.cn

[R26] 命令替换
来源：http://ex.huanxung.cn

now=$(date +%F); echo "$now"
来源：http://vg.szxytkj.cn

[R27] 算术展开
来源：http://fo.shxzukj.cn

echo $((1 + 2 * 3))
来源：http://xz.yuexingan06.cn

[R28] 浮点运算
来源：http://uw.nszjky.cn

echo "scale=2; 10/3" | bc
来源：http://pr.521024.cn

[R29] 定义函数
来源：http://jl.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mw.9csxet.cn

[R30] 函数返回状态码
来源：http://lp.nicolike.cn

f() { return 0; }; f || echo "失败了"
来源：http://dl.newstarts.cn

[R31] 局部变量
来源：http://nx.colortex.cn

f() { local x=1; echo "$x"; }
来源：http://jj.lnxyls.cn

[R32] 参数个数校验
来源：http://pl.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pa.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://qg.colortex.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wd.huixinmuqiang.cn

[R34] 退出时清理
来源：http://td.huixinmuqiang.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zm.hahajie.cn

[R35] 后台执行并等待
来源：http://yh.haigaiapp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ow.lnxyls.cn

[R36] 并发执行多个任务
来源：http://ko.hnjuh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://au.szsharing.cn

[R37] 把输出赋给变量
来源：http://tp.huixiangedu.cn

files=$(ls -1)
来源：http://lx.chemitech.net.cn

[R38] 管道串联
来源：http://hl.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://ip.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://ko.szxytkj.cn

cmd > out.log 2>&1
来源：http://lt.hnjuh.cn

[R40] 追加写日志
来源：http://tz.haigaiapp.cn

echo "log" >> out.log
来源：http://se.shxzukj.cn

[R41] 丢弃输出
来源：http://tq.shxzukj.cn

cmd >/dev/null 2>&1
来源：http://qa.bookmarksfly.cn

[R42] 输入重定向
来源：http://iy.huixiangedu.cn

wc -l < a.txt
来源：http://rd.shtwfgs.cn

[R43] 按名字查找文件
来源：http://sd.9csxet.cn

find . -name "*.log" -type f
来源：http://ox.wgjwhj.cn

[R44] 按修改时间查找
来源：http://wr.bookmarksfly.cn

find . -mtime -7 -type f
来源：http://eg.lnxyls.cn

[R45] 批量删除
来源：http://cu.521024.cn

find . -name "*.tmp" -delete
来源：http://cz.muxihuayi.cn

[R46] 递归替换文件内容
来源：http://sk.huanxung.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://me.521024.cn

[R47] sed 单行替换
来源：http://au.bjjhwx.cn

sed -i 's/foo/bar/g' a.txt
来源：http://we.huanxung.cn

[R48] awk 取指定列
来源：http://fv.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://ui.jianghongdianzi.cn

[R49] awk 带条件
来源：http://hh.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qo.wgjwhj.cn

[R50] awk 求和
来源：http://yu.panjiajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nw.yuexingan06.cn

[R51] 排序去重取前几
来源：http://bz.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bn.nszjky.cn

[R52] 统计行数
来源：http://cz.muxihuayi.cn

wc -l a.txt
来源：http://nj.asd995.cn

[R53] 查看文件头与实时尾
来源：http://vp.chemitech.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zb.newstarts.cn

[R54] 比较两个文件
来源：http://ft.panjiajie.cn

diff a.txt b.txt
来源：http://bv.bjjhwx.cn

[R55] 压缩与解压
来源：http://px.asd995.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uv.9csxet.cn

[R56] 远程拷贝
来源：http://ka.gzmigu.cn

scp file user@host:/path/
来源：http://ns.shxzukj.cn

[R57] 远程执行命令
来源：http://vb.panjiajie.cn

ssh user@host 'uptime'
来源：http://ol.yuntaijiaju.cn

[R58] 下载文件
来源：http://pd.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wy.9csxet.cn

[R59] 发 POST JSON
来源：http://by.newstarts.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yy.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://ha.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sk.haigaiapp.cn

[R61] 磁盘占用
来源：http://vp.colortex.cn

df -h;  du -sh *
来源：http://ww.hnjuh.cn

[R62] 找最占空间的文件
来源：http://gh.chemitech.net.cn

du -ah . | sort -rh | head -10
来源：http://hr.huixiangedu.cn

[R63] 内存与进程
来源：http://qt.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://zy.lnxyls.cn

[R64] 结束进程
来源：http://mx.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://jd.521024.cn

[R65] 查看端口占用
来源：http://zb.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ad.yuntaijiaju.cn

[R66] 定时任务
来源：http://tc.nicolike.cn

crontab -e;  crontab -l
来源：http://pf.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://em.yuntaijiaju.cn

openssl rand -hex 16
来源：http://pm.szxytkj.cn

[R68] 计算文件校验值
来源：http://oc.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vm.hahajie.cn

[R69] 生成随机密码
来源：http://ap.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://zb.521024.cn

[R70] 时间戳与互转
来源：http://yw.newstarts.cn

date +%s;  date -d @1700000000
来源：http://yi.bjjhwx.cn

[R71] 日期格式化
来源：http://db.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qa.hahajie.cn

[R72] 等待端口就绪
来源：http://pr.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mi.yuexingan06.cn

[R73] 分割大日志
来源：http://yk.huixiangedu.cn

split -l 1000 big.log part_
来源：http://bd.szxytkj.cn

[R74] 批量重命名
来源：http://ml.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ae.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ti.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://sa.lnxyls.cn

[R76] 使用临时文件
来源：http://cx.newstarts.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gu.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://zy.huanxung.cn

read -rp "请输入: " ans
来源：http://uu.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://bo.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jh.colortex.cn

[R79] 解析命令行选项
来源：http://ck.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ve.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://di.shtwfgs.cn

time ./run.sh
来源：http://rf.yuexingan06.cn

================================================================================
来源：http://cq.wgjwhj.cn

S. C / C++ 专题
来源：http://bg.gzmigu.cn

================================================================================
来源：http://rs.yuexingan06.cn

[S01] C：Hello World
来源：http://pa.jctech888.com.cn

#include <stdio.h>
来源：http://dd.hnjuh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pf.colortex.cn

[S02] C：变量与格式化输出
来源：http://ee.shxzskj.cn

int a = 10; printf("%d\n", a);
来源：http://zu.szsharing.cn

[S03] C：读入整数
来源：http://ig.hahajie.cn

int x; scanf("%d", &x);
来源：http://qv.lnxyls.cn

[S04] C：字符串复制
来源：http://dn.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ub.nszjky.cn

[S05] C：字符串长度
来源：http://vn.haigaiapp.cn

strlen(s)
来源：http://yu.huanxung.cn

[S06] C：字符串比较
来源：http://vk.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://tg.gzmigu.cn

[S07] C：数组遍历求和
来源：http://yi.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zz.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://no.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zx.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://th.jianghongdianzi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lw.shxzukj.cn

[S10] C：指针与解引用
来源：http://ab.jctech888.com.cn

int *p = &a;  *p = 5;
来源：http://gu.newstarts.cn

[S11] C：逐行读文件
来源：http://as.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ey.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ju.asd995.cn

fclose(f);
来源：http://dj.shxzukj.cn

[S12] C：写文件
来源：http://wr.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://na.shxzukj.cn

[S13] C：宏定义
来源：http://bs.panjiajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wc.hahajie.cn

[S14] C：枚举
来源：http://rj.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://zz.gzmigu.cn

[S15] C：类型转换
来源：http://km.haigaiapp.cn

(double) a / b
来源：http://ra.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ae.nicolike.cn

x |= (1 << 3);
来源：http://vv.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://fq.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://di.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://nm.huixiangedu.cn

int main(int argc, char **argv)
来源：http://ba.521024.cn

[S19] C：快速排序
来源：http://os.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ha.yuntaijiaju.cn

[S20] C：二分查找
来源：http://kc.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lm.9csxet.cn

[S21] C：字符类别判断
来源：http://ch.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gl.hnjuh.cn

[S22] C：字符串转数字
来源：http://wg.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ni.shtwfgs.cn

[S23] C：随机数
来源：http://ws.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ae.panjiajie.cn

[S24] C：获取本地时间
来源：http://wj.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lg.newstarts.cn

[S25] C：内存拷贝
来源：http://ta.521024.cn

memcpy(dst, src, n);
来源：http://og.huixiangedu.cn

[S26] C：内存清零
来源：http://it.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://sq.jianghongdianzi.cn

[S27] C：定义常量
来源：http://yc.shxzskj.cn

const double PI = 3.14159;
来源：http://lo.yuntaijiaju.cn

[S28] C：静态变量
来源：http://xx.chemitech.net.cn

static int counter = 0;
来源：http://bf.nicolike.cn

[S29] C：变参函数
来源：http://je.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rb.huixiangedu.cn

[S30] C：头文件保护
来源：http://pw.shxzskj.cn

#ifndef X_H
来源：http://qs.bjjhwx.cn

#define X_H
来源：http://wa.hnjuh.cn

#endif
来源：http://zh.chemitech.net.cn

[S31] C++：Hello World
来源：http://ov.shxzskj.cn

#include <iostream>
来源：http://kj.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://sf.huanxung.cn

[S32] C++：字符串
来源：http://xl.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://xs.521024.cn

[S33] C++：vector 增删
来源：http://gv.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vr.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://sc.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://mr.huanxung.cn

[S35] C++：map
来源：http://tp.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://di.9csxet.cn

[S36] C++：unordered_map
来源：http://in.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pv.bookmarksfly.cn

[S37] C++：set
来源：http://mi.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://th.asd995.cn

[S38] C++：排序
来源：http://oq.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://sp.yuntaijiaju.cn


<!-- 参考信息 -->