代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sv.szxytkj.cn

[Q60] 取上一行 / 下一行
来源：http://px.9csxet.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gc.huixiangedu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://en.huanxung.cn

[Q61] 移动平均
来源：http://qa.newstarts.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nc.nszjky.cn

[Q62] 分组占比
来源：http://uq.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pp.shxzukj.cn

[Q63] 开启事务
来源：http://ap.newstarts.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ut.bookmarksfly.cn

[Q64] 提交事务
来源：http://lv.hahajie.cn

COMMIT;
来源：http://cu.muxihuayi.cn

[Q65] 回滚事务
来源：http://do.jctech888.com.cn

ROLLBACK;
来源：http://sf.huixiangedu.cn

[Q66] 行锁查询
来源：http://ep.nicolike.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xo.haigaiapp.cn

[Q67] 设置隔离级别
来源：http://zs.wgjwhj.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cf.huanxung.cn

[Q68] 保存点
来源：http://ap.szxytkj.cn

SAVEPOINT sp1;
来源：http://sf.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://zx.yuexingan06.cn

[Q69] 查看执行计划
来源：http://xv.yuexingan06.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zp.9csxet.cn

[Q70] 更新统计信息
来源：http://py.shxzukj.cn

ANALYZE TABLE users;
来源：http://yi.szsharing.cn

[Q71] 查看建表语句
来源：http://ow.521024.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iv.asd995.cn

[Q72] 查看索引
来源：http://uh.szxytkj.cn

SHOW INDEX FROM users;
来源：http://fv.shtwfgs.cn

[Q73] 查看表状态
来源：http://lm.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mf.chemitech.net.cn

[Q74] 强制使用索引
来源：http://ew.panjiajie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ry.bjjhwx.cn

[Q75] 日期格式化
来源：http://xd.shxzskj.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yj.shxzukj.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ig.lnxyls.cn

[Q76] 按天统计
来源：http://ub.wgjwhj.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jx.newstarts.cn

[Q77] 时间加减
来源：http://vb.colortex.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qi.huixiangedu.cn

[Q78] 当前时间
来源：http://dg.nszjky.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mb.szxytkj.cn

[Q79] 字符串拼接
来源：http://hv.yuexingan06.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nl.chemitech.net.cn

[Q80] 字符串截取
来源：http://ii.wgjwhj.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ui.huixinmuqiang.cn

[Q81] 字符串替换
来源：http://ls.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hm.jianghongdianzi.cn

[Q82] 字符长度与字节长度
来源：http://qs.lnxyls.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://af.521024.cn

[Q83] 大小写转换
来源：http://kv.haigaiapp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://en.hnjuh.cn

[Q84] 去除首尾空格
来源：http://zr.nicolike.cn

SELECT TRIM(name) FROM users;
来源：http://ae.jianghongdianzi.cn

[Q85] 数值取整
来源：http://me.muxihuayi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vd.shxzskj.cn

[Q86] 读取 JSON 字段
来源：http://tv.jianghongdianzi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ks.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://fz.jctech888.com.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ji.panjiajie.cn

[Q88] 行转列（条件聚合）
来源：http://pg.newstarts.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rd.shxzukj.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.szxytkj.cn

[Q89] 判断表是否存在
来源：http://tk.bjjhwx.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nc.nicolike.cn

[Q90] 生成序号列
来源：http://ml.bjjhwx.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dm.521024.cn

================================================================================
来源：http://xr.nicolike.cn

R. Bash 专题
来源：http://vx.shxzukj.cn

================================================================================
来源：http://ea.shxzskj.cn

[R01] shebang 与严格模式
来源：http://ua.huanxung.cn

#!/usr/bin/env bash
来源：http://tt.huixinmuqiang.cn

set -euo pipefail
来源：http://df.shxzskj.cn

[R02] 变量赋值与使用
来源：http://aw.haigaiapp.cn

name="Tom"; echo "$name"
来源：http://ry.szsharing.cn

[R03] 只读变量
来源：http://cl.panjiajie.cn

