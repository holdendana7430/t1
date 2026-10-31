代发 wailian999

[Q67] 设置隔离级别
来源：http://sg.shtwfgs.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bd.haigaiapp.cn

[Q68] 保存点
来源：http://rv.muxihuayi.cn

SAVEPOINT sp1;
来源：http://ov.shxzukj.cn

ROLLBACK TO sp1;
来源：http://fr.shtwfgs.cn

[Q69] 查看执行计划
来源：http://zx.9csxet.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hy.wgjwhj.cn

[Q70] 更新统计信息
来源：http://nb.hahajie.cn

ANALYZE TABLE users;
来源：http://kv.haigaiapp.cn

[Q71] 查看建表语句
来源：http://pc.newstarts.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ow.szxytkj.cn

[Q72] 查看索引
来源：http://gk.yuntaijiaju.cn

SHOW INDEX FROM users;
来源：http://zy.wgjwhj.cn

[Q73] 查看表状态
来源：http://fj.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qk.huanxung.cn

[Q74] 强制使用索引
来源：http://ea.shxzskj.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rm.huixiangedu.cn

[Q75] 日期格式化
来源：http://ro.asd995.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://of.yuexingan06.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vh.colortex.cn

[Q76] 按天统计
来源：http://su.chemitech.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://co.szsharing.cn

[Q77] 时间加减
来源：http://nu.wgjwhj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://et.szxytkj.cn

[Q78] 当前时间
来源：http://ia.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ba.muxihuayi.cn

[Q79] 字符串拼接
来源：http://br.newstarts.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uy.gzmigu.cn

[Q80] 字符串截取
来源：http://gp.shtwfgs.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cy.gzmigu.cn

[Q81] 字符串替换
来源：http://it.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xk.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://yf.huixiangedu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jy.huanxung.cn

[Q83] 大小写转换
来源：http://dw.hahajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ua.panjiajie.cn

[Q84] 去除首尾空格
来源：http://as.szxytkj.cn

SELECT TRIM(name) FROM users;
来源：http://hz.jctech888.com.cn

[Q85] 数值取整
来源：http://cp.gzmigu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vx.gzmigu.cn

[Q86] 读取 JSON 字段
来源：http://cn.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ro.muxihuayi.cn

[Q87] JSON 字段做条件
来源：http://yc.gzmigu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pi.jianghongdianzi.cn

[Q88] 行转列（条件聚合）
来源：http://hw.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lx.asd995.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zl.wgjwhj.cn

[Q89] 判断表是否存在
来源：http://zg.shxzskj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lr.yuntaijiaju.cn

[Q90] 生成序号列
来源：http://yd.shtwfgs.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tt.muxihuayi.cn

================================================================================
来源：http://cy.bookmarksfly.cn

R. Bash 专题
来源：http://fs.panjiajie.cn

================================================================================
来源：http://ob.huixinmuqiang.cn

[R01] shebang 与严格模式
来源：http://ax.wgjwhj.cn

#!/usr/bin/env bash
来源：http://of.shtwfgs.cn

set -euo pipefail
来源：http://vl.shtwfgs.cn

[R02] 变量赋值与使用
来源：http://qb.huixiangedu.cn

name="Tom"; echo "$name"
来源：http://ht.szxytkj.cn

[R03] 只读变量
来源：http://en.shxzukj.cn

readonly PI=3.14
来源：http://zo.yuexingan06.cn

[R04] 位置参数
来源：http://mt.nicolike.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qe.newstarts.cn

[R05] 参数默认值
来源：http://tw.yuntaijiaju.cn

name="${1:-default}"
来源：http://gi.jianghongdianzi.cn

[R06] 判断命令是否存在
来源：http://pt.muxihuayi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bn.chemitech.net.cn

[R07] if 判断文件
来源：http://hl.huixinmuqiang.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jm.jianghongdianzi.cn

[R08] 数值比较
来源：http://cv.bookmarksfly.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fh.yuntaijiaju.cn

