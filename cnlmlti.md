代发 wailian999

[Q67] 设置隔离级别
来源：http://hx.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xt.newstarts.cn

[Q68] 保存点
来源：http://ic.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://pw.huanxung.cn

ROLLBACK TO sp1;
来源：http://uh.huanxung.cn

[Q69] 查看执行计划
来源：http://zl.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ys.colortex.cn

[Q70] 更新统计信息
来源：http://tr.gzmigu.cn

ANALYZE TABLE users;
来源：http://qo.gzmigu.cn

[Q71] 查看建表语句
来源：http://ss.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cx.nicolike.cn

[Q72] 查看索引
来源：http://fe.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://qz.newstarts.cn

[Q73] 查看表状态
来源：http://ve.huixiangedu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gx.jctech888.com.cn

[Q74] 强制使用索引
来源：http://mi.gzmigu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jr.hahajie.cn

[Q75] 日期格式化
来源：http://rp.jianghongdianzi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fa.yuntaijiaju.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://km.huanxung.cn

[Q76] 按天统计
来源：http://bx.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rq.shxzukj.cn

[Q77] 时间加减
来源：http://yv.bjjhwx.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nt.panjiajie.cn

[Q78] 当前时间
来源：http://zx.haigaiapp.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sn.wgjwhj.cn

[Q79] 字符串拼接
来源：http://jx.9csxet.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mg.yuexingan06.cn

[Q80] 字符串截取
来源：http://nq.huanxung.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rl.shxzskj.cn

[Q81] 字符串替换
来源：http://xb.huanxung.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yq.shxzukj.cn

[Q82] 字符长度与字节长度
来源：http://ge.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gm.chemitech.net.cn

[Q83] 大小写转换
来源：http://xh.colortex.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kl.nszjky.cn

[Q84] 去除首尾空格
来源：http://de.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://kt.szxytkj.cn

[Q85] 数值取整
来源：http://hs.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ad.shtwfgs.cn

[Q86] 读取 JSON 字段
来源：http://va.wgjwhj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mq.lnxyls.cn

[Q87] JSON 字段做条件
来源：http://ak.muxihuayi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xl.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://bt.panjiajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kq.hnjuh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qc.jianghongdianzi.cn

[Q89] 判断表是否存在
来源：http://wl.colortex.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ne.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://zk.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iz.colortex.cn

================================================================================
来源：http://vp.szsharing.cn

R. Bash 专题
来源：http://oh.haigaiapp.cn

================================================================================
来源：http://fh.hnjuh.cn

[R01] shebang 与严格模式
来源：http://jw.huixiangedu.cn

#!/usr/bin/env bash
来源：http://bo.bjjhwx.cn

set -euo pipefail
来源：http://ju.yuexingan06.cn

[R02] 变量赋值与使用
来源：http://qe.gzmigu.cn

name="Tom"; echo "$name"
来源：http://cy.newstarts.cn

[R03] 只读变量
来源：http://sk.wgjwhj.cn

readonly PI=3.14
来源：http://nz.asd995.cn

[R04] 位置参数
来源：http://ja.lnxyls.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vb.newstarts.cn

[R05] 参数默认值
来源：http://zo.huixinmuqiang.cn

name="${1:-default}"
来源：http://tx.bjjhwx.cn

[R06] 判断命令是否存在
来源：http://yj.shxzukj.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lo.9csxet.cn

[R07] if 判断文件
来源：http://cg.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jw.shxzskj.cn

[R08] 数值比较
来源：http://fq.chemitech.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kx.bookmarksfly.cn

[R09] 字符串比较
来源：http://iw.hnjuh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xa.asd995.cn

[R10] 正则匹配
来源：http://ji.gzmigu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yy.9csxet.cn

[R11] case 多分支
来源：http://ub.panjiajie.cn

case "$1" in
来源：http://nh.shtwfgs.cn

start) echo "启动" ;;
来源：http://pd.nicolike.cn

stop)  echo "停止" ;;
来源：http://xd.nszjky.cn

*)     echo "未知命令" ;;
来源：http://jo.szxytkj.cn

esac
来源：http://gx.shtwfgs.cn

[R12] for 遍历文件
来源：http://xf.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://au.szsharing.cn

[R13] for 计数循环
来源：http://gc.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://gm.panjiajie.cn

[R14] C 风格 for
来源：http://mw.huanxung.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iw.muxihuayi.cn

[R15] while 逐行读文件
来源：http://bq.gzmigu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fh.haigaiapp.cn

[R16] until 等待条件
来源：http://gb.colortex.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wp.shxzukj.cn

[R17] 数组定义与取值
来源：http://uv.shxzskj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cr.newstarts.cn

[R18] 遍历数组
来源：http://pi.wgjwhj.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hj.huixiangedu.cn

[R19] 数组长度
来源：http://ai.jianghongdianzi.cn

echo "${#arr[@]}"
来源：http://cq.shxzskj.cn

[R20] 关联数组（字典）
来源：http://bl.nszjky.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ey.newstarts.cn

[R21] 字符串长度
来源：http://sf.bjjhwx.cn

