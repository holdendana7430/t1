代发 wailian999

[Q65] 回滚事务
来源：http://ep.yuntaijiaju.cn

ROLLBACK;
来源：http://fc.haigaiapp.cn

[Q66] 行锁查询
来源：http://py.hahajie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pi.jianghongdianzi.cn

[Q67] 设置隔离级别
来源：http://sv.huixinmuqiang.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ly.newstarts.cn

[Q68] 保存点
来源：http://tj.yuexingan06.cn

SAVEPOINT sp1;
来源：http://nz.jianghongdianzi.cn

ROLLBACK TO sp1;
来源：http://xw.wgjwhj.cn

[Q69] 查看执行计划
来源：http://rs.huanxung.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bp.yuexingan06.cn

[Q70] 更新统计信息
来源：http://tx.huixinmuqiang.cn

ANALYZE TABLE users;
来源：http://ao.gzmigu.cn

[Q71] 查看建表语句
来源：http://cu.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dj.haigaiapp.cn

[Q72] 查看索引
来源：http://lz.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://wr.jctech888.com.cn

[Q73] 查看表状态
来源：http://gp.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sg.bjjhwx.cn

[Q74] 强制使用索引
来源：http://bg.wgjwhj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zm.chemitech.net.cn

[Q75] 日期格式化
来源：http://bb.haigaiapp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wy.huixinmuqiang.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ik.hnjuh.cn

[Q76] 按天统计
来源：http://am.asd995.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ov.jianghongdianzi.cn

[Q77] 时间加减
来源：http://ge.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rh.lnxyls.cn

[Q78] 当前时间
来源：http://hn.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kr.shxzskj.cn

[Q79] 字符串拼接
来源：http://et.bjjhwx.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fv.yuntaijiaju.cn

[Q80] 字符串截取
来源：http://vc.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lv.yuntaijiaju.cn

[Q81] 字符串替换
来源：http://aa.bjjhwx.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sm.9csxet.cn

[Q82] 字符长度与字节长度
来源：http://ev.newstarts.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oj.jianghongdianzi.cn

[Q83] 大小写转换
来源：http://vp.muxihuayi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ji.shxzukj.cn

[Q84] 去除首尾空格
来源：http://bg.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://gl.chemitech.net.cn

[Q85] 数值取整
来源：http://yl.hahajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://si.lnxyls.cn

[Q86] 读取 JSON 字段
来源：http://eh.bookmarksfly.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nv.hnjuh.cn

[Q87] JSON 字段做条件
来源：http://fk.bookmarksfly.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mf.szsharing.cn

[Q88] 行转列（条件聚合）
来源：http://zb.shtwfgs.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jr.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tb.lnxyls.cn

[Q89] 判断表是否存在
来源：http://nq.asd995.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pf.colortex.cn

[Q90] 生成序号列
来源：http://rt.yuexingan06.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nf.muxihuayi.cn

================================================================================
来源：http://la.gzmigu.cn

R. Bash 专题
来源：http://xe.huixinmuqiang.cn

================================================================================
来源：http://mw.szxytkj.cn

[R01] shebang 与严格模式
来源：http://rw.gzmigu.cn

#!/usr/bin/env bash
来源：http://ms.521024.cn

set -euo pipefail
来源：http://vy.9csxet.cn

[R02] 变量赋值与使用
来源：http://ir.muxihuayi.cn

name="Tom"; echo "$name"
来源：http://ra.bjjhwx.cn

[R03] 只读变量
来源：http://wo.muxihuayi.cn

readonly PI=3.14
来源：http://sd.szsharing.cn

[R04] 位置参数
来源：http://tu.szsharing.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ae.yuexingan06.cn

[R05] 参数默认值
来源：http://nb.wgjwhj.cn

name="${1:-default}"
来源：http://zl.gzmigu.cn

[R06] 判断命令是否存在
来源：http://xa.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://je.asd995.cn

[R07] if 判断文件
来源：http://ll.shtwfgs.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zz.hahajie.cn

