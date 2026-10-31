代发 wailian999

[Q67] 设置隔离级别
来源：http://xd.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zt.asd995.cn

[Q68] 保存点
来源：http://dc.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://xu.newstarts.cn

ROLLBACK TO sp1;
来源：http://mp.huixiangedu.cn

[Q69] 查看执行计划
来源：http://pl.shtwfgs.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lt.shtwfgs.cn

[Q70] 更新统计信息
来源：http://mb.colortex.cn

ANALYZE TABLE users;
来源：http://zn.nicolike.cn

[Q71] 查看建表语句
来源：http://vv.wgjwhj.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ck.bjjhwx.cn

[Q72] 查看索引
来源：http://jg.jctech888.com.cn

SHOW INDEX FROM users;
来源：http://yr.colortex.cn

[Q73] 查看表状态
来源：http://fm.bookmarksfly.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ar.hnjuh.cn

[Q74] 强制使用索引
来源：http://ql.huixiangedu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pi.521024.cn

[Q75] 日期格式化
来源：http://jt.shxzukj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ix.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vf.9csxet.cn

[Q76] 按天统计
来源：http://oe.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fd.szsharing.cn

[Q77] 时间加减
来源：http://nn.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pz.nicolike.cn

[Q78] 当前时间
来源：http://rc.colortex.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cw.hahajie.cn

[Q79] 字符串拼接
来源：http://bf.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dx.hahajie.cn

[Q80] 字符串截取
来源：http://nn.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qj.jianghongdianzi.cn

[Q81] 字符串替换
来源：http://ek.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zq.haigaiapp.cn

[Q82] 字符长度与字节长度
来源：http://dm.jctech888.com.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pv.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://vd.jctech888.com.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://em.lnxyls.cn

[Q84] 去除首尾空格
来源：http://wt.jianghongdianzi.cn

SELECT TRIM(name) FROM users;
来源：http://mo.bjjhwx.cn

[Q85] 数值取整
来源：http://xq.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pv.szxytkj.cn

[Q86] 读取 JSON 字段
来源：http://xx.panjiajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jm.asd995.cn

[Q87] JSON 字段做条件
来源：http://nw.9csxet.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pt.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://by.shxzskj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sh.bjjhwx.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nh.521024.cn

[Q89] 判断表是否存在
来源：http://gg.haigaiapp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dn.nicolike.cn

[Q90] 生成序号列
来源：http://sd.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jn.szsharing.cn

================================================================================
来源：http://ds.521024.cn

R. Bash 专题
来源：http://yu.shxzskj.cn

================================================================================
来源：http://va.asd995.cn

[R01] shebang 与严格模式
来源：http://og.muxihuayi.cn

#!/usr/bin/env bash
来源：http://er.shtwfgs.cn

set -euo pipefail
来源：http://rb.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://xo.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://tb.yuexingan06.cn

[R03] 只读变量
来源：http://oe.haigaiapp.cn

readonly PI=3.14
来源：http://yv.shtwfgs.cn

[R04] 位置参数
来源：http://xc.colortex.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ci.shtwfgs.cn

[R05] 参数默认值
来源：http://cq.szsharing.cn

name="${1:-default}"
来源：http://yf.hnjuh.cn

[R06] 判断命令是否存在
来源：http://yu.wgjwhj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lz.colortex.cn

[R07] if 判断文件
来源：http://sy.nicolike.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ut.nicolike.cn

[R08] 数值比较
来源：http://re.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sr.521024.cn

[R09] 字符串比较
来源：http://qg.colortex.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ui.shxzskj.cn

[R10] 正则匹配
来源：http://jw.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ix.huanxung.cn

[R11] case 多分支
来源：http://to.huixinmuqiang.cn

case "$1" in
来源：http://hz.9csxet.cn

start) echo "启动" ;;
来源：http://jk.jianghongdianzi.cn

stop)  echo "停止" ;;
来源：http://ea.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://he.yuntaijiaju.cn

esac
来源：http://zs.colortex.cn

[R12] for 遍历文件
来源：http://vc.521024.cn

for f in *.txt; do echo "$f"; done
来源：http://rb.huanxung.cn

[R13] for 计数循环
来源：http://dg.gzmigu.cn

for i in {1..10}; do echo "$i"; done
来源：http://dk.nicolike.cn

[R14] C 风格 for
来源：http://yg.521024.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jw.bookmarksfly.cn

[R15] while 逐行读文件
来源：http://wo.chemitech.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oq.huixiangedu.cn

[R16] until 等待条件
来源：http://za.huixiangedu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iw.nszjky.cn

[R17] 数组定义与取值
来源：http://fm.szsharing.cn

arr=(a b c); echo "${arr[0]}"
来源：http://yc.lnxyls.cn

[R18] 遍历数组
来源：http://jf.shxzskj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tb.huixiangedu.cn

[R19] 数组长度
来源：http://ji.nicolike.cn

echo "${#arr[@]}"
来源：http://rv.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://yx.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wx.newstarts.cn

[R21] 字符串长度
来源：http://kw.huanxung.cn

