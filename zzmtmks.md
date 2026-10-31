代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eo.jctech888.com.cn

[Q60] 取上一行 / 下一行
来源：http://nf.szxytkj.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tz.shxzukj.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rs.nicolike.cn

[Q61] 移动平均
来源：http://vi.nicolike.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ox.yuexingan06.cn

[Q62] 分组占比
来源：http://gx.yuntaijiaju.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dh.bjjhwx.cn

[Q63] 开启事务
来源：http://ic.521024.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ud.yuexingan06.cn

[Q64] 提交事务
来源：http://ve.huanxung.cn

COMMIT;
来源：http://qa.szsharing.cn

[Q65] 回滚事务
来源：http://gb.hnjuh.cn

ROLLBACK;
来源：http://ba.wgjwhj.cn

[Q66] 行锁查询
来源：http://rt.chemitech.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jb.chemitech.net.cn

[Q67] 设置隔离级别
来源：http://ne.nicolike.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pt.jctech888.com.cn

[Q68] 保存点
来源：http://cm.bjjhwx.cn

SAVEPOINT sp1;
来源：http://ca.chemitech.net.cn

ROLLBACK TO sp1;
来源：http://pa.haigaiapp.cn

[Q69] 查看执行计划
来源：http://bz.gzmigu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ik.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ml.jctech888.com.cn

ANALYZE TABLE users;
来源：http://wh.haigaiapp.cn

[Q71] 查看建表语句
来源：http://ut.panjiajie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qd.shxzukj.cn

[Q72] 查看索引
来源：http://tw.gzmigu.cn

SHOW INDEX FROM users;
来源：http://ka.huixiangedu.cn

[Q73] 查看表状态
来源：http://of.asd995.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ou.haigaiapp.cn

[Q74] 强制使用索引
来源：http://oz.shtwfgs.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pq.bjjhwx.cn

[Q75] 日期格式化
来源：http://bf.lnxyls.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ng.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mz.bookmarksfly.cn

[Q76] 按天统计
来源：http://fc.haigaiapp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wz.jctech888.com.cn

[Q77] 时间加减
来源：http://ir.yuntaijiaju.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pl.jctech888.com.cn

[Q78] 当前时间
来源：http://xc.chemitech.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xy.muxihuayi.cn

[Q79] 字符串拼接
来源：http://or.lnxyls.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nn.haigaiapp.cn

[Q80] 字符串截取
来源：http://jm.muxihuayi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hm.haigaiapp.cn

[Q81] 字符串替换
来源：http://wt.shxzskj.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qq.panjiajie.cn

[Q82] 字符长度与字节长度
来源：http://oc.shtwfgs.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://po.bookmarksfly.cn

[Q83] 大小写转换
来源：http://na.shtwfgs.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://up.shxzskj.cn

[Q84] 去除首尾空格
来源：http://sw.shxzskj.cn

SELECT TRIM(name) FROM users;
来源：http://jv.newstarts.cn

[Q85] 数值取整
来源：http://lw.chemitech.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ah.hahajie.cn

[Q86] 读取 JSON 字段
来源：http://zv.yuntaijiaju.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://et.newstarts.cn

[Q87] JSON 字段做条件
来源：http://ka.shxzukj.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ag.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://vq.szxytkj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ug.yuexingan06.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lj.hahajie.cn

[Q89] 判断表是否存在
来源：http://ua.nszjky.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rv.panjiajie.cn

[Q90] 生成序号列
来源：http://fo.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ya.yuexingan06.cn

================================================================================
来源：http://dg.yuntaijiaju.cn

R. Bash 专题
来源：http://tt.jctech888.com.cn

================================================================================
来源：http://zl.hnjuh.cn

[R01] shebang 与严格模式
来源：http://kl.jianghongdianzi.cn

#!/usr/bin/env bash
来源：http://od.muxihuayi.cn

set -euo pipefail
来源：http://ze.shxzukj.cn

[R02] 变量赋值与使用
来源：http://kb.colortex.cn

name="Tom"; echo "$name"
来源：http://kk.colortex.cn

