代发 wailian999

[Q65] 回滚事务
来源：http://yj.jctech888.com.cn

ROLLBACK;
来源：http://jp.gzmigu.cn

[Q66] 行锁查询
来源：http://vg.521024.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yo.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://gg.hnjuh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kd.hahajie.cn

[Q68] 保存点
来源：http://tz.bookmarksfly.cn

SAVEPOINT sp1;
来源：http://nb.haigaiapp.cn

ROLLBACK TO sp1;
来源：http://sg.asd995.cn

[Q69] 查看执行计划
来源：http://mx.huixinmuqiang.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ft.colortex.cn

[Q70] 更新统计信息
来源：http://fd.jianghongdianzi.cn

ANALYZE TABLE users;
来源：http://an.nszjky.cn

[Q71] 查看建表语句
来源：http://gc.lnxyls.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://in.muxihuayi.cn

[Q72] 查看索引
来源：http://uf.chemitech.net.cn

SHOW INDEX FROM users;
来源：http://vb.lnxyls.cn

[Q73] 查看表状态
来源：http://qi.nicolike.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ot.wgjwhj.cn

[Q74] 强制使用索引
来源：http://ss.huanxung.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cn.huanxung.cn

[Q75] 日期格式化
来源：http://vi.huixinmuqiang.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fc.gzmigu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ce.shxzskj.cn

[Q76] 按天统计
来源：http://bp.shxzskj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nk.wgjwhj.cn

[Q77] 时间加减
来源：http://md.shxzskj.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://un.jianghongdianzi.cn

[Q78] 当前时间
来源：http://zt.9csxet.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wd.panjiajie.cn

[Q79] 字符串拼接
来源：http://zf.muxihuayi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kz.szxytkj.cn

[Q80] 字符串截取
来源：http://ij.yuexingan06.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qp.panjiajie.cn

[Q81] 字符串替换
来源：http://fs.chemitech.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.muxihuayi.cn

[Q82] 字符长度与字节长度
来源：http://sh.nszjky.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pv.szsharing.cn

[Q83] 大小写转换
来源：http://vn.yuntaijiaju.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wg.nszjky.cn

[Q84] 去除首尾空格
来源：http://ge.szsharing.cn

SELECT TRIM(name) FROM users;
来源：http://fx.521024.cn

[Q85] 数值取整
来源：http://vm.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sw.bjjhwx.cn

[Q86] 读取 JSON 字段
来源：http://qo.jctech888.com.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ti.colortex.cn

[Q87] JSON 字段做条件
来源：http://ms.colortex.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ax.huixinmuqiang.cn

[Q88] 行转列（条件聚合）
来源：http://ai.521024.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fw.huixinmuqiang.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zp.lnxyls.cn

[Q89] 判断表是否存在
来源：http://gn.huixinmuqiang.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lc.hnjuh.cn

[Q90] 生成序号列
来源：http://uu.wgjwhj.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fp.jctech888.com.cn

================================================================================
来源：http://oy.yuntaijiaju.cn

R. Bash 专题
来源：http://ty.huanxung.cn

================================================================================
来源：http://hy.yuntaijiaju.cn

[R01] shebang 与严格模式
来源：http://rt.chemitech.net.cn

#!/usr/bin/env bash
来源：http://us.shtwfgs.cn

set -euo pipefail
来源：http://er.colortex.cn

[R02] 变量赋值与使用
来源：http://gd.huanxung.cn

name="Tom"; echo "$name"
来源：http://tv.lnxyls.cn

[R03] 只读变量
来源：http://xg.szxytkj.cn

readonly PI=3.14
来源：http://ae.huanxung.cn

[R04] 位置参数
来源：http://kw.chemitech.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hi.yuntaijiaju.cn

[R05] 参数默认值
来源：http://io.haigaiapp.cn

name="${1:-default}"
来源：http://op.gzmigu.cn

[R06] 判断命令是否存在
来源：http://ma.huixinmuqiang.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kq.panjiajie.cn

[R07] if 判断文件
来源：http://vp.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uk.lnxyls.cn