echo "${#s}"
来源：http://wa.hahajie.cn

[R22] 截取子串
来源：http://ak.chemitech.net.cn

echo "${s:0:5}"
来源：http://gt.shxzukj.cn

[R23] 字符串替换
来源：http://ib.hahajie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hr.muxihuayi.cn

[R24] 大小写转换
来源：http://yi.huanxung.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ar.haigaiapp.cn

[R25] 去后缀 / 去前缀
来源：http://lb.huanxung.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://me.jctech888.com.cn

[R26] 命令替换
来源：http://jc.newstarts.cn

now=$(date +%F); echo "$now"
来源：http://je.shxzskj.cn

[R27] 算术展开
来源：http://kn.huixiangedu.cn

echo $((1 + 2 * 3))
来源：http://lm.nszjky.cn

[R28] 浮点运算
来源：http://kf.colortex.cn

echo "scale=2; 10/3" | bc
来源：http://iz.haigaiapp.cn

[R29] 定义函数
来源：http://sz.huixinmuqiang.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ts.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://bd.shtwfgs.cn

f() { return 0; }; f || echo "失败了"
来源：http://sr.shxzskj.cn

[R31] 局部变量
来源：http://ww.hnjuh.cn

f() { local x=1; echo "$x"; }
来源：http://pp.panjiajie.cn

[R32] 参数个数校验
来源：http://hh.521024.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gs.colortex.cn

[R33] 捕获错误并提示行号
来源：http://lr.9csxet.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fp.bookmarksfly.cn

[R34] 退出时清理
来源：http://ih.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yd.hnjuh.cn

[R35] 后台执行并等待
来源：http://nq.9csxet.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yf.shxzskj.cn

[R36] 并发执行多个任务
来源：http://wx.huixinmuqiang.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eg.yuexingan06.cn

[R37] 把输出赋给变量
来源：http://um.yuexingan06.cn

files=$(ls -1)
来源：http://sj.9csxet.cn

[R38] 管道串联
来源：http://nf.huixiangedu.cn

cat a.txt | grep -i error | wc -l
来源：http://mn.hahajie.cn

[R39] 重定向标准输出与错误
来源：http://bm.panjiajie.cn

cmd > out.log 2>&1
来源：http://uq.chemitech.net.cn

[R40] 追加写日志
来源：http://rm.panjiajie.cn

echo "log" >> out.log
来源：http://un.nszjky.cn

[R41] 丢弃输出
来源：http://hg.panjiajie.cn

cmd >/dev/null 2>&1
来源：http://dw.shxzukj.cn

[R42] 输入重定向
来源：http://yu.panjiajie.cn

wc -l < a.txt
来源：http://vm.bjjhwx.cn

[R43] 按名字查找文件
来源：http://in.haigaiapp.cn

find . -name "*.log" -type f
来源：http://fe.huanxung.cn

[R44] 按修改时间查找
来源：http://gh.521024.cn

find . -mtime -7 -type f
来源：http://fo.colortex.cn

[R45] 批量删除
来源：http://wc.newstarts.cn

find . -name "*.tmp" -delete
来源：http://to.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://xm.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xc.huanxung.cn

[R47] sed 单行替换
来源：http://xz.hnjuh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cg.newstarts.cn

[R48] awk 取指定列
来源：http://jx.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://jt.shxzukj.cn

[R49] awk 带条件
来源：http://ft.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vf.hahajie.cn

[R50] awk 求和
来源：http://wz.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zi.hahajie.cn

[R51] 排序去重取前几
来源：http://sf.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jg.jianghongdianzi.cn

[R52] 统计行数
来源：http://lj.jctech888.com.cn

wc -l a.txt
来源：http://nm.hnjuh.cn

[R53] 查看文件头与实时尾
来源：http://xv.hahajie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tz.hahajie.cn

[R54] 比较两个文件
来源：http://qs.hahajie.cn

diff a.txt b.txt
来源：http://sb.muxihuayi.cn

[R55] 压缩与解压
来源：http://pb.521024.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ek.huanxung.cn

[R56] 远程拷贝
来源：http://gj.asd995.cn

scp file user@host:/path/
来源：http://vs.szxytkj.cn

[R57] 远程执行命令
来源：http://qz.newstarts.cn

ssh user@host 'uptime'
来源：http://yb.lnxyls.cn

[R58] 下载文件
来源：http://wa.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ot.huixinmuqiang.cn

[R59] 发 POST JSON
来源：http://id.wgjwhj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rf.bjjhwx.cn

[R60] 只看 HTTP 状态码
来源：http://mu.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://st.haigaiapp.cn

[R61] 磁盘占用
来源：http://am.9csxet.cn

df -h;  du -sh *
来源：http://hr.nicolike.cn

[R62] 找最占空间的文件
来源：http://zg.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://vk.asd995.cn

[R63] 内存与进程
来源：http://ne.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://pi.shtwfgs.cn

[R64] 结束进程
来源：http://tb.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://pt.bookmarksfly.cn

[R65] 查看端口占用
来源：http://nf.hnjuh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ac.panjiajie.cn

