代发 wailian999

[Q65] 回滚事务
来源：http://ie.wgjwhj.cn

ROLLBACK;
来源：http://dd.bookmarksfly.cn

[Q66] 行锁查询
来源：http://hw.nszjky.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dl.hnjuh.cn

[Q67] 设置隔离级别
来源：http://wq.yuexingan06.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wq.gzmigu.cn

[Q68] 保存点
来源：http://tp.haigaiapp.cn

SAVEPOINT sp1;
来源：http://oa.yuntaijiaju.cn

ROLLBACK TO sp1;
来源：http://lx.yuntaijiaju.cn

[Q69] 查看执行计划
来源：http://dz.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xs.nicolike.cn

[Q70] 更新统计信息
来源：http://iw.yuexingan06.cn

ANALYZE TABLE users;
来源：http://vu.9csxet.cn

[Q71] 查看建表语句
来源：http://ea.colortex.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://km.521024.cn

[Q72] 查看索引
来源：http://qz.wgjwhj.cn

SHOW INDEX FROM users;
来源：http://md.haigaiapp.cn

[Q73] 查看表状态
来源：http://wl.shxzskj.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lm.nszjky.cn

[Q74] 强制使用索引
来源：http://hi.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uz.hnjuh.cn

[Q75] 日期格式化
来源：http://it.newstarts.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mg.lnxyls.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://np.panjiajie.cn

[Q76] 按天统计
来源：http://wn.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://re.shxzskj.cn

[Q77] 时间加减
来源：http://po.chemitech.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gg.yuexingan06.cn

[Q78] 当前时间
来源：http://jv.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ia.szxytkj.cn

[Q79] 字符串拼接
来源：http://hl.nszjky.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nr.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://vt.colortex.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gt.panjiajie.cn

[Q81] 字符串替换
来源：http://om.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ig.bjjhwx.cn

[Q82] 字符长度与字节长度
来源：http://ry.huanxung.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oh.bookmarksfly.cn

[Q83] 大小写转换
来源：http://cg.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ku.wgjwhj.cn

[Q84] 去除首尾空格
来源：http://kg.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://op.yuntaijiaju.cn

[Q85] 数值取整
来源：http://bq.huixinmuqiang.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ix.newstarts.cn

[Q86] 读取 JSON 字段
来源：http://ws.shtwfgs.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qu.jianghongdianzi.cn

[Q87] JSON 字段做条件
来源：http://io.huanxung.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rj.haigaiapp.cn

[Q88] 行转列（条件聚合）
来源：http://bx.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pj.jianghongdianzi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xq.shtwfgs.cn

[Q89] 判断表是否存在
来源：http://oq.jianghongdianzi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vc.shxzukj.cn

[Q90] 生成序号列
来源：http://eg.hahajie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jo.wgjwhj.cn

================================================================================
来源：http://ag.lnxyls.cn

R. Bash 专题
来源：http://ow.shtwfgs.cn

================================================================================
来源：http://pi.shtwfgs.cn

[R01] shebang 与严格模式
来源：http://ci.jctech888.com.cn

#!/usr/bin/env bash
来源：http://vk.jianghongdianzi.cn

set -euo pipefail
来源：http://fr.muxihuayi.cn

[R02] 变量赋值与使用
来源：http://zs.wgjwhj.cn

name="Tom"; echo "$name"
来源：http://vv.gzmigu.cn

[R03] 只读变量
来源：http://ph.bjjhwx.cn

readonly PI=3.14
来源：http://gf.yuexingan06.cn

[R04] 位置参数
来源：http://kv.asd995.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yl.lnxyls.cn

[R05] 参数默认值
来源：http://ox.hahajie.cn

name="${1:-default}"
来源：http://ir.lnxyls.cn

[R06] 判断命令是否存在
来源：http://az.szsharing.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://go.hnjuh.cn

[R07] if 判断文件
来源：http://jb.gzmigu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fs.newstarts.cn

[R08] 数值比较
来源：http://nm.gzmigu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rj.muxihuayi.cn

[R09] 字符串比较
来源：http://dz.yuntaijiaju.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fa.bjjhwx.cn

[R10] 正则匹配
来源：http://hn.hahajie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qj.nicolike.cn

[R11] case 多分支
来源：http://hp.muxihuayi.cn

case "$1" in
来源：http://gv.huanxung.cn

start) echo "启动" ;;
来源：http://of.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://tg.huanxung.cn

*)     echo "未知命令" ;;
来源：http://at.newstarts.cn

esac
来源：http://wp.9csxet.cn

[R12] for 遍历文件
来源：http://pk.shtwfgs.cn

for f in *.txt; do echo "$f"; done
来源：http://je.lnxyls.cn

[R13] for 计数循环
来源：http://xo.9csxet.cn

for i in {1..10}; do echo "$i"; done
来源：http://uj.hahajie.cn

[R14] C 风格 for
来源：http://de.nszjky.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jh.shxzskj.cn

[R15] while 逐行读文件
来源：http://cb.huanxung.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uh.yuexingan06.cn

[R16] until 等待条件
来源：http://dw.huanxung.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vc.szxytkj.cn