[R03] 只读变量
来源：http://wb.shxzskj.cn

readonly PI=3.14
来源：http://nu.panjiajie.cn

[R04] 位置参数
来源：http://xx.szxytkj.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://as.chemitech.net.cn

[R05] 参数默认值
来源：http://jo.bookmarksfly.cn

name="${1:-default}"
来源：http://nk.szsharing.cn

[R06] 判断命令是否存在
来源：http://cw.huanxung.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qr.chemitech.net.cn

[R07] if 判断文件
来源：http://cx.huixiangedu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qp.colortex.cn

[R08] 数值比较
来源：http://my.bjjhwx.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vp.9csxet.cn

[R09] 字符串比较
来源：http://xh.panjiajie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tm.yuexingan06.cn

[R10] 正则匹配
来源：http://bu.huixiangedu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pk.shxzskj.cn

[R11] case 多分支
来源：http://mu.gzmigu.cn

case "$1" in
来源：http://iv.521024.cn

start) echo "启动" ;;
来源：http://qo.nszjky.cn

stop)  echo "停止" ;;
来源：http://wz.shxzukj.cn

*)     echo "未知命令" ;;
来源：http://mc.jianghongdianzi.cn

esac
来源：http://ng.9csxet.cn

[R12] for 遍历文件
来源：http://dg.szsharing.cn

for f in *.txt; do echo "$f"; done
来源：http://ic.shxzskj.cn

[R13] for 计数循环
来源：http://cb.nszjky.cn

for i in {1..10}; do echo "$i"; done
来源：http://tc.haigaiapp.cn

[R14] C 风格 for
来源：http://jc.muxihuayi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://te.shxzskj.cn

[R15] while 逐行读文件
来源：http://hi.521024.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ec.bjjhwx.cn

[R16] until 等待条件
来源：http://no.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hu.yuexingan06.cn

[R17] 数组定义与取值
来源：http://sj.huixiangedu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eq.szsharing.cn

[R18] 遍历数组
来源：http://ve.9csxet.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ta.gzmigu.cn

[R19] 数组长度
来源：http://ky.lnxyls.cn

echo "${#arr[@]}"
来源：http://gv.yuntaijiaju.cn

[R20] 关联数组（字典）
来源：http://jh.szxytkj.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hy.wgjwhj.cn

[R21] 字符串长度
来源：http://kt.chemitech.net.cn

echo "${#s}"
来源：http://xa.haigaiapp.cn

[R22] 截取子串
来源：http://ey.shxzukj.cn

echo "${s:0:5}"
来源：http://mp.szsharing.cn

[R23] 字符串替换
来源：http://rv.asd995.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lk.bookmarksfly.cn

[R24] 大小写转换
来源：http://ry.yuntaijiaju.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xm.newstarts.cn

[R25] 去后缀 / 去前缀
来源：http://bc.lnxyls.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vq.asd995.cn

[R26] 命令替换
来源：http://fo.bookmarksfly.cn

now=$(date +%F); echo "$now"
来源：http://qe.hnjuh.cn

[R27] 算术展开
来源：http://hg.wgjwhj.cn

echo $((1 + 2 * 3))
来源：http://dw.shxzukj.cn

[R28] 浮点运算
来源：http://lt.521024.cn

echo "scale=2; 10/3" | bc
来源：http://nj.nszjky.cn

[R29] 定义函数
来源：http://wp.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://me.chemitech.net.cn

[R30] 函数返回状态码
来源：http://rf.shxzukj.cn

f() { return 0; }; f || echo "失败了"
来源：http://kq.huanxung.cn

[R31] 局部变量
来源：http://ii.jianghongdianzi.cn

f() { local x=1; echo "$x"; }
来源：http://ld.muxihuayi.cn

[R32] 参数个数校验
来源：http://fl.bookmarksfly.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pz.shxzskj.cn

[R33] 捕获错误并提示行号
来源：http://yd.jianghongdianzi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cl.newstarts.cn

[R34] 退出时清理
来源：http://qj.lnxyls.cn

trap 'rm -f "$tmp"' EXIT
来源：http://es.nszjky.cn