[R08] 数值比较
来源：http://rs.jctech888.com.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ex.panjiajie.cn

[R09] 字符串比较
来源：http://mf.nicolike.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://st.shxzukj.cn

[R10] 正则匹配
来源：http://ql.nicolike.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ln.yuexingan06.cn

[R11] case 多分支
来源：http://ak.lnxyls.cn

case "$1" in
来源：http://ap.shtwfgs.cn

start) echo "启动" ;;
来源：http://cf.shtwfgs.cn

stop)  echo "停止" ;;
来源：http://gn.colortex.cn

*)     echo "未知命令" ;;
来源：http://po.muxihuayi.cn

esac
来源：http://ye.lnxyls.cn

[R12] for 遍历文件
来源：http://kk.wgjwhj.cn

for f in *.txt; do echo "$f"; done
来源：http://uw.hnjuh.cn

[R13] for 计数循环
来源：http://yd.colortex.cn

for i in {1..10}; do echo "$i"; done
来源：http://ef.huanxung.cn

[R14] C 风格 for
来源：http://pt.szsharing.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nu.shxzskj.cn

[R15] while 逐行读文件
来源：http://zx.jianghongdianzi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dp.haigaiapp.cn

[R16] until 等待条件
来源：http://nx.nicolike.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yk.shxzukj.cn

[R17] 数组定义与取值
来源：http://nt.hahajie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eq.shxzukj.cn

[R18] 遍历数组
来源：http://dx.shtwfgs.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dp.nicolike.cn

[R19] 数组长度
来源：http://ge.haigaiapp.cn

echo "${#arr[@]}"
来源：http://xl.huanxung.cn

[R20] 关联数组（字典）
来源：http://fa.nicolike.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kg.huanxung.cn

[R21] 字符串长度
来源：http://ov.yuexingan06.cn

echo "${#s}"
来源：http://gg.hnjuh.cn

[R22] 截取子串
来源：http://uf.panjiajie.cn

echo "${s:0:5}"
来源：http://iv.jianghongdianzi.cn

[R23] 字符串替换
来源：http://dm.haigaiapp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oi.hahajie.cn

[R24] 大小写转换
来源：http://kq.bookmarksfly.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wi.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://zu.shxzskj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wf.huixinmuqiang.cn

[R26] 命令替换
来源：http://qy.yuexingan06.cn

now=$(date +%F); echo "$now"
来源：http://rb.yuntaijiaju.cn

[R27] 算术展开
来源：http://tp.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://in.yuntaijiaju.cn

[R28] 浮点运算
来源：http://ew.bookmarksfly.cn

echo "scale=2; 10/3" | bc
来源：http://mk.haigaiapp.cn

[R29] 定义函数
来源：http://qc.shxzskj.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sx.huanxung.cn

[R30] 函数返回状态码
来源：http://po.bjjhwx.cn

f() { return 0; }; f || echo "失败了"
来源：http://qp.newstarts.cn

[R31] 局部变量
来源：http://rh.szsharing.cn

f() { local x=1; echo "$x"; }
来源：http://hb.shxzskj.cn

[R32] 参数个数校验
来源：http://jz.chemitech.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eh.hahajie.cn

[R33] 捕获错误并提示行号
来源：http://pj.chemitech.net.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lg.bookmarksfly.cn

[R34] 退出时清理
来源：http://ei.haigaiapp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dv.huixinmuqiang.cn

[R35] 后台执行并等待
来源：http://qu.panjiajie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sm.szxytkj.cn

[R36] 并发执行多个任务
来源：http://nl.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yi.shxzskj.cn

[R37] 把输出赋给变量
来源：http://xv.jctech888.com.cn

files=$(ls -1)
来源：http://ce.asd995.cn

[R38] 管道串联
来源：http://rt.asd995.cn

cat a.txt | grep -i error | wc -l
来源：http://dm.huixiangedu.cn

[R39] 重定向标准输出与错误
来源：http://jr.haigaiapp.cn

cmd > out.log 2>&1
来源：http://fm.shxzukj.cn

[R40] 追加写日志
来源：http://uh.521024.cn