[R17] 数组定义与取值
来源：http://vp.bookmarksfly.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ip.bjjhwx.cn

[R18] 遍历数组
来源：http://gc.hnjuh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vs.gzmigu.cn

[R19] 数组长度
来源：http://ko.huixinmuqiang.cn

echo "${#arr[@]}"
来源：http://vy.shxzskj.cn

[R20] 关联数组（字典）
来源：http://ii.bookmarksfly.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gr.huixiangedu.cn

[R21] 字符串长度
来源：http://xc.huanxung.cn

echo "${#s}"
来源：http://bu.wgjwhj.cn

[R22] 截取子串
来源：http://dz.chemitech.net.cn

echo "${s:0:5}"
来源：http://kh.huixiangedu.cn

[R23] 字符串替换
来源：http://ty.wgjwhj.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bb.huixiangedu.cn

[R24] 大小写转换
来源：http://dt.lnxyls.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sw.bookmarksfly.cn

[R25] 去后缀 / 去前缀
来源：http://bi.bookmarksfly.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ho.521024.cn

[R26] 命令替换
来源：http://rk.huixinmuqiang.cn

now=$(date +%F); echo "$now"
来源：http://lf.9csxet.cn

[R27] 算术展开
来源：http://ce.9csxet.cn

echo $((1 + 2 * 3))
来源：http://tb.hnjuh.cn

[R28] 浮点运算
来源：http://ft.521024.cn

echo "scale=2; 10/3" | bc
来源：http://jx.hnjuh.cn

[R29] 定义函数
来源：http://hj.panjiajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sa.hahajie.cn

[R30] 函数返回状态码
来源：http://yf.hahajie.cn

f() { return 0; }; f || echo "失败了"
来源：http://ee.newstarts.cn

[R31] 局部变量
来源：http://us.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://dr.asd995.cn

[R32] 参数个数校验
来源：http://kd.nicolike.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nz.szxytkj.cn

[R33] 捕获错误并提示行号
来源：http://wd.shtwfgs.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sr.jianghongdianzi.cn

[R34] 退出时清理
来源：http://og.hnjuh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://su.lnxyls.cn

[R35] 后台执行并等待
来源：http://hc.bookmarksfly.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xf.asd995.cn

[R36] 并发执行多个任务
来源：http://ek.huanxung.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tp.nicolike.cn

[R37] 把输出赋给变量
来源：http://ue.chemitech.net.cn

files=$(ls -1)
来源：http://vn.nszjky.cn

[R38] 管道串联
来源：http://bm.shxzskj.cn

cat a.txt | grep -i error | wc -l
来源：http://oc.shtwfgs.cn

[R39] 重定向标准输出与错误
来源：http://jq.shxzukj.cn

cmd > out.log 2>&1
来源：http://ud.wgjwhj.cn

[R40] 追加写日志
来源：http://eh.gzmigu.cn

echo "log" >> out.log
来源：http://qg.szsharing.cn

[R41] 丢弃输出
来源：http://qc.newstarts.cn

cmd >/dev/null 2>&1
来源：http://rq.hahajie.cn

[R42] 输入重定向
来源：http://nx.szxytkj.cn

wc -l < a.txt
来源：http://hr.nicolike.cn

[R43] 按名字查找文件
来源：http://ll.asd995.cn

find . -name "*.log" -type f
来源：http://xi.nszjky.cn

[R44] 按修改时间查找
来源：http://qt.wgjwhj.cn

find . -mtime -7 -type f
来源：http://ib.huixiangedu.cn

[R45] 批量删除
来源：http://oz.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://rq.asd995.cn

[R46] 递归替换文件内容
来源：http://ua.nicolike.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sl.jctech888.com.cn

[R47] sed 单行替换
来源：http://iw.muxihuayi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mi.9csxet.cn

[R48] awk 取指定列
来源：http://ak.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://bm.yuntaijiaju.cn

[R49] awk 带条件
来源：http://cx.huixinmuqiang.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sa.huixiangedu.cn

[R50] awk 求和
来源：http://px.hahajie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://go.shxzskj.cn

[R51] 排序去重取前几
来源：http://vj.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yp.nicolike.cn

[R52] 统计行数
来源：http://rv.newstarts.cn

wc -l a.txt
来源：http://qp.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://uw.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ve.shxzukj.cn

[R54] 比较两个文件
来源：http://lc.huanxung.cn

diff a.txt b.txt
来源：http://er.bjjhwx.cn

[R55] 压缩与解压
来源：http://jn.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ph.bookmarksfly.cn

[R56] 远程拷贝
来源：http://vy.wgjwhj.cn

scp file user@host:/path/
来源：http://ch.yuntaijiaju.cn

[R57] 远程执行命令
来源：http://er.wgjwhj.cn

ssh user@host 'uptime'
来源：http://yb.shtwfgs.cn

[R58] 下载文件
来源：http://gu.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://em.bjjhwx.cn

[R59] 发 POST JSON
来源：http://nm.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zf.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://dg.szsharing.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zq.asd995.cn

[R61] 磁盘占用
来源：http://rs.jianghongdianzi.cn

df -h;  du -sh *
来源：http://dn.jctech888.com.cn