[R09] 字符串比较
来源：http://oo.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qm.newstarts.cn

[R10] 正则匹配
来源：http://xp.bookmarksfly.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fj.hnjuh.cn

[R11] case 多分支
来源：http://dn.yuexingan06.cn

case "$1" in
来源：http://jc.huixinmuqiang.cn

start) echo "启动" ;;
来源：http://gh.huanxung.cn

stop)  echo "停止" ;;
来源：http://tm.haigaiapp.cn

*)     echo "未知命令" ;;
来源：http://uz.bookmarksfly.cn

esac
来源：http://vc.panjiajie.cn

[R12] for 遍历文件
来源：http://at.hnjuh.cn

for f in *.txt; do echo "$f"; done
来源：http://dz.panjiajie.cn

[R13] for 计数循环
来源：http://sm.haigaiapp.cn

for i in {1..10}; do echo "$i"; done
来源：http://ry.huixinmuqiang.cn

[R14] C 风格 for
来源：http://yo.wgjwhj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bp.nicolike.cn

[R15] while 逐行读文件
来源：http://ry.bjjhwx.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kv.yuntaijiaju.cn

[R16] until 等待条件
来源：http://ar.jianghongdianzi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://at.asd995.cn

[R17] 数组定义与取值
来源：http://hw.shtwfgs.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rm.szxytkj.cn

[R18] 遍历数组
来源：http://ml.bjjhwx.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zi.hnjuh.cn

[R19] 数组长度
来源：http://on.panjiajie.cn

echo "${#arr[@]}"
来源：http://at.yuexingan06.cn

[R20] 关联数组（字典）
来源：http://km.muxihuayi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wh.panjiajie.cn

[R21] 字符串长度
来源：http://bg.jctech888.com.cn

echo "${#s}"
来源：http://zi.szxytkj.cn

[R22] 截取子串
来源：http://io.shxzskj.cn

echo "${s:0:5}"
来源：http://ii.muxihuayi.cn

[R23] 字符串替换
来源：http://lp.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ha.szsharing.cn

[R24] 大小写转换
来源：http://gc.asd995.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iq.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://fy.nicolike.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ty.colortex.cn

[R26] 命令替换
来源：http://dv.muxihuayi.cn

now=$(date +%F); echo "$now"
来源：http://qv.jianghongdianzi.cn

[R27] 算术展开
来源：http://fp.asd995.cn

echo $((1 + 2 * 3))
来源：http://ty.yuexingan06.cn

[R28] 浮点运算
来源：http://sj.yuntaijiaju.cn

echo "scale=2; 10/3" | bc
来源：http://xq.jianghongdianzi.cn

[R29] 定义函数
来源：http://ob.bookmarksfly.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mx.panjiajie.cn

[R30] 函数返回状态码
来源：http://mz.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://md.shtwfgs.cn

[R31] 局部变量
来源：http://nm.bookmarksfly.cn

f() { local x=1; echo "$x"; }
来源：http://sv.yuexingan06.cn

[R32] 参数个数校验
来源：http://fy.haigaiapp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sv.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://vi.gzmigu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nh.jctech888.com.cn

[R34] 退出时清理
来源：http://ui.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lw.shxzskj.cn

[R35] 后台执行并等待
来源：http://vu.jianghongdianzi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://eo.shtwfgs.cn

[R36] 并发执行多个任务
来源：http://nd.szsharing.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nw.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://el.521024.cn

files=$(ls -1)
来源：http://hq.haigaiapp.cn

[R38] 管道串联
来源：http://oz.yuntaijiaju.cn

cat a.txt | grep -i error | wc -l
来源：http://yn.bookmarksfly.cn

[R39] 重定向标准输出与错误
来源：http://ji.shxzukj.cn

cmd > out.log 2>&1
来源：http://px.chemitech.net.cn

[R40] 追加写日志
来源：http://tl.jctech888.com.cn

echo "log" >> out.log
来源：http://ul.huixiangedu.cn