echo "log" >> out.log
来源：http://pe.muxihuayi.cn

[R41] 丢弃输出
来源：http://ez.hahajie.cn

cmd >/dev/null 2>&1
来源：http://xo.jianghongdianzi.cn

[R42] 输入重定向
来源：http://uj.huixinmuqiang.cn

wc -l < a.txt
来源：http://ua.jctech888.com.cn

[R43] 按名字查找文件
来源：http://lx.szsharing.cn

find . -name "*.log" -type f
来源：http://vj.gzmigu.cn

[R44] 按修改时间查找
来源：http://gb.jctech888.com.cn

find . -mtime -7 -type f
来源：http://bw.nicolike.cn

[R45] 批量删除
来源：http://lt.newstarts.cn

find . -name "*.tmp" -delete
来源：http://tr.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://uy.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cd.panjiajie.cn

[R47] sed 单行替换
来源：http://wx.nicolike.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hr.yuntaijiaju.cn

[R48] awk 取指定列
来源：http://zb.huanxung.cn

awk '{print $1, $3}' a.txt
来源：http://nz.jianghongdianzi.cn

[R49] awk 带条件
来源：http://se.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ho.szxytkj.cn

[R50] awk 求和
来源：http://ma.huixiangedu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sf.szxytkj.cn

[R51] 排序去重取前几
来源：http://xa.muxihuayi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://di.nicolike.cn

[R52] 统计行数
来源：http://xs.newstarts.cn

wc -l a.txt
来源：http://do.bjjhwx.cn

[R53] 查看文件头与实时尾
来源：http://lq.muxihuayi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eu.521024.cn

[R54] 比较两个文件
来源：http://qz.huanxung.cn

diff a.txt b.txt
来源：http://lh.shtwfgs.cn

[R55] 压缩与解压
来源：http://co.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qi.szxytkj.cn

[R56] 远程拷贝
来源：http://ez.newstarts.cn

scp file user@host:/path/
来源：http://se.chemitech.net.cn

[R57] 远程执行命令
来源：http://lg.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://sp.hahajie.cn

[R58] 下载文件
来源：http://bv.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oa.hnjuh.cn

[R59] 发 POST JSON
来源：http://fa.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hl.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://mb.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ja.shxzukj.cn

[R61] 磁盘占用
来源：http://zy.shtwfgs.cn

df -h;  du -sh *
来源：http://mp.colortex.cn

[R62] 找最占空间的文件
来源：http://yn.colortex.cn

du -ah . | sort -rh | head -10
来源：http://eh.huixinmuqiang.cn

[R63] 内存与进程
来源：http://fc.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://bw.shxzskj.cn

[R64] 结束进程
来源：http://xp.lnxyls.cn

kill -9 $(pgrep -f app.py)
来源：http://va.jctech888.com.cn

[R65] 查看端口占用
来源：http://np.shxzukj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ed.9csxet.cn

[R66] 定时任务
来源：http://re.haigaiapp.cn

crontab -e;  crontab -l
来源：http://nh.bookmarksfly.cn

[R67] 生成随机十六进制串
来源：http://eq.shxzukj.cn

openssl rand -hex 16
来源：http://ef.shxzskj.cn

[R68] 计算文件校验值
来源：http://hx.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yj.lnxyls.cn

[R69] 生成随机密码
来源：http://uf.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://ga.shxzukj.cn

[R70] 时间戳与互转
来源：http://yo.colortex.cn

date +%s;  date -d @1700000000
来源：http://fi.hnjuh.cn

[R71] 日期格式化
来源：http://yr.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uj.newstarts.cn

[R72] 等待端口就绪
来源：http://nr.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://am.bookmarksfly.cn

[R73] 分割大日志
来源：http://tj.nicolike.cn

split -l 1000 big.log part_
来源：http://ya.nicolike.cn

[R74] 批量重命名
来源：http://ul.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ry.shtwfgs.cn

[R75] 导出环境变量
来源：http://ax.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://vg.shxzskj.cn

[R76] 使用临时文件
来源：http://wr.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mj.panjiajie.cn

[R77] 读取用户输入
来源：http://jd.asd995.cn