readonly PI=3.14
来源：http://ds.jctech888.com.cn

[R04] 位置参数
来源：http://nl.bookmarksfly.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tt.bookmarksfly.cn

[R05] 参数默认值
来源：http://se.yuntaijiaju.cn

name="${1:-default}"
来源：http://ke.shtwfgs.cn

[R06] 判断命令是否存在
来源：http://ry.shtwfgs.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fa.panjiajie.cn

[R07] if 判断文件
来源：http://ea.shxzskj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ev.panjiajie.cn

[R08] 数值比较
来源：http://wg.lnxyls.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mx.newstarts.cn

[R09] 字符串比较
来源：http://pc.bjjhwx.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tn.newstarts.cn

[R10] 正则匹配
来源：http://yf.szxytkj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pk.huanxung.cn

[R11] case 多分支
来源：http://sl.yuntaijiaju.cn

case "$1" in
来源：http://jo.yuexingan06.cn

start) echo "启动" ;;
来源：http://nj.bjjhwx.cn

stop)  echo "停止" ;;
来源：http://na.huixinmuqiang.cn

*)     echo "未知命令" ;;
来源：http://jl.nszjky.cn

esac
来源：http://sg.muxihuayi.cn

[R12] for 遍历文件
来源：http://gq.huanxung.cn

for f in *.txt; do echo "$f"; done
来源：http://sv.yuntaijiaju.cn

[R13] for 计数循环
来源：http://qs.wgjwhj.cn

for i in {1..10}; do echo "$i"; done
来源：http://ca.jctech888.com.cn

[R14] C 风格 for
来源：http://kj.gzmigu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wy.nszjky.cn

[R15] while 逐行读文件
来源：http://fz.shxzskj.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vw.9csxet.cn

[R16] until 等待条件
来源：http://ew.haigaiapp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gf.lnxyls.cn

[R17] 数组定义与取值
来源：http://em.shxzukj.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uu.haigaiapp.cn

[R18] 遍历数组
来源：http://ra.hahajie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ga.yuntaijiaju.cn

[R19] 数组长度
来源：http://ot.shxzskj.cn

echo "${#arr[@]}"
来源：http://cl.muxihuayi.cn

[R20] 关联数组（字典）
来源：http://dq.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eo.chemitech.net.cn

[R21] 字符串长度
来源：http://gi.huixiangedu.cn

echo "${#s}"
来源：http://tq.jianghongdianzi.cn

[R22] 截取子串
来源：http://dm.hnjuh.cn

echo "${s:0:5}"
来源：http://lr.shxzukj.cn

[R23] 字符串替换
来源：http://xe.szsharing.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ak.huanxung.cn

[R24] 大小写转换
来源：http://fj.huixinmuqiang.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qq.gzmigu.cn

[R25] 去后缀 / 去前缀
来源：http://mv.asd995.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wt.haigaiapp.cn

[R26] 命令替换
来源：http://lx.shxzskj.cn

now=$(date +%F); echo "$now"
来源：http://rk.wgjwhj.cn

[R27] 算术展开
来源：http://xs.hnjuh.cn

echo $((1 + 2 * 3))
来源：http://bc.nicolike.cn

[R28] 浮点运算
来源：http://li.9csxet.cn

echo "scale=2; 10/3" | bc
来源：http://sm.newstarts.cn

[R29] 定义函数
来源：http://cx.hahajie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xb.asd995.cn

[R30] 函数返回状态码
来源：http://ib.szxytkj.cn

f() { return 0; }; f || echo "失败了"
来源：http://jx.bookmarksfly.cn

[R31] 局部变量
来源：http://zt.huixinmuqiang.cn

f() { local x=1; echo "$x"; }
来源：http://bb.huixiangedu.cn

[R32] 参数个数校验
来源：http://xs.yuntaijiaju.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://og.haigaiapp.cn

[R33] 捕获错误并提示行号
来源：http://ud.haigaiapp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bz.yuexingan06.cn

[R34] 退出时清理
来源：http://ya.wgjwhj.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iq.asd995.cn