[R62] 找最占空间的文件
来源：http://en.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ov.chemitech.net.cn

[R63] 内存与进程
来源：http://bg.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://iu.colortex.cn

[R64] 结束进程
来源：http://kf.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://gb.nicolike.cn

[R65] 查看端口占用
来源：http://cr.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xg.newstarts.cn

[R66] 定时任务
来源：http://mi.yuexingan06.cn

crontab -e;  crontab -l
来源：http://ws.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://uk.hahajie.cn

openssl rand -hex 16
来源：http://jo.wgjwhj.cn

[R68] 计算文件校验值
来源：http://nr.yuntaijiaju.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kb.szxytkj.cn

[R69] 生成随机密码
来源：http://jo.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://tr.hnjuh.cn

[R70] 时间戳与互转
来源：http://tp.lnxyls.cn

date +%s;  date -d @1700000000
来源：http://nj.huanxung.cn

[R71] 日期格式化
来源：http://yu.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yi.hnjuh.cn

[R72] 等待端口就绪
来源：http://so.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yt.nicolike.cn

[R73] 分割大日志
来源：http://ek.szxytkj.cn

split -l 1000 big.log part_
来源：http://em.shtwfgs.cn

[R74] 批量重命名
来源：http://cd.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bc.panjiajie.cn

[R75] 导出环境变量
来源：http://hm.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://lf.jctech888.com.cn

[R76] 使用临时文件
来源：http://jy.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qg.wgjwhj.cn

[R77] 读取用户输入
来源：http://sw.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://uk.shtwfgs.cn

[R78] 交互式菜单
来源：http://iw.hahajie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pg.gzmigu.cn

[R79] 解析命令行选项
来源：http://fn.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kb.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://rx.yuexingan06.cn

time ./run.sh
来源：http://dx.szsharing.cn

================================================================================
来源：http://nc.nszjky.cn

S. C / C++ 专题
来源：http://cf.shxzukj.cn

================================================================================
来源：http://qf.9csxet.cn

[S01] C：Hello World
来源：http://iy.panjiajie.cn

#include <stdio.h>
来源：http://yv.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mf.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://en.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://mj.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ad.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://zk.gzmigu.cn

[S04] C：字符串复制
来源：http://qv.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bs.hnjuh.cn

[S05] C：字符串长度
来源：http://pp.muxihuayi.cn

strlen(s)
来源：http://cr.colortex.cn

[S06] C：字符串比较
来源：http://aw.nicolike.cn

strcmp(a, b) == 0
来源：http://hs.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://in.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ce.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://st.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eo.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://vk.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ll.jctech888.com.cn

[S10] C：指针与解引用
来源：http://qt.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://aj.9csxet.cn

[S11] C：逐行读文件
来源：http://or.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ax.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gi.yuntaijiaju.cn

fclose(f);
来源：http://no.shxzukj.cn

[S12] C：写文件
来源：http://ln.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qb.lnxyls.cn

[S13] C：宏定义
来源：http://gt.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ob.9csxet.cn

[S14] C：枚举
来源：http://cy.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://sw.haigaiapp.cn

[S15] C：类型转换
来源：http://do.9csxet.cn

(double) a / b
来源：http://as.lnxyls.cn

[S16] C：位操作置位
来源：http://um.huixiangedu.cn

x |= (1 << 3);
来源：http://vi.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://zw.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aa.asd995.cn

[S18] C：命令行参数
来源：http://fw.asd995.cn

int main(int argc, char **argv)
来源：http://kk.jctech888.com.cn

[S19] C：快速排序
来源：http://ac.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://it.9csxet.cn

[S20] C：二分查找
来源：http://ad.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dy.wgjwhj.cn

[S21] C：字符类别判断
来源：http://ri.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://co.asd995.cn

[S22] C：字符串转数字
来源：http://rp.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ey.huixinmuqiang.cn

[S23] C：随机数
来源：http://fs.9csxet.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ag.9csxet.cn

[S24] C：获取本地时间
来源：http://pj.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ku.lnxyls.cn

[S25] C：内存拷贝
来源：http://yh.lnxyls.cn

memcpy(dst, src, n);
来源：http://yx.szsharing.cn

[S26] C：内存清零
来源：http://ob.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://mw.9csxet.cn

[S27] C：定义常量
来源：http://fo.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://lg.yuntaijiaju.cn

[S28] C：静态变量
来源：http://fl.panjiajie.cn

static int counter = 0;
来源：http://ue.muxihuayi.cn

[S29] C：变参函数
来源：http://nx.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sy.9csxet.cn

[S30] C：头文件保护
来源：http://io.szxytkj.cn

#ifndef X_H
来源：http://kz.nicolike.cn

#define X_H
来源：http://hc.bjjhwx.cn

#endif
来源：http://dw.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://yi.huanxung.cn

#include <iostream>
来源：http://jv.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://bd.yuntaijiaju.cn

[S32] C++：字符串
来源：http://xa.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://ew.szsharing.cn

[S33] C++：vector 增删
来源：http://gb.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ub.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://sb.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://da.nszjky.cn


<!-- 参考信息 -->