[R66] 定时任务
来源：http://xg.chemitech.net.cn

crontab -e;  crontab -l
来源：http://in.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://dw.shtwfgs.cn

openssl rand -hex 16
来源：http://jo.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://jx.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sj.lnxyls.cn

[R69] 生成随机密码
来源：http://bo.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://bf.bjjhwx.cn

[R70] 时间戳与互转
来源：http://xq.9csxet.cn

date +%s;  date -d @1700000000
来源：http://sf.colortex.cn

[R71] 日期格式化
来源：http://tv.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ud.szsharing.cn

[R72] 等待端口就绪
来源：http://py.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://us.9csxet.cn

[R73] 分割大日志
来源：http://qv.colortex.cn

split -l 1000 big.log part_
来源：http://oy.huixinmuqiang.cn

[R74] 批量重命名
来源：http://ov.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lj.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://ro.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://om.hnjuh.cn

[R76] 使用临时文件
来源：http://sd.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ws.chemitech.net.cn

[R77] 读取用户输入
来源：http://fq.colortex.cn

read -rp "请输入: " ans
来源：http://ib.huixiangedu.cn

[R78] 交互式菜单
来源：http://ou.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ou.asd995.cn

[R79] 解析命令行选项
来源：http://rx.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ue.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://kh.muxihuayi.cn

time ./run.sh
来源：http://zz.yuexingan06.cn

================================================================================
来源：http://tf.bjjhwx.cn

S. C / C++ 专题
来源：http://wd.shxzukj.cn

================================================================================
来源：http://by.jctech888.com.cn

[S01] C：Hello World
来源：http://ew.9csxet.cn

#include <stdio.h>
来源：http://bs.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bi.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://rk.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://bu.9csxet.cn

[S03] C：读入整数
来源：http://mo.hahajie.cn

int x; scanf("%d", &x);
来源：http://js.shxzukj.cn

[S04] C：字符串复制
来源：http://vy.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cv.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://pt.muxihuayi.cn

strlen(s)
来源：http://nn.hahajie.cn

[S06] C：字符串比较
来源：http://sk.colortex.cn

strcmp(a, b) == 0
来源：http://dz.panjiajie.cn

[S07] C：数组遍历求和
来源：http://lc.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eh.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://am.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mr.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://ld.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kl.nszjky.cn

[S10] C：指针与解引用
来源：http://go.hahajie.cn

int *p = &a;  *p = 5;
来源：http://wx.wgjwhj.cn

[S11] C：逐行读文件
来源：http://jb.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://xq.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ik.9csxet.cn

fclose(f);
来源：http://pi.wgjwhj.cn

[S12] C：写文件
来源：http://za.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ri.gzmigu.cn

[S13] C：宏定义
来源：http://sd.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bj.yuexingan06.cn

[S14] C：枚举
来源：http://yb.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://tz.muxihuayi.cn

[S15] C：类型转换
来源：http://id.shxzukj.cn

(double) a / b
来源：http://kk.521024.cn

[S16] C：位操作置位
来源：http://io.huixiangedu.cn

x |= (1 << 3);
来源：http://sh.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://dl.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://za.szxytkj.cn

[S18] C：命令行参数
来源：http://rr.bjjhwx.cn

int main(int argc, char **argv)
来源：http://il.szsharing.cn

[S19] C：快速排序
来源：http://qe.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vh.shxzskj.cn

[S20] C：二分查找
来源：http://gp.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bp.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://is.nszjky.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ih.shxzukj.cn

[S22] C：字符串转数字
来源：http://mt.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ns.asd995.cn

[S23] C：随机数
来源：http://fa.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yf.jctech888.com.cn

[S24] C：获取本地时间
来源：http://ow.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rc.panjiajie.cn

[S25] C：内存拷贝
来源：http://vb.newstarts.cn

memcpy(dst, src, n);
来源：http://bz.colortex.cn

[S26] C：内存清零
来源：http://cz.szsharing.cn

memset(a, 0, sizeof a);
来源：http://lv.huixinmuqiang.cn

[S27] C：定义常量
来源：http://lq.asd995.cn

const double PI = 3.14159;
来源：http://za.hahajie.cn

[S28] C：静态变量
来源：http://tg.haigaiapp.cn

static int counter = 0;
来源：http://sh.hnjuh.cn

[S29] C：变参函数
来源：http://zs.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qp.szxytkj.cn

[S30] C：头文件保护
来源：http://nv.haigaiapp.cn

#ifndef X_H
来源：http://nx.shxzukj.cn

#define X_H
来源：http://vq.9csxet.cn

#endif
来源：http://ch.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://vm.szsharing.cn

#include <iostream>
来源：http://uo.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://rm.hahajie.cn

[S32] C++：字符串
来源：http://jd.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://br.yuexingan06.cn

[S33] C++：vector 增删
来源：http://py.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ee.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://hu.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://vy.521024.cn

[S35] C++：map
来源：http://an.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rs.colortex.cn

[S36] C++：unordered_map
来源：http://uw.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yp.newstarts.cn


<!-- 参考信息 -->