echo "${#s}"
来源：http://py.newstarts.cn

[R22] 截取子串
来源：http://hu.shxzskj.cn

echo "${s:0:5}"
来源：http://qw.nicolike.cn

[R23] 字符串替换
来源：http://vp.nicolike.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ur.nicolike.cn

[R24] 大小写转换
来源：http://ij.panjiajie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xb.yuexingan06.cn

[R25] 去后缀 / 去前缀
来源：http://kl.szxytkj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ce.shxzukj.cn

[R26] 命令替换
来源：http://xk.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://ma.9csxet.cn

[R27] 算术展开
来源：http://yy.nicolike.cn

echo $((1 + 2 * 3))
来源：http://xl.haigaiapp.cn

[R28] 浮点运算
来源：http://zc.shtwfgs.cn

echo "scale=2; 10/3" | bc
来源：http://cx.chemitech.net.cn

[R29] 定义函数
来源：http://vc.bjjhwx.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bn.jianghongdianzi.cn

[R30] 函数返回状态码
来源：http://ns.asd995.cn

f() { return 0; }; f || echo "失败了"
来源：http://iq.9csxet.cn

[R31] 局部变量
来源：http://wg.yuntaijiaju.cn

f() { local x=1; echo "$x"; }
来源：http://rb.shxzskj.cn

[R32] 参数个数校验
来源：http://ed.muxihuayi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xz.panjiajie.cn

[R33] 捕获错误并提示行号
来源：http://dk.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fm.yuexingan06.cn

[R34] 退出时清理
来源：http://qd.nszjky.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ia.yuexingan06.cn

[R35] 后台执行并等待
来源：http://ag.521024.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nt.hnjuh.cn

[R36] 并发执行多个任务
来源：http://rm.gzmigu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tb.huanxung.cn

[R37] 把输出赋给变量
来源：http://aa.jctech888.com.cn

files=$(ls -1)
来源：http://cw.yuexingan06.cn

[R38] 管道串联
来源：http://vo.huixinmuqiang.cn

cat a.txt | grep -i error | wc -l
来源：http://pw.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://jr.szxytkj.cn

cmd > out.log 2>&1
来源：http://jr.szxytkj.cn

[R40] 追加写日志
来源：http://gm.nszjky.cn

echo "log" >> out.log
来源：http://ee.wgjwhj.cn

[R41] 丢弃输出
来源：http://tx.asd995.cn

cmd >/dev/null 2>&1
来源：http://fr.jianghongdianzi.cn

[R42] 输入重定向
来源：http://go.521024.cn

wc -l < a.txt
来源：http://ej.nszjky.cn

[R43] 按名字查找文件
来源：http://vo.szxytkj.cn

find . -name "*.log" -type f
来源：http://uv.chemitech.net.cn

[R44] 按修改时间查找
来源：http://xq.nicolike.cn

find . -mtime -7 -type f
来源：http://pe.shxzukj.cn

[R45] 批量删除
来源：http://ar.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://ax.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://et.szsharing.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://su.shxzukj.cn

[R47] sed 单行替换
来源：http://er.panjiajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ww.wgjwhj.cn

[R48] awk 取指定列
来源：http://dp.jianghongdianzi.cn

awk '{print $1, $3}' a.txt
来源：http://xe.huixinmuqiang.cn

[R49] awk 带条件
来源：http://vz.szxytkj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sy.yuexingan06.cn

[R50] awk 求和
来源：http://cr.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ak.panjiajie.cn

[R51] 排序去重取前几
来源：http://wv.huixinmuqiang.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://on.colortex.cn

[R52] 统计行数
来源：http://fv.muxihuayi.cn

wc -l a.txt
来源：http://jy.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://ca.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://os.bookmarksfly.cn

[R54] 比较两个文件
来源：http://kz.hahajie.cn

diff a.txt b.txt
来源：http://zi.shxzukj.cn

[R55] 压缩与解压
来源：http://wp.jctech888.com.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ms.gzmigu.cn

[R56] 远程拷贝
来源：http://bg.chemitech.net.cn

scp file user@host:/path/
来源：http://cm.shxzskj.cn

[R57] 远程执行命令
来源：http://vz.chemitech.net.cn

ssh user@host 'uptime'
来源：http://yt.shxzukj.cn

[R58] 下载文件
来源：http://ck.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zg.szsharing.cn

[R59] 发 POST JSON
来源：http://kj.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ex.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://hh.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yn.huanxung.cn

[R61] 磁盘占用
来源：http://vp.huixinmuqiang.cn

df -h;  du -sh *
来源：http://cj.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://fc.nszjky.cn

du -ah . | sort -rh | head -10
来源：http://gi.haigaiapp.cn

[R63] 内存与进程
来源：http://ax.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://cb.muxihuayi.cn

[R64] 结束进程
来源：http://ha.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://oj.szxytkj.cn

[R65] 查看端口占用
来源：http://jq.hahajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://he.jctech888.com.cn

[R66] 定时任务
来源：http://bm.szsharing.cn

crontab -e;  crontab -l
来源：http://me.nszjky.cn