[R35] 后台执行并等待
来源：http://vj.lnxyls.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tj.huixinmuqiang.cn

[R36] 并发执行多个任务
来源：http://ga.yuntaijiaju.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ur.haigaiapp.cn

[R37] 把输出赋给变量
来源：http://ba.shxzukj.cn

files=$(ls -1)
来源：http://fn.colortex.cn

[R38] 管道串联
来源：http://nk.chemitech.net.cn

cat a.txt | grep -i error | wc -l
来源：http://gt.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://gt.hnjuh.cn

cmd > out.log 2>&1
来源：http://uf.jianghongdianzi.cn

[R40] 追加写日志
来源：http://qa.wgjwhj.cn

echo "log" >> out.log
来源：http://dx.asd995.cn

[R41] 丢弃输出
来源：http://lf.chemitech.net.cn

cmd >/dev/null 2>&1
来源：http://qf.wgjwhj.cn

[R42] 输入重定向
来源：http://rt.huixiangedu.cn

wc -l < a.txt
来源：http://xs.jctech888.com.cn

[R43] 按名字查找文件
来源：http://xt.lnxyls.cn

find . -name "*.log" -type f
来源：http://kb.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://mm.lnxyls.cn

find . -mtime -7 -type f
来源：http://ew.hnjuh.cn

[R45] 批量删除
来源：http://ho.gzmigu.cn

find . -name "*.tmp" -delete
来源：http://hf.wgjwhj.cn

[R46] 递归替换文件内容
来源：http://bt.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ew.gzmigu.cn

[R47] sed 单行替换
来源：http://oo.nszjky.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pf.newstarts.cn

[R48] awk 取指定列
来源：http://hy.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://hn.szsharing.cn

[R49] awk 带条件
来源：http://wi.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mo.jctech888.com.cn

[R50] awk 求和
来源：http://fy.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xx.hahajie.cn

[R51] 排序去重取前几
来源：http://dk.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lr.bookmarksfly.cn

[R52] 统计行数
来源：http://ua.chemitech.net.cn

wc -l a.txt
来源：http://qn.521024.cn

[R53] 查看文件头与实时尾
来源：http://ov.huixinmuqiang.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pf.yuexingan06.cn

[R54] 比较两个文件
来源：http://ua.gzmigu.cn

diff a.txt b.txt
来源：http://yv.bookmarksfly.cn

[R55] 压缩与解压
来源：http://gi.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wf.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://cy.bjjhwx.cn

scp file user@host:/path/
来源：http://qc.szxytkj.cn

[R57] 远程执行命令
来源：http://za.bjjhwx.cn

ssh user@host 'uptime'
来源：http://bt.newstarts.cn

[R58] 下载文件
来源：http://mm.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ok.wgjwhj.cn

[R59] 发 POST JSON
来源：http://sy.hnjuh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bk.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://dz.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://de.hnjuh.cn

[R61] 磁盘占用
来源：http://la.yuntaijiaju.cn

df -h;  du -sh *
来源：http://bf.shxzukj.cn

[R62] 找最占空间的文件
来源：http://qm.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ev.wgjwhj.cn

[R63] 内存与进程
来源：http://hx.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://ck.huixiangedu.cn

[R64] 结束进程
来源：http://lp.shtwfgs.cn

kill -9 $(pgrep -f app.py)
来源：http://ub.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://yb.panjiajie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wq.gzmigu.cn

[R66] 定时任务
来源：http://uj.haigaiapp.cn

crontab -e;  crontab -l
来源：http://rk.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://mc.jianghongdianzi.cn

openssl rand -hex 16
来源：http://rf.asd995.cn

[R68] 计算文件校验值
来源：http://jz.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jt.muxihuayi.cn

[R69] 生成随机密码
来源：http://oy.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://gf.shtwfgs.cn

[R70] 时间戳与互转
来源：http://yr.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://tu.huixinmuqiang.cn

[R71] 日期格式化
来源：http://dw.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ul.szsharing.cn

