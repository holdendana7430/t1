代发 wailian999

[Q65] 回滚事务
来源：http://zk.panjiajie.cn

ROLLBACK;
来源：http://pq.shxzukj.cn

[Q66] 行锁查询
来源：http://yw.huixiangedu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://or.huanxung.cn

[Q67] 设置隔离级别
来源：http://zc.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oy.chemitech.net.cn

[Q68] 保存点
来源：http://gn.szsharing.cn

SAVEPOINT sp1;
来源：http://wl.jctech888.com.cn

ROLLBACK TO sp1;
来源：http://hu.gzmigu.cn

[Q69] 查看执行计划
来源：http://uf.asd995.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rc.shxzskj.cn

[Q70] 更新统计信息
来源：http://wh.9csxet.cn

ANALYZE TABLE users;
来源：http://lq.521024.cn

[Q71] 查看建表语句
来源：http://bn.asd995.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tz.huanxung.cn

[Q72] 查看索引
来源：http://np.huixinmuqiang.cn

SHOW INDEX FROM users;
来源：http://qo.szsharing.cn

[Q73] 查看表状态
来源：http://kd.9csxet.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ev.shxzskj.cn

[Q74] 强制使用索引
来源：http://nw.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tk.gzmigu.cn

[Q75] 日期格式化
来源：http://jf.nszjky.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yv.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ky.nicolike.cn

[Q76] 按天统计
来源：http://eu.jctech888.com.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ll.szsharing.cn

[Q77] 时间加减
来源：http://lh.gzmigu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ez.jctech888.com.cn

[Q78] 当前时间
来源：http://pj.yuntaijiaju.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oy.hnjuh.cn

[Q79] 字符串拼接
来源：http://vu.panjiajie.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fz.bookmarksfly.cn

[Q80] 字符串截取
来源：http://bt.haigaiapp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ve.newstarts.cn

[Q81] 字符串替换
来源：http://yq.wgjwhj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fq.wgjwhj.cn

[Q82] 字符长度与字节长度
来源：http://wc.hahajie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ou.shxzskj.cn

[Q83] 大小写转换
来源：http://yh.shxzskj.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hs.asd995.cn

[Q84] 去除首尾空格
来源：http://nq.colortex.cn

SELECT TRIM(name) FROM users;
来源：http://qe.nszjky.cn

[Q85] 数值取整
来源：http://ia.panjiajie.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cf.nszjky.cn

[Q86] 读取 JSON 字段
来源：http://ro.hahajie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yk.yuntaijiaju.cn

[Q87] JSON 字段做条件
来源：http://pt.newstarts.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qs.bookmarksfly.cn

[Q88] 行转列（条件聚合）
来源：http://gv.hahajie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xi.nicolike.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sb.hnjuh.cn

[Q89] 判断表是否存在
来源：http://hy.chemitech.net.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jg.lnxyls.cn

[Q90] 生成序号列
来源：http://gp.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://em.hnjuh.cn

================================================================================
来源：http://xz.huanxung.cn

R. Bash 专题
来源：http://ld.szsharing.cn

================================================================================
来源：http://fj.panjiajie.cn

[R01] shebang 与严格模式
来源：http://og.shxzukj.cn

#!/usr/bin/env bash
来源：http://rl.yuntaijiaju.cn

set -euo pipefail
来源：http://qh.gzmigu.cn

[R02] 变量赋值与使用
来源：http://lm.yuexingan06.cn

name="Tom"; echo "$name"
来源：http://eg.szsharing.cn

[R03] 只读变量
来源：http://nh.szxytkj.cn

readonly PI=3.14
来源：http://cm.wgjwhj.cn

[R04] 位置参数
来源：http://uw.hnjuh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ol.szsharing.cn

[R05] 参数默认值
来源：http://fn.yuexingan06.cn

name="${1:-default}"
来源：http://ln.bookmarksfly.cn

[R06] 判断命令是否存在
来源：http://kp.newstarts.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sa.chemitech.net.cn

[R07] if 判断文件
来源：http://qy.bookmarksfly.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kj.shxzskj.cn

[R08] 数值比较
来源：http://jx.wgjwhj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mm.shxzukj.cn

[R09] 字符串比较
来源：http://tw.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lh.newstarts.cn

[R10] 正则匹配
来源：http://jn.colortex.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ry.jianghongdianzi.cn

[R11] case 多分支
来源：http://xw.chemitech.net.cn

case "$1" in
来源：http://ic.hnjuh.cn

start) echo "启动" ;;
来源：http://gx.newstarts.cn

stop)  echo "停止" ;;
来源：http://jg.asd995.cn

*)     echo "未知命令" ;;
来源：http://xl.haigaiapp.cn

esac
来源：http://ww.asd995.cn

[R12] for 遍历文件
来源：http://fm.panjiajie.cn

for f in *.txt; do echo "$f"; done
来源：http://im.gzmigu.cn

[R13] for 计数循环
来源：http://rd.bjjhwx.cn

for i in {1..10}; do echo "$i"; done
来源：http://lt.hahajie.cn