[R08] 数值比较
来源：http://yk.huanxung.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hp.szsharing.cn

[R09] 字符串比较
来源：http://eu.asd995.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qx.hnjuh.cn

[R10] 正则匹配
来源：http://va.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nw.lnxyls.cn

[R11] case 多分支
来源：http://dg.shxzukj.cn

case "$1" in
来源：http://ir.szsharing.cn

start) echo "启动" ;;
来源：http://ir.hnjuh.cn

stop)  echo "停止" ;;
来源：http://fx.9csxet.cn

*)     echo "未知命令" ;;
来源：http://xq.shxzskj.cn

esac
来源：http://bl.newstarts.cn

[R12] for 遍历文件
来源：http://tz.huixinmuqiang.cn

for f in *.txt; do echo "$f"; done
来源：http://er.wgjwhj.cn

[R13] for 计数循环
来源：http://ry.szxytkj.cn

for i in {1..10}; do echo "$i"; done
来源：http://cg.szxytkj.cn

[R14] C 风格 for
来源：http://ht.chemitech.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cm.panjiajie.cn

[R15] while 逐行读文件
来源：http://do.shtwfgs.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yn.huixinmuqiang.cn

[R16] until 等待条件
来源：http://dj.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fm.hnjuh.cn

[R17] 数组定义与取值
来源：http://rd.gzmigu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bz.shtwfgs.cn

[R18] 遍历数组
来源：http://es.asd995.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sd.hnjuh.cn

[R19] 数组长度
来源：http://rm.shxzskj.cn

echo "${#arr[@]}"
来源：http://gw.jctech888.com.cn

[R20] 关联数组（字典）
来源：http://ew.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ed.yuexingan06.cn

[R21] 字符串长度
来源：http://zg.colortex.cn

echo "${#s}"
来源：http://fr.hahajie.cn

[R22] 截取子串
来源：http://zh.yuexingan06.cn

echo "${s:0:5}"
来源：http://ad.panjiajie.cn

[R23] 字符串替换
来源：http://bj.9csxet.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kz.asd995.cn

[R24] 大小写转换
来源：http://bd.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mb.asd995.cn

[R25] 去后缀 / 去前缀
来源：http://mt.521024.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gu.lnxyls.cn

[R26] 命令替换
来源：http://na.jctech888.com.cn

now=$(date +%F); echo "$now"
来源：http://oo.muxihuayi.cn

[R27] 算术展开
来源：http://wj.hahajie.cn

echo $((1 + 2 * 3))
来源：http://px.colortex.cn

[R28] 浮点运算
来源：http://me.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://qw.huanxung.cn

[R29] 定义函数
来源：http://bd.nicolike.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nr.9csxet.cn

[R30] 函数返回状态码
来源：http://su.colortex.cn

f() { return 0; }; f || echo "失败了"
来源：http://aa.chemitech.net.cn

[R31] 局部变量
来源：http://lj.521024.cn

f() { local x=1; echo "$x"; }
来源：http://pi.haigaiapp.cn

[R32] 参数个数校验
来源：http://eh.lnxyls.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mq.bjjhwx.cn

[R33] 捕获错误并提示行号
来源：http://tj.bookmarksfly.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ay.wgjwhj.cn

[R34] 退出时清理
来源：http://cw.shxzskj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ub.yuntaijiaju.cn

[R35] 后台执行并等待
来源：http://sq.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pe.jctech888.com.cn

[R36] 并发执行多个任务
来源：http://cu.bookmarksfly.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ny.nszjky.cn

[R37] 把输出赋给变量
来源：http://oa.yuntaijiaju.cn

files=$(ls -1)
来源：http://fl.chemitech.net.cn

[R38] 管道串联
来源：http://bw.shtwfgs.cn

cat a.txt | grep -i error | wc -l
来源：http://dy.szxytkj.cn

[R39] 重定向标准输出与错误
来源：http://yl.panjiajie.cn

cmd > out.log 2>&1
来源：http://bk.panjiajie.cn