read -rp "请输入: " ans
来源：http://yy.huanxung.cn

[R78] 交互式菜单
来源：http://ip.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jr.newstarts.cn

[R79] 解析命令行选项
来源：http://tv.wgjwhj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vl.shxzskj.cn

[R80] 查看脚本执行耗时
来源：http://ax.muxihuayi.cn

time ./run.sh
来源：http://ta.hahajie.cn

================================================================================
来源：http://oe.shxzukj.cn

S. C / C++ 专题
来源：http://bd.hahajie.cn

================================================================================
来源：http://qv.panjiajie.cn

[S01] C：Hello World
来源：http://rk.panjiajie.cn

#include <stdio.h>
来源：http://ig.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tq.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://fc.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://ly.szsharing.cn

[S03] C：读入整数
来源：http://bc.9csxet.cn

int x; scanf("%d", &x);
来源：http://ib.yuexingan06.cn

[S04] C：字符串复制
来源：http://ch.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gc.chemitech.net.cn

[S05] C：字符串长度
来源：http://wo.hahajie.cn

strlen(s)
来源：http://xg.colortex.cn

[S06] C：字符串比较
来源：http://fr.jctech888.com.cn

strcmp(a, b) == 0
来源：http://xa.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://bn.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://my.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://lu.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tb.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://wo.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tc.nicolike.cn

[S10] C：指针与解引用
来源：http://vr.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://ge.panjiajie.cn

[S11] C：逐行读文件
来源：http://tj.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://so.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://if.shtwfgs.cn

fclose(f);
来源：http://ip.shxzukj.cn

[S12] C：写文件
来源：http://kv.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ul.521024.cn

[S13] C：宏定义
来源：http://ud.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ap.shxzukj.cn

[S14] C：枚举
来源：http://rh.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://qw.chemitech.net.cn

[S15] C：类型转换
来源：http://hi.haigaiapp.cn

(double) a / b
来源：http://wa.asd995.cn

[S16] C：位操作置位
来源：http://uq.panjiajie.cn

x |= (1 << 3);
来源：http://wg.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://dl.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zx.jctech888.com.cn

[S18] C：命令行参数
来源：http://jr.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://vw.szxytkj.cn

[S19] C：快速排序
来源：http://ph.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sl.yuexingan06.cn

[S20] C：二分查找
来源：http://nx.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ac.shxzskj.cn

[S21] C：字符类别判断
来源：http://so.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kd.chemitech.net.cn

[S22] C：字符串转数字
来源：http://yf.chemitech.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pg.huanxung.cn

[S23] C：随机数
来源：http://pd.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fi.chemitech.net.cn

[S24] C：获取本地时间
来源：http://sg.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://si.shxzukj.cn

[S25] C：内存拷贝
来源：http://vy.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ql.shtwfgs.cn

[S26] C：内存清零
来源：http://fq.asd995.cn

memset(a, 0, sizeof a);
来源：http://ns.muxihuayi.cn

[S27] C：定义常量
来源：http://hs.muxihuayi.cn

const double PI = 3.14159;
来源：http://bf.yuexingan06.cn

[S28] C：静态变量
来源：http://jy.huixiangedu.cn

static int counter = 0;
来源：http://oh.chemitech.net.cn

[S29] C：变参函数
来源：http://pr.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fi.huixiangedu.cn

[S30] C：头文件保护
来源：http://qd.szxytkj.cn

#ifndef X_H
来源：http://ez.shxzukj.cn

#define X_H
来源：http://cm.shxzskj.cn

#endif
来源：http://kt.szsharing.cn

[S31] C++：Hello World
来源：http://ao.szxytkj.cn

#include <iostream>
来源：http://gu.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://db.521024.cn

[S32] C++：字符串
来源：http://qe.colortex.cn

std::string s = "hi";  s += "!";
来源：http://mt.9csxet.cn

[S33] C++：vector 增删
来源：http://ga.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wd.gzmigu.cn

[S34] C++：遍历 vector
来源：http://xg.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://ob.lnxyls.cn


<!-- 参考信息 -->