[R14] C 风格 for
来源：http://du.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bb.yuexingan06.cn

[R15] while 逐行读文件
来源：http://uy.szxytkj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cx.shxzskj.cn

[R16] until 等待条件
来源：http://eg.szxytkj.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dz.shtwfgs.cn

[R17] 数组定义与取值
来源：http://ed.asd995.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fb.nicolike.cn

[R18] 遍历数组
来源：http://gi.panjiajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ss.yuexingan06.cn

[R19] 数组长度
来源：http://hd.colortex.cn

echo "${#arr[@]}"
来源：http://kf.haigaiapp.cn

[R20] 关联数组（字典）
来源：http://mw.asd995.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dp.chemitech.net.cn

[R21] 字符串长度
来源：http://wi.chemitech.net.cn

echo "${#s}"
来源：http://hn.shxzukj.cn

[R22] 截取子串
来源：http://cr.521024.cn

echo "${s:0:5}"
来源：http://si.nicolike.cn

[R23] 字符串替换
来源：http://vn.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://en.huixiangedu.cn

[R24] 大小写转换
来源：http://rr.shxzskj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hk.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://gb.hnjuh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wm.szsharing.cn

[R26] 命令替换
来源：http://ke.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://yk.shxzskj.cn

[R27] 算术展开
来源：http://wg.jianghongdianzi.cn

echo $((1 + 2 * 3))
来源：http://iy.shxzskj.cn

[R28] 浮点运算
来源：http://ft.yuexingan06.cn

echo "scale=2; 10/3" | bc
来源：http://iv.asd995.cn

[R29] 定义函数
来源：http://kr.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://av.huixinmuqiang.cn

[R30] 函数返回状态码
来源：http://qs.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://kk.asd995.cn

[R31] 局部变量
来源：http://pl.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://bw.colortex.cn

[R32] 参数个数校验
来源：http://bw.szsharing.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gl.bookmarksfly.cn

[R33] 捕获错误并提示行号
来源：http://nf.panjiajie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tu.bookmarksfly.cn

[R34] 退出时清理
来源：http://ak.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uy.bookmarksfly.cn

[R35] 后台执行并等待
来源：http://wj.shxzukj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pk.yuexingan06.cn

[R36] 并发执行多个任务
来源：http://ot.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hw.bookmarksfly.cn

[R37] 把输出赋给变量
来源：http://gv.huanxung.cn

files=$(ls -1)
来源：http://ms.lnxyls.cn

[R38] 管道串联
来源：http://yu.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://em.jctech888.com.cn

[R39] 重定向标准输出与错误
来源：http://kl.huixiangedu.cn

cmd > out.log 2>&1
来源：http://di.huixinmuqiang.cn

[R40] 追加写日志
来源：http://lh.huanxung.cn

echo "log" >> out.log
来源：http://ww.colortex.cn

[R41] 丢弃输出
来源：http://uj.szxytkj.cn

cmd >/dev/null 2>&1
来源：http://lv.hahajie.cn

[R42] 输入重定向
来源：http://sx.nicolike.cn

wc -l < a.txt
来源：http://dr.hahajie.cn

[R43] 按名字查找文件
来源：http://da.nicolike.cn

find . -name "*.log" -type f
来源：http://cv.asd995.cn

[R44] 按修改时间查找
来源：http://ye.9csxet.cn

find . -mtime -7 -type f
来源：http://pi.haigaiapp.cn

[R45] 批量删除
来源：http://bp.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://ju.jianghongdianzi.cn

[R46] 递归替换文件内容
来源：http://eq.521024.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://en.shxzskj.cn

[R47] sed 单行替换
来源：http://jm.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jk.hnjuh.cn

[R48] awk 取指定列
来源：http://nv.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://sr.haigaiapp.cn

[R49] awk 带条件
来源：http://mu.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mc.wgjwhj.cn

[R50] awk 求和
来源：http://az.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ca.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://sy.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://it.muxihuayi.cn

[R52] 统计行数
来源：http://ez.huanxung.cn

wc -l a.txt
来源：http://vf.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://pc.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://um.nicolike.cn

[R54] 比较两个文件
来源：http://lq.szsharing.cn

diff a.txt b.txt
来源：http://vn.gzmigu.cn

[R55] 压缩与解压
来源：http://gm.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jv.9csxet.cn

[R56] 远程拷贝
来源：http://yp.bjjhwx.cn

scp file user@host:/path/
来源：http://ab.szxytkj.cn

[R57] 远程执行命令
来源：http://gz.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://iq.jianghongdianzi.cn

[R58] 下载文件
来源：http://lt.colortex.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lp.gzmigu.cn

[R59] 发 POST JSON
来源：http://ts.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://na.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://lv.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hv.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://oc.wgjwhj.cn

df -h;  du -sh *
来源：http://yu.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://fz.bookmarksfly.cn

du -ah . | sort -rh | head -10
来源：http://bn.9csxet.cn

[R63] 内存与进程
来源：http://xl.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://oe.gzmigu.cn

[R64] 结束进程
来源：http://hc.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://fp.chemitech.net.cn