[R67] 生成随机十六进制串
来源：http://jb.szsharing.cn

openssl rand -hex 16
来源：http://he.shxzskj.cn

[R68] 计算文件校验值
来源：http://ym.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vy.yuntaijiaju.cn

[R69] 生成随机密码
来源：http://mp.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://gt.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://le.9csxet.cn

date +%s;  date -d @1700000000
来源：http://ls.asd995.cn

[R71] 日期格式化
来源：http://hj.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://av.wgjwhj.cn

[R72] 等待端口就绪
来源：http://vk.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mg.nicolike.cn

[R73] 分割大日志
来源：http://tb.jianghongdianzi.cn

split -l 1000 big.log part_
来源：http://es.lnxyls.cn

[R74] 批量重命名
来源：http://ma.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kf.newstarts.cn

[R75] 导出环境变量
来源：http://gk.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://ar.hahajie.cn

[R76] 使用临时文件
来源：http://vx.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xz.lnxyls.cn

[R77] 读取用户输入
来源：http://pp.chemitech.net.cn

read -rp "请输入: " ans
来源：http://bb.bookmarksfly.cn

[R78] 交互式菜单
来源：http://wq.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oh.panjiajie.cn

[R79] 解析命令行选项
来源：http://se.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://md.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://hg.wgjwhj.cn

time ./run.sh
来源：http://io.bookmarksfly.cn

================================================================================
来源：http://qj.jctech888.com.cn

S. C / C++ 专题
来源：http://eq.asd995.cn

================================================================================
来源：http://ur.huixinmuqiang.cn

[S01] C：Hello World
来源：http://md.szsharing.cn

#include <stdio.h>
来源：http://nh.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gb.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://oa.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://hp.wgjwhj.cn

[S03] C：读入整数
来源：http://xk.muxihuayi.cn

int x; scanf("%d", &x);
来源：http://uh.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://cg.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://am.newstarts.cn

[S05] C：字符串长度
来源：http://zw.chemitech.net.cn

strlen(s)
来源：http://xw.9csxet.cn

[S06] C：字符串比较
来源：http://oc.9csxet.cn

strcmp(a, b) == 0
来源：http://oc.asd995.cn

[S07] C：数组遍历求和
来源：http://eu.nicolike.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ry.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://dl.hnjuh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nv.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://dp.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bn.bjjhwx.cn

[S10] C：指针与解引用
来源：http://bs.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://xl.hahajie.cn

[S11] C：逐行读文件
来源：http://rz.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://yh.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bf.yuntaijiaju.cn

fclose(f);
来源：http://we.521024.cn

[S12] C：写文件
来源：http://br.521024.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vf.newstarts.cn

[S13] C：宏定义
来源：http://qy.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yg.newstarts.cn

[S14] C：枚举
来源：http://ri.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://ea.shxzukj.cn

[S15] C：类型转换
来源：http://bg.huixinmuqiang.cn

(double) a / b
来源：http://qv.nszjky.cn

[S16] C：位操作置位
来源：http://bj.panjiajie.cn

x |= (1 << 3);
来源：http://yb.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://jv.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pu.nszjky.cn

[S18] C：命令行参数
来源：http://sm.szsharing.cn

int main(int argc, char **argv)
来源：http://pa.wgjwhj.cn

[S19] C：快速排序
来源：http://hh.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rb.haigaiapp.cn

[S20] C：二分查找
来源：http://oz.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rt.jianghongdianzi.cn

[S21] C：字符类别判断
来源：http://kz.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ar.lnxyls.cn

[S22] C：字符串转数字
来源：http://py.nszjky.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dm.newstarts.cn

[S23] C：随机数
来源：http://px.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mr.muxihuayi.cn

[S24] C：获取本地时间
来源：http://pc.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zu.szsharing.cn

[S25] C：内存拷贝
来源：http://cn.szsharing.cn

memcpy(dst, src, n);
来源：http://za.newstarts.cn

[S26] C：内存清零
来源：http://an.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://db.nicolike.cn

[S27] C：定义常量
来源：http://qf.hahajie.cn

const double PI = 3.14159;
来源：http://rk.hahajie.cn

[S28] C：静态变量
来源：http://nb.lnxyls.cn

static int counter = 0;
来源：http://jk.szsharing.cn

[S29] C：变参函数
来源：http://db.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qw.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ma.shtwfgs.cn

#ifndef X_H
来源：http://oo.shxzskj.cn

#define X_H
来源：http://pq.jctech888.com.cn

#endif
来源：http://np.muxihuayi.cn

[S31] C++：Hello World
来源：http://ru.yuexingan06.cn

#include <iostream>
来源：http://ah.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://op.shxzskj.cn

[S32] C++：字符串
来源：http://rm.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://xf.yuexingan06.cn

[S33] C++：vector 增删
来源：http://nw.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ff.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://qh.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://kq.9csxet.cn

[S35] C++：map
来源：http://io.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sx.gzmigu.cn

[S36] C++：unordered_map
来源：http://jy.hahajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ny.muxihuayi.cn


<!-- 参考信息 -->