[R35] 后台执行并等待
来源：http://zz.huixinmuqiang.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ts.szsharing.cn

[R36] 并发执行多个任务
来源：http://pn.muxihuayi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mp.panjiajie.cn

[R37] 把输出赋给变量
来源：http://oj.nszjky.cn

files=$(ls -1)
来源：http://hz.nicolike.cn

[R38] 管道串联
来源：http://dr.jctech888.com.cn

cat a.txt | grep -i error | wc -l
来源：http://ij.wgjwhj.cn

[R39] 重定向标准输出与错误
来源：http://yp.bjjhwx.cn

cmd > out.log 2>&1
来源：http://sf.huixinmuqiang.cn

[R40] 追加写日志
来源：http://jy.bjjhwx.cn

echo "log" >> out.log
来源：http://ol.szsharing.cn

[R41] 丢弃输出
来源：http://qt.asd995.cn

cmd >/dev/null 2>&1
来源：http://sf.bjjhwx.cn

[R42] 输入重定向
来源：http://yy.gzmigu.cn

wc -l < a.txt
来源：http://fq.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://ab.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://ny.huixinmuqiang.cn

[R44] 按修改时间查找
来源：http://ql.muxihuayi.cn

find . -mtime -7 -type f
来源：http://mh.jianghongdianzi.cn

[R45] 批量删除
来源：http://xw.hnjuh.cn

find . -name "*.tmp" -delete
来源：http://sw.nszjky.cn

[R46] 递归替换文件内容
来源：http://pl.hahajie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jf.huixinmuqiang.cn

[R47] sed 单行替换
来源：http://yo.shtwfgs.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xe.521024.cn

[R48] awk 取指定列
来源：http://wt.shtwfgs.cn

awk '{print $1, $3}' a.txt
来源：http://bs.shxzskj.cn

[R49] awk 带条件
来源：http://gs.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xz.jctech888.com.cn

[R50] awk 求和
来源：http://bv.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xw.bookmarksfly.cn

[R51] 排序去重取前几
来源：http://ka.colortex.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fn.jctech888.com.cn

[R52] 统计行数
来源：http://sg.huixinmuqiang.cn

wc -l a.txt
来源：http://qk.huanxung.cn

[R53] 查看文件头与实时尾
来源：http://iw.gzmigu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ld.lnxyls.cn

[R54] 比较两个文件
来源：http://bl.jianghongdianzi.cn

diff a.txt b.txt
来源：http://su.wgjwhj.cn

[R55] 压缩与解压
来源：http://rk.newstarts.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://se.521024.cn

[R56] 远程拷贝
来源：http://oj.jianghongdianzi.cn

scp file user@host:/path/
来源：http://jf.colortex.cn

[R57] 远程执行命令
来源：http://dt.szxytkj.cn

ssh user@host 'uptime'
来源：http://tj.muxihuayi.cn

[R58] 下载文件
来源：http://ks.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://si.521024.cn

[R59] 发 POST JSON
来源：http://mz.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oi.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://xa.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kl.bjjhwx.cn

[R61] 磁盘占用
来源：http://wy.huanxung.cn

df -h;  du -sh *
来源：http://vm.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://na.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://rk.nicolike.cn

[R63] 内存与进程
来源：http://ta.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://bh.bookmarksfly.cn

[R64] 结束进程
来源：http://ta.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://lp.szxytkj.cn

[R65] 查看端口占用
来源：http://ee.yuntaijiaju.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yp.9csxet.cn

[R66] 定时任务
来源：http://gx.9csxet.cn

crontab -e;  crontab -l
来源：http://af.shxzukj.cn

[R67] 生成随机十六进制串
来源：http://us.shxzskj.cn

openssl rand -hex 16
来源：http://al.nszjky.cn

[R68] 计算文件校验值
来源：http://ny.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ol.huanxung.cn

[R69] 生成随机密码
来源：http://ki.hahajie.cn

head -c 16 /dev/urandom | base64
来源：http://ti.colortex.cn

[R70] 时间戳与互转
来源：http://lg.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://ur.szsharing.cn