[R40] 追加写日志
来源：http://pj.nicolike.cn

echo "log" >> out.log
来源：http://tp.nicolike.cn

[R41] 丢弃输出
来源：http://al.asd995.cn

cmd >/dev/null 2>&1
来源：http://zo.wgjwhj.cn

[R42] 输入重定向
来源：http://yn.bookmarksfly.cn

wc -l < a.txt
来源：http://ic.szsharing.cn

[R43] 按名字查找文件
来源：http://ak.bjjhwx.cn

find . -name "*.log" -type f
来源：http://uh.colortex.cn

[R44] 按修改时间查找
来源：http://bm.asd995.cn

find . -mtime -7 -type f
来源：http://gy.hahajie.cn

[R45] 批量删除
来源：http://wd.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://xz.asd995.cn

[R46] 递归替换文件内容
来源：http://ey.chemitech.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ur.huanxung.cn

[R47] sed 单行替换
来源：http://lk.hahajie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sm.huanxung.cn

[R48] awk 取指定列
来源：http://ho.szxytkj.cn

awk '{print $1, $3}' a.txt
来源：http://ml.jctech888.com.cn

[R49] awk 带条件
来源：http://hu.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lu.newstarts.cn

[R50] awk 求和
来源：http://ms.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ak.newstarts.cn

[R51] 排序去重取前几
来源：http://vy.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xd.asd995.cn

[R52] 统计行数
来源：http://su.panjiajie.cn

wc -l a.txt
来源：http://ys.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://ce.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://la.haigaiapp.cn

[R54] 比较两个文件
来源：http://zw.chemitech.net.cn

diff a.txt b.txt
来源：http://vl.shtwfgs.cn

[R55] 压缩与解压
来源：http://kv.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ea.nszjky.cn

[R56] 远程拷贝
来源：http://rv.yuexingan06.cn

scp file user@host:/path/
来源：http://wt.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://pw.521024.cn

ssh user@host 'uptime'
来源：http://fd.szxytkj.cn

[R58] 下载文件
来源：http://dp.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zz.hnjuh.cn

[R59] 发 POST JSON
来源：http://sl.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://st.huixiangedu.cn

[R60] 只看 HTTP 状态码
来源：http://zv.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tc.bookmarksfly.cn

[R61] 磁盘占用
来源：http://dk.asd995.cn

df -h;  du -sh *
来源：http://wg.asd995.cn

[R62] 找最占空间的文件
来源：http://fd.hnjuh.cn

du -ah . | sort -rh | head -10
来源：http://ni.szsharing.cn

[R63] 内存与进程
来源：http://qz.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://uz.lnxyls.cn

[R64] 结束进程
来源：http://gb.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://lf.jctech888.com.cn

[R65] 查看端口占用
来源：http://fj.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gm.9csxet.cn

[R66] 定时任务
来源：http://af.gzmigu.cn

crontab -e;  crontab -l
来源：http://jo.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://cl.9csxet.cn

openssl rand -hex 16
来源：http://ka.lnxyls.cn

[R68] 计算文件校验值
来源：http://va.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gh.szxytkj.cn

[R69] 生成随机密码
来源：http://qd.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://bi.gzmigu.cn

[R70] 时间戳与互转
来源：http://ol.nszjky.cn

date +%s;  date -d @1700000000
来源：http://fd.gzmigu.cn

[R71] 日期格式化
来源：http://kq.hnjuh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rg.chemitech.net.cn

[R72] 等待端口就绪
来源：http://cx.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://km.jianghongdianzi.cn

[R73] 分割大日志
来源：http://sj.shxzukj.cn

split -l 1000 big.log part_
来源：http://og.chemitech.net.cn

[R74] 批量重命名
来源：http://dn.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dc.lnxyls.cn

[R75] 导出环境变量
来源：http://nn.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://jz.nszjky.cn

[R76] 使用临时文件
来源：http://bt.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sb.9csxet.cn