[R65] 查看端口占用
来源：http://de.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ql.szsharing.cn

[R66] 定时任务
来源：http://lh.hahajie.cn

crontab -e;  crontab -l
来源：http://te.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://ky.szxytkj.cn

openssl rand -hex 16
来源：http://ek.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://io.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fk.nicolike.cn

[R69] 生成随机密码
来源：http://kk.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://qg.521024.cn

[R70] 时间戳与互转
来源：http://wc.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://qo.jctech888.com.cn

[R71] 日期格式化
来源：http://ll.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dl.muxihuayi.cn

[R72] 等待端口就绪
来源：http://kd.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jk.shxzukj.cn

[R73] 分割大日志
来源：http://im.nicolike.cn

split -l 1000 big.log part_
来源：http://bv.hahajie.cn

[R74] 批量重命名
来源：http://fg.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xk.shxzskj.cn

[R75] 导出环境变量
来源：http://lf.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://ja.shxzskj.cn

[R76] 使用临时文件
来源：http://ey.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vs.panjiajie.cn

[R77] 读取用户输入
来源：http://hq.shxzukj.cn

read -rp "请输入: " ans
来源：http://je.huixiangedu.cn

[R78] 交互式菜单
来源：http://gl.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mh.szsharing.cn

[R79] 解析命令行选项
来源：http://hx.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ra.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://uj.521024.cn

time ./run.sh
来源：http://jk.yuntaijiaju.cn

================================================================================
来源：http://bn.huixinmuqiang.cn

S. C / C++ 专题
来源：http://qh.jctech888.com.cn

================================================================================
来源：http://ly.newstarts.cn

[S01] C：Hello World
来源：http://fq.jianghongdianzi.cn

#include <stdio.h>
来源：http://wy.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ra.asd995.cn

[S02] C：变量与格式化输出
来源：http://xr.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://cw.hnjuh.cn

[S03] C：读入整数
来源：http://lm.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://zq.yuexingan06.cn

[S04] C：字符串复制
来源：http://bp.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xb.hahajie.cn

[S05] C：字符串长度
来源：http://tg.huanxung.cn

strlen(s)
来源：http://le.muxihuayi.cn

[S06] C：字符串比较
来源：http://cm.hnjuh.cn

strcmp(a, b) == 0
来源：http://rh.hnjuh.cn

[S07] C：数组遍历求和
来源：http://gn.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pr.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://sz.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ox.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://id.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gb.nszjky.cn

[S10] C：指针与解引用
来源：http://xl.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://gw.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://ub.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ky.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ds.yuntaijiaju.cn

fclose(f);
来源：http://mr.jctech888.com.cn

[S12] C：写文件
来源：http://ha.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qf.shxzukj.cn

[S13] C：宏定义
来源：http://wp.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://po.lnxyls.cn

[S14] C：枚举
来源：http://wu.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://qh.yuntaijiaju.cn

[S15] C：类型转换
来源：http://ik.521024.cn

(double) a / b
来源：http://pv.gzmigu.cn

[S16] C：位操作置位
来源：http://yy.huanxung.cn

x |= (1 << 3);
来源：http://ah.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://us.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oi.yuntaijiaju.cn

[S18] C：命令行参数
来源：http://vz.shxzukj.cn

int main(int argc, char **argv)
来源：http://px.jianghongdianzi.cn

[S19] C：快速排序
来源：http://st.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wb.shxzskj.cn

[S20] C：二分查找
来源：http://uy.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mq.muxihuayi.cn

[S21] C：字符类别判断
来源：http://wo.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cy.szsharing.cn

[S22] C：字符串转数字
来源：http://ay.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ac.lnxyls.cn

[S23] C：随机数
来源：http://jd.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zy.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://av.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gp.haigaiapp.cn

[S25] C：内存拷贝
来源：http://vy.huixiangedu.cn

memcpy(dst, src, n);
来源：http://my.muxihuayi.cn

[S26] C：内存清零
来源：http://ra.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://vh.huixinmuqiang.cn

[S27] C：定义常量
来源：http://cu.bjjhwx.cn

const double PI = 3.14159;
来源：http://sz.szxytkj.cn

[S28] C：静态变量
来源：http://cr.huanxung.cn

static int counter = 0;
来源：http://zx.wgjwhj.cn

[S29] C：变参函数
来源：http://ly.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yp.nicolike.cn

[S30] C：头文件保护
来源：http://je.newstarts.cn

#ifndef X_H
来源：http://av.huanxung.cn

#define X_H
来源：http://oc.szxytkj.cn

#endif
来源：http://wk.haigaiapp.cn

[S31] C++：Hello World
来源：http://nj.haigaiapp.cn

#include <iostream>
来源：http://ba.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ha.newstarts.cn

[S32] C++：字符串
来源：http://mb.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://td.shxzskj.cn

[S33] C++：vector 增删
来源：http://um.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yx.hnjuh.cn

[S34] C++：遍历 vector
来源：http://xa.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://tc.jctech888.com.cn


<!-- 参考信息 -->