[R71] 日期格式化
来源：http://ux.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kk.panjiajie.cn

[R72] 等待端口就绪
来源：http://eq.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yu.9csxet.cn

[R73] 分割大日志
来源：http://gr.lnxyls.cn

split -l 1000 big.log part_
来源：http://tk.nicolike.cn

[R74] 批量重命名
来源：http://ds.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vi.huixiangedu.cn

[R75] 导出环境变量
来源：http://hb.hnjuh.cn

export PATH="$HOME/bin:$PATH"
来源：http://se.shxzskj.cn

[R76] 使用临时文件
来源：http://cj.yuntaijiaju.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yj.shtwfgs.cn

[R77] 读取用户输入
来源：http://hs.shxzskj.cn

read -rp "请输入: " ans
来源：http://gu.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://yx.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dx.huixiangedu.cn

[R79] 解析命令行选项
来源：http://gn.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://td.9csxet.cn

[R80] 查看脚本执行耗时
来源：http://ea.szsharing.cn

time ./run.sh
来源：http://dg.521024.cn

================================================================================
来源：http://pq.hnjuh.cn

S. C / C++ 专题
来源：http://bv.huixinmuqiang.cn

================================================================================
来源：http://ti.bjjhwx.cn

[S01] C：Hello World
来源：http://dd.yuexingan06.cn

#include <stdio.h>
来源：http://ag.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ni.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://mq.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://ik.wgjwhj.cn

[S03] C：读入整数
来源：http://nd.colortex.cn

int x; scanf("%d", &x);
来源：http://vu.shxzukj.cn

[S04] C：字符串复制
来源：http://eq.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dz.nicolike.cn

[S05] C：字符串长度
来源：http://er.chemitech.net.cn

strlen(s)
来源：http://bs.hnjuh.cn

[S06] C：字符串比较
来源：http://no.wgjwhj.cn

strcmp(a, b) == 0
来源：http://jv.asd995.cn

[S07] C：数组遍历求和
来源：http://tk.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vp.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://cb.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kc.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://zl.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ul.chemitech.net.cn

[S10] C：指针与解引用
来源：http://py.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ay.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ad.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://up.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xx.huixiangedu.cn

fclose(f);
来源：http://la.huixinmuqiang.cn

[S12] C：写文件
来源：http://tx.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tk.jianghongdianzi.cn

[S13] C：宏定义
来源：http://og.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ss.colortex.cn

[S14] C：枚举
来源：http://qt.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://hk.szxytkj.cn

[S15] C：类型转换
来源：http://ul.chemitech.net.cn

(double) a / b
来源：http://bw.nicolike.cn

[S16] C：位操作置位
来源：http://dm.nicolike.cn

x |= (1 << 3);
来源：http://jd.nszjky.cn

[S17] C：安全拼接字符串
来源：http://pl.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ry.szsharing.cn

[S18] C：命令行参数
来源：http://zh.nicolike.cn

int main(int argc, char **argv)
来源：http://qv.shtwfgs.cn

[S19] C：快速排序
来源：http://jy.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ft.jctech888.com.cn

[S20] C：二分查找
来源：http://fg.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cq.yuexingan06.cn

[S21] C：字符类别判断
来源：http://rk.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ws.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://mx.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://co.szxytkj.cn

[S23] C：随机数
来源：http://mn.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qy.szsharing.cn

[S24] C：获取本地时间
来源：http://sr.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://se.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://qx.huanxung.cn

memcpy(dst, src, n);
来源：http://vp.bjjhwx.cn

[S26] C：内存清零
来源：http://mm.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://oy.jctech888.com.cn

[S27] C：定义常量
来源：http://iq.chemitech.net.cn

const double PI = 3.14159;
来源：http://zy.panjiajie.cn

[S28] C：静态变量
来源：http://kt.shxzukj.cn

static int counter = 0;
来源：http://cs.521024.cn

[S29] C：变参函数
来源：http://vh.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wp.hahajie.cn

[S30] C：头文件保护
来源：http://sg.szsharing.cn


<!-- 参考信息 -->