[R41] 丢弃输出
来源：http://cw.muxihuayi.cn

cmd >/dev/null 2>&1
来源：http://ie.yuntaijiaju.cn

[R42] 输入重定向
来源：http://uf.shxzskj.cn

wc -l < a.txt
来源：http://pc.lnxyls.cn

[R43] 按名字查找文件
来源：http://me.hahajie.cn

find . -name "*.log" -type f
来源：http://fg.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://ga.lnxyls.cn

find . -mtime -7 -type f
来源：http://nc.nszjky.cn

[R45] 批量删除
来源：http://wi.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://jb.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://xy.muxihuayi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ap.chemitech.net.cn

[R47] sed 单行替换
来源：http://sh.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ln.hnjuh.cn

[R48] awk 取指定列
来源：http://rk.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://mo.huanxung.cn

[R49] awk 带条件
来源：http://ab.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vx.gzmigu.cn

[R50] awk 求和
来源：http://mu.hnjuh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ph.bjjhwx.cn

[R51] 排序去重取前几
来源：http://lf.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vc.muxihuayi.cn

[R52] 统计行数
来源：http://tf.wgjwhj.cn

wc -l a.txt
来源：http://da.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://vj.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yy.huixinmuqiang.cn

[R54] 比较两个文件
来源：http://wm.hnjuh.cn

diff a.txt b.txt
来源：http://ok.szsharing.cn

[R55] 压缩与解压
来源：http://oz.yuntaijiaju.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hy.muxihuayi.cn

[R56] 远程拷贝
来源：http://vi.shxzukj.cn

scp file user@host:/path/
来源：http://td.hnjuh.cn

[R57] 远程执行命令
来源：http://fm.szxytkj.cn

ssh user@host 'uptime'
来源：http://du.muxihuayi.cn

[R58] 下载文件
来源：http://vz.chemitech.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://se.521024.cn

[R59] 发 POST JSON
来源：http://ui.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nd.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://jn.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uv.panjiajie.cn

[R61] 磁盘占用
来源：http://xr.wgjwhj.cn

df -h;  du -sh *
来源：http://sd.lnxyls.cn

[R62] 找最占空间的文件
来源：http://bu.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://fg.bjjhwx.cn

[R63] 内存与进程
来源：http://fq.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://lv.muxihuayi.cn

[R64] 结束进程
来源：http://ef.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://xz.9csxet.cn

[R65] 查看端口占用
来源：http://tl.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://df.jianghongdianzi.cn

[R66] 定时任务
来源：http://kn.colortex.cn

crontab -e;  crontab -l
来源：http://ny.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://xh.muxihuayi.cn

openssl rand -hex 16
来源：http://jq.yuexingan06.cn

[R68] 计算文件校验值
来源：http://vx.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ag.chemitech.net.cn

[R69] 生成随机密码
来源：http://lk.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ln.shxzukj.cn

[R70] 时间戳与互转
来源：http://kv.asd995.cn

date +%s;  date -d @1700000000
来源：http://cv.bookmarksfly.cn

[R71] 日期格式化
来源：http://sa.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fn.yuntaijiaju.cn

[R72] 等待端口就绪
来源：http://cx.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mi.bjjhwx.cn

[R73] 分割大日志
来源：http://ub.szsharing.cn

split -l 1000 big.log part_
来源：http://dl.szsharing.cn

[R74] 批量重命名
来源：http://kl.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dg.hahajie.cn

[R75] 导出环境变量
来源：http://av.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://th.hahajie.cn

[R76] 使用临时文件
来源：http://bw.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lh.hahajie.cn

[R77] 读取用户输入
来源：http://jf.chemitech.net.cn

read -rp "请输入: " ans
来源：http://zn.huixiangedu.cn

[R78] 交互式菜单
来源：http://od.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dl.wgjwhj.cn

[R79] 解析命令行选项
来源：http://fa.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dv.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://ve.muxihuayi.cn

time ./run.sh
来源：http://ny.bjjhwx.cn

================================================================================
来源：http://hm.chemitech.net.cn