[R72] 等待端口就绪
来源：http://ss.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uj.colortex.cn

[R73] 分割大日志
来源：http://xl.shtwfgs.cn

split -l 1000 big.log part_
来源：http://gk.huixiangedu.cn

[R74] 批量重命名
来源：http://yx.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gq.shtwfgs.cn

[R75] 导出环境变量
来源：http://oq.yuexingan06.cn

export PATH="$HOME/bin:$PATH"
来源：http://vj.chemitech.net.cn

[R76] 使用临时文件
来源：http://nm.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tb.colortex.cn

[R77] 读取用户输入
来源：http://xa.shxzskj.cn

read -rp "请输入: " ans
来源：http://vr.jctech888.com.cn

[R78] 交互式菜单
来源：http://vs.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ol.gzmigu.cn

[R79] 解析命令行选项
来源：http://hp.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zd.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://zo.chemitech.net.cn

time ./run.sh
来源：http://ww.yuntaijiaju.cn

================================================================================
来源：http://cm.jianghongdianzi.cn

S. C / C++ 专题
来源：http://xp.jctech888.com.cn

================================================================================
来源：http://uj.shxzskj.cn

[S01] C：Hello World
来源：http://iy.huanxung.cn

#include <stdio.h>
来源：http://tp.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qf.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://nz.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ma.yuexingan06.cn

[S03] C：读入整数
来源：http://ko.hahajie.cn

int x; scanf("%d", &x);
来源：http://yp.hnjuh.cn

[S04] C：字符串复制
来源：http://ys.lnxyls.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jx.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://lr.hnjuh.cn

strlen(s)
来源：http://ou.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://wx.nicolike.cn

strcmp(a, b) == 0
来源：http://ut.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://po.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ho.colortex.cn

[S08] C：动态内存分配与释放
来源：http://ra.shxzskj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rn.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://cg.hnjuh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mu.yuexingan06.cn

[S10] C：指针与解引用
来源：http://ky.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://kj.szxytkj.cn

[S11] C：逐行读文件
来源：http://ux.shtwfgs.cn

FILE *f = fopen("a.txt", "r");
来源：http://na.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tf.szsharing.cn

fclose(f);
来源：http://wb.szxytkj.cn

[S12] C：写文件
来源：http://bx.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xk.colortex.cn

[S13] C：宏定义
来源：http://xk.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ix.huixiangedu.cn

[S14] C：枚举
来源：http://am.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://ns.haigaiapp.cn

[S15] C：类型转换
来源：http://ff.asd995.cn

(double) a / b
来源：http://am.lnxyls.cn

[S16] C：位操作置位
来源：http://uu.shxzskj.cn

x |= (1 << 3);
来源：http://rl.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://gt.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pg.nicolike.cn

[S18] C：命令行参数
来源：http://bu.521024.cn

int main(int argc, char **argv)
来源：http://to.haigaiapp.cn

[S19] C：快速排序
来源：http://jj.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dn.yuexingan06.cn

[S20] C：二分查找
来源：http://wn.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wk.panjiajie.cn

[S21] C：字符类别判断
来源：http://uy.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://om.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://tb.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://md.9csxet.cn

[S23] C：随机数
来源：http://lh.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fy.shxzukj.cn

[S24] C：获取本地时间
来源：http://db.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dq.huanxung.cn

[S25] C：内存拷贝
来源：http://yy.huixiangedu.cn

memcpy(dst, src, n);
来源：http://dm.szxytkj.cn

[S26] C：内存清零
来源：http://kg.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://zr.huixinmuqiang.cn

[S27] C：定义常量
来源：http://so.hnjuh.cn

const double PI = 3.14159;
来源：http://nh.shtwfgs.cn

[S28] C：静态变量
来源：http://fz.yuntaijiaju.cn

static int counter = 0;
来源：http://br.nicolike.cn

[S29] C：变参函数
来源：http://yb.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zf.jctech888.com.cn

[S30] C：头文件保护
来源：http://ta.jianghongdianzi.cn


<!-- 参考信息 -->