[R77] 读取用户输入
来源：http://id.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ap.muxihuayi.cn

[R78] 交互式菜单
来源：http://ak.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rf.9csxet.cn

[R79] 解析命令行选项
来源：http://zn.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fl.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ho.haigaiapp.cn

time ./run.sh
来源：http://yf.gzmigu.cn

================================================================================
来源：http://jo.gzmigu.cn

S. C / C++ 专题
来源：http://jj.haigaiapp.cn

================================================================================
来源：http://as.wgjwhj.cn

[S01] C：Hello World
来源：http://wd.szxytkj.cn

#include <stdio.h>
来源：http://zm.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ol.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://ai.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://vo.9csxet.cn

[S03] C：读入整数
来源：http://tm.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://lq.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://bo.asd995.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ur.wgjwhj.cn

[S05] C：字符串长度
来源：http://us.shxzskj.cn

strlen(s)
来源：http://ku.newstarts.cn

[S06] C：字符串比较
来源：http://pa.bookmarksfly.cn

strcmp(a, b) == 0
来源：http://ba.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://xs.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rb.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://xu.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cm.521024.cn

[S09] C：结构体定义与初始化
来源：http://sz.lnxyls.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hu.newstarts.cn

[S10] C：指针与解引用
来源：http://sd.asd995.cn

int *p = &a;  *p = 5;
来源：http://ma.nicolike.cn

[S11] C：逐行读文件
来源：http://rm.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://rt.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zy.szsharing.cn

fclose(f);
来源：http://ak.jianghongdianzi.cn

[S12] C：写文件
来源：http://lf.newstarts.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://co.shxzskj.cn

[S13] C：宏定义
来源：http://fi.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uh.haigaiapp.cn

[S14] C：枚举
来源：http://nn.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://tw.gzmigu.cn

[S15] C：类型转换
来源：http://as.shtwfgs.cn

(double) a / b
来源：http://xk.hahajie.cn

[S16] C：位操作置位
来源：http://gb.nicolike.cn

x |= (1 << 3);
来源：http://me.nszjky.cn

[S17] C：安全拼接字符串
来源：http://st.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wh.newstarts.cn

[S18] C：命令行参数
来源：http://cl.wgjwhj.cn

int main(int argc, char **argv)
来源：http://sa.huanxung.cn

[S19] C：快速排序
来源：http://vk.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://th.huanxung.cn

[S20] C：二分查找
来源：http://bl.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ll.shxzskj.cn

[S21] C：字符类别判断
来源：http://wc.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xq.shtwfgs.cn

[S22] C：字符串转数字
来源：http://jx.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://me.panjiajie.cn

[S23] C：随机数
来源：http://rd.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mm.szxytkj.cn

[S24] C：获取本地时间
来源：http://sy.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cv.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://pe.nicolike.cn

memcpy(dst, src, n);
来源：http://zh.newstarts.cn

[S26] C：内存清零
来源：http://gw.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://iy.shxzskj.cn

[S27] C：定义常量
来源：http://el.521024.cn

const double PI = 3.14159;
来源：http://ud.yuexingan06.cn

[S28] C：静态变量
来源：http://ip.szsharing.cn

static int counter = 0;
来源：http://mq.asd995.cn

[S29] C：变参函数
来源：http://ty.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yg.lnxyls.cn

[S30] C：头文件保护
来源：http://mh.yuntaijiaju.cn

#ifndef X_H
来源：http://eq.colortex.cn

#define X_H
来源：http://xy.shxzukj.cn

#endif
来源：http://xl.nicolike.cn

[S31] C++：Hello World
来源：http://lk.9csxet.cn

#include <iostream>
来源：http://hh.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://pm.jctech888.com.cn

[S32] C++：字符串
来源：http://kl.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://gj.muxihuayi.cn

[S33] C++：vector 增删
来源：http://az.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ax.szsharing.cn

[S34] C++：遍历 vector
来源：http://hi.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://es.huixinmuqiang.cn


<!-- 参考信息 -->