S. C / C++ 专题
来源：http://en.jctech888.com.cn

================================================================================
来源：http://kt.huixinmuqiang.cn

[S01] C：Hello World
来源：http://ey.bookmarksfly.cn

#include <stdio.h>
来源：http://bj.shtwfgs.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gh.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://wd.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://jo.yuntaijiaju.cn

[S03] C：读入整数
来源：http://ie.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://yx.yuexingan06.cn

[S04] C：字符串复制
来源：http://xt.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pd.nszjky.cn

[S05] C：字符串长度
来源：http://sx.shxzukj.cn

strlen(s)
来源：http://jr.shxzskj.cn

[S06] C：字符串比较
来源：http://op.chemitech.net.cn

strcmp(a, b) == 0
来源：http://hr.hahajie.cn

[S07] C：数组遍历求和
来源：http://qk.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qt.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://zk.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ca.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://xw.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xw.bjjhwx.cn

[S10] C：指针与解引用
来源：http://dk.9csxet.cn

int *p = &a;  *p = 5;
来源：http://wr.bjjhwx.cn

[S11] C：逐行读文件
来源：http://dr.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://ve.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iu.wgjwhj.cn

fclose(f);
来源：http://ls.bjjhwx.cn

[S12] C：写文件
来源：http://ss.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dw.jianghongdianzi.cn

[S13] C：宏定义
来源：http://go.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uw.jctech888.com.cn

[S14] C：枚举
来源：http://bx.asd995.cn

enum Color { RED, GREEN, BLUE };
来源：http://ym.shxzskj.cn

[S15] C：类型转换
来源：http://rf.asd995.cn

(double) a / b
来源：http://tt.szxytkj.cn

[S16] C：位操作置位
来源：http://ab.huanxung.cn

x |= (1 << 3);
来源：http://om.hahajie.cn

[S17] C：安全拼接字符串
来源：http://rv.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hj.wgjwhj.cn

[S18] C：命令行参数
来源：http://ta.gzmigu.cn

int main(int argc, char **argv)
来源：http://hk.asd995.cn

[S19] C：快速排序
来源：http://jv.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vt.huixiangedu.cn

[S20] C：二分查找
来源：http://fx.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mi.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://xm.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eh.shxzskj.cn

[S22] C：字符串转数字
来源：http://vm.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ub.hahajie.cn

[S23] C：随机数
来源：http://pv.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qh.haigaiapp.cn

[S24] C：获取本地时间
来源：http://sl.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gt.szxytkj.cn

[S25] C：内存拷贝
来源：http://jp.shxzukj.cn

memcpy(dst, src, n);
来源：http://hz.gzmigu.cn

[S26] C：内存清零
来源：http://rt.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://re.huixiangedu.cn

[S27] C：定义常量
来源：http://ct.hahajie.cn

const double PI = 3.14159;
来源：http://go.hnjuh.cn

[S28] C：静态变量
来源：http://jr.nicolike.cn

static int counter = 0;
来源：http://mr.jianghongdianzi.cn

[S29] C：变参函数
来源：http://vr.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ck.bjjhwx.cn

[S30] C：头文件保护
来源：http://mw.bookmarksfly.cn

#ifndef X_H
来源：http://hs.jianghongdianzi.cn

#define X_H
来源：http://fo.panjiajie.cn

#endif
来源：http://cd.bjjhwx.cn

[S31] C++：Hello World
来源：http://ju.szxytkj.cn

#include <iostream>
来源：http://sq.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://yi.panjiajie.cn

[S32] C++：字符串
来源：http://bw.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://jq.muxihuayi.cn

[S33] C++：vector 增删
来源：http://uf.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ct.huanxung.cn

[S34] C++：遍历 vector
来源：http://mb.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gf.nszjky.cn

[S35] C++：map
来源：http://jk.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://is.panjiajie.cn

[S36] C++：unordered_map
来源：http://wr.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xr.szxytkj.cn


<!-- 参考信息 -->