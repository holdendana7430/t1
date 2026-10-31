代发 wailian999

[Q48] CTE 公用表表达式
来源：http://ut.jianghongdianzi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://db.gzmigu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ie.muxihuayi.cn

[Q49] 更新单行
来源：http://lm.jctech888.com.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jl.9csxet.cn

[Q50] 批量更新
来源：http://aj.hahajie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gs.newstarts.cn

[Q51] 用子查询更新
来源：http://oz.newstarts.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dy.huixiangedu.cn

[Q52] 删除指定行
来源：http://he.9csxet.cn

DELETE FROM users WHERE id = 10;
来源：http://ar.jianghongdianzi.cn

[Q53] 按条件删除
来源：http://jl.colortex.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sr.yuexingan06.cn

[Q54] 清空表
来源：http://yf.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://gx.szxytkj.cn

[Q55] 排名（并列占位）
来源：http://zx.jianghongdianzi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ou.shxzskj.cn

[Q56] 密集排名（并列不占位）
来源：http://vz.shxzskj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://la.hnjuh.cn

[Q57] 行号
来源：http://zu.hnjuh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ai.shxzukj.cn

[Q58] 累计求和
来源：http://eq.yuexingan06.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qa.nszjky.cn

[Q59] 分组内累计
来源：http://yg.szsharing.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tl.bookmarksfly.cn

[Q60] 取上一行 / 下一行
来源：http://qy.asd995.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ii.gzmigu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ys.521024.cn

[Q61] 移动平均
来源：http://jz.huanxung.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://la.huixinmuqiang.cn

[Q62] 分组占比
来源：http://vq.hnjuh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://se.shtwfgs.cn

[Q63] 开启事务
来源：http://zf.chemitech.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qn.hahajie.cn

[Q64] 提交事务
来源：http://oc.jctech888.com.cn

COMMIT;
来源：http://wb.asd995.cn

[Q65] 回滚事务
来源：http://cu.jianghongdianzi.cn

ROLLBACK;
来源：http://nl.shxzukj.cn

[Q66] 行锁查询
来源：http://wp.jctech888.com.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pe.gzmigu.cn

[Q67] 设置隔离级别
来源：http://pk.muxihuayi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://db.szsharing.cn

[Q68] 保存点
来源：http://dk.colortex.cn

SAVEPOINT sp1;
来源：http://id.wgjwhj.cn

ROLLBACK TO sp1;
来源：http://yt.hnjuh.cn

[Q69] 查看执行计划
来源：http://hi.wgjwhj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kd.yuntaijiaju.cn

[Q70] 更新统计信息
来源：http://ut.szsharing.cn

ANALYZE TABLE users;
来源：http://xl.szxytkj.cn

[Q71] 查看建表语句
来源：http://xy.bookmarksfly.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xn.nszjky.cn

[Q72] 查看索引
来源：http://vw.9csxet.cn

SHOW INDEX FROM users;
来源：http://wc.huixiangedu.cn

[Q73] 查看表状态
来源：http://kt.newstarts.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://pv.bookmarksfly.cn

[Q74] 强制使用索引
来源：http://bi.asd995.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gt.9csxet.cn

[Q75] 日期格式化
来源：http://pc.gzmigu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ro.hahajie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xw.asd995.cn

[Q76] 按天统计
来源：http://vr.huixiangedu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qr.bookmarksfly.cn

[Q77] 时间加减
来源：http://al.muxihuayi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dr.colortex.cn

[Q78] 当前时间
来源：http://ym.panjiajie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fo.521024.cn

[Q79] 字符串拼接
来源：http://ja.521024.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pk.9csxet.cn

[Q80] 字符串截取
来源：http://vm.nicolike.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fk.hnjuh.cn

[Q81] 字符串替换
来源：http://mq.muxihuayi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ta.nszjky.cn

[Q82] 字符长度与字节长度
来源：http://nq.9csxet.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qo.521024.cn

[Q83] 大小写转换
来源：http://hk.huanxung.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wk.szxytkj.cn

[Q84] 去除首尾空格
来源：http://bo.gzmigu.cn

SELECT TRIM(name) FROM users;
来源：http://gk.muxihuayi.cn

[Q85] 数值取整
来源：http://be.szsharing.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ke.yuntaijiaju.cn

[Q86] 读取 JSON 字段
来源：http://fq.shxzukj.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cz.gzmigu.cn

[Q87] JSON 字段做条件
来源：http://xg.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ry.nszjky.cn

[Q88] 行转列（条件聚合）
来源：http://ck.shxzukj.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rp.bookmarksfly.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zd.chemitech.net.cn

[Q89] 判断表是否存在
来源：http://hv.hnjuh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ju.shtwfgs.cn

[Q90] 生成序号列
来源：http://rq.bookmarksfly.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yx.szxytkj.cn

================================================================================
来源：http://tf.hnjuh.cn

R. Bash 专题
来源：http://gy.jctech888.com.cn

================================================================================
来源：http://ej.bjjhwx.cn

[R01] shebang 与严格模式
来源：http://wi.panjiajie.cn

#!/usr/bin/env bash
来源：http://wd.yuntaijiaju.cn

set -euo pipefail
来源：http://di.jctech888.com.cn

[R02] 变量赋值与使用
来源：http://ig.nicolike.cn

name="Tom"; echo "$name"
来源：http://fn.jianghongdianzi.cn

[R03] 只读变量
来源：http://ya.jctech888.com.cn

readonly PI=3.14
来源：http://ms.wgjwhj.cn

[R04] 位置参数
来源：http://aw.jctech888.com.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qp.panjiajie.cn

[R05] 参数默认值
来源：http://du.shtwfgs.cn

name="${1:-default}"
来源：http://pn.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://ap.hahajie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eo.panjiajie.cn

[R07] if 判断文件
来源：http://bm.bjjhwx.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wt.lnxyls.cn

[R08] 数值比较
来源：http://ib.huixiangedu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ol.nicolike.cn

[R09] 字符串比较
来源：http://dd.shxzskj.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ky.9csxet.cn

[R10] 正则匹配
来源：http://iz.nszjky.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tz.huixinmuqiang.cn

[R11] case 多分支
来源：http://fo.colortex.cn

case "$1" in
来源：http://gc.yuntaijiaju.cn

start) echo "启动" ;;
来源：http://my.lnxyls.cn

stop)  echo "停止" ;;
来源：http://tj.shtwfgs.cn

*)     echo "未知命令" ;;
来源：http://ci.panjiajie.cn

esac
来源：http://aq.asd995.cn

[R12] for 遍历文件
来源：http://sz.shxzukj.cn

for f in *.txt; do echo "$f"; done
来源：http://iu.asd995.cn

[R13] for 计数循环
来源：http://xu.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://ac.bookmarksfly.cn

[R14] C 风格 for
来源：http://bc.jctech888.com.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ce.shxzskj.cn

[R15] while 逐行读文件
来源：http://th.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://we.chemitech.net.cn

[R16] until 等待条件
来源：http://ui.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mo.nszjky.cn

[R17] 数组定义与取值
来源：http://da.521024.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kg.shxzukj.cn

[R18] 遍历数组
来源：http://hx.huixinmuqiang.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eh.szsharing.cn

[R19] 数组长度
来源：http://fp.huixiangedu.cn

echo "${#arr[@]}"
来源：http://qb.panjiajie.cn

[R20] 关联数组（字典）
来源：http://kf.521024.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://au.bookmarksfly.cn

[R21] 字符串长度
来源：http://gt.asd995.cn

echo "${#s}"
来源：http://yr.521024.cn

[R22] 截取子串
来源：http://kd.szsharing.cn

echo "${s:0:5}"
来源：http://uv.colortex.cn

[R23] 字符串替换
来源：http://cb.yuexingan06.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oe.huixiangedu.cn

[R24] 大小写转换
来源：http://ty.wgjwhj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zn.nicolike.cn

[R25] 去后缀 / 去前缀
来源：http://xe.wgjwhj.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://aa.nszjky.cn

[R26] 命令替换
来源：http://ke.nszjky.cn

now=$(date +%F); echo "$now"
来源：http://dj.hnjuh.cn

[R27] 算术展开
来源：http://so.panjiajie.cn

echo $((1 + 2 * 3))
来源：http://dl.hnjuh.cn

[R28] 浮点运算
来源：http://wb.asd995.cn

echo "scale=2; 10/3" | bc
来源：http://zr.chemitech.net.cn

[R29] 定义函数
来源：http://sv.gzmigu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vu.yuntaijiaju.cn

[R30] 函数返回状态码
来源：http://it.yuntaijiaju.cn

f() { return 0; }; f || echo "失败了"
来源：http://sl.9csxet.cn

[R31] 局部变量
来源：http://di.huixiangedu.cn

f() { local x=1; echo "$x"; }
来源：http://fc.chemitech.net.cn

[R32] 参数个数校验
来源：http://xx.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rd.nszjky.cn

[R33] 捕获错误并提示行号
来源：http://il.huixinmuqiang.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jm.shxzskj.cn

[R34] 退出时清理
来源：http://vw.bjjhwx.cn

trap 'rm -f "$tmp"' EXIT
来源：http://to.521024.cn

[R35] 后台执行并等待
来源：http://ho.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cy.nszjky.cn

[R36] 并发执行多个任务
来源：http://zd.nicolike.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cu.wgjwhj.cn

[R37] 把输出赋给变量
来源：http://bz.yuntaijiaju.cn

files=$(ls -1)
来源：http://rs.shxzukj.cn

[R38] 管道串联
来源：http://ka.521024.cn

cat a.txt | grep -i error | wc -l
来源：http://bk.asd995.cn

[R39] 重定向标准输出与错误
来源：http://ad.colortex.cn

cmd > out.log 2>&1
来源：http://uy.hahajie.cn

[R40] 追加写日志
来源：http://wb.yuntaijiaju.cn

echo "log" >> out.log
来源：http://qh.huixinmuqiang.cn

[R41] 丢弃输出
来源：http://iz.colortex.cn

cmd >/dev/null 2>&1
来源：http://rt.yuntaijiaju.cn

[R42] 输入重定向
来源：http://uy.asd995.cn

wc -l < a.txt
来源：http://ga.jctech888.com.cn

[R43] 按名字查找文件
来源：http://ss.wgjwhj.cn

find . -name "*.log" -type f
来源：http://wo.muxihuayi.cn

[R44] 按修改时间查找
来源：http://cf.muxihuayi.cn

find . -mtime -7 -type f
来源：http://xh.shxzukj.cn

[R45] 批量删除
来源：http://qw.huixiangedu.cn

find . -name "*.tmp" -delete
来源：http://ph.bookmarksfly.cn

[R46] 递归替换文件内容
来源：http://ut.yuexingan06.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://la.huixiangedu.cn

[R47] sed 单行替换
来源：http://sv.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xx.yuexingan06.cn

[R48] awk 取指定列
来源：http://qt.colortex.cn

awk '{print $1, $3}' a.txt
来源：http://lj.lnxyls.cn

[R49] awk 带条件
来源：http://ye.yuexingan06.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eq.yuexingan06.cn

[R50] awk 求和
来源：http://qx.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://et.szxytkj.cn

[R51] 排序去重取前几
来源：http://hg.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wt.nicolike.cn

[R52] 统计行数
来源：http://qx.lnxyls.cn

wc -l a.txt
来源：http://yn.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://uz.521024.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vc.huixiangedu.cn

[R54] 比较两个文件
来源：http://wp.nszjky.cn

diff a.txt b.txt
来源：http://or.hahajie.cn

[R55] 压缩与解压
来源：http://jw.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cs.jianghongdianzi.cn

[R56] 远程拷贝
来源：http://zs.shxzukj.cn

scp file user@host:/path/
来源：http://by.chemitech.net.cn

[R57] 远程执行命令
来源：http://rm.haigaiapp.cn

ssh user@host 'uptime'
来源：http://gn.shxzukj.cn

[R58] 下载文件
来源：http://js.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hw.hnjuh.cn

[R59] 发 POST JSON
来源：http://nv.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://te.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://ze.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dw.asd995.cn

[R61] 磁盘占用
来源：http://iv.colortex.cn

df -h;  du -sh *
来源：http://ep.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://sq.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://cs.yuntaijiaju.cn

[R63] 内存与进程
来源：http://hn.huixiangedu.cn

free -h;  ps aux | grep nginx
来源：http://vt.shxzskj.cn

[R64] 结束进程
来源：http://qr.szsharing.cn

kill -9 $(pgrep -f app.py)
来源：http://rh.asd995.cn

[R65] 查看端口占用
来源：http://lh.muxihuayi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mw.szxytkj.cn

[R66] 定时任务
来源：http://ay.bjjhwx.cn

crontab -e;  crontab -l
来源：http://pf.huanxung.cn

[R67] 生成随机十六进制串
来源：http://jl.bjjhwx.cn

openssl rand -hex 16
来源：http://kn.9csxet.cn

[R68] 计算文件校验值
来源：http://hb.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fj.shtwfgs.cn

[R69] 生成随机密码
来源：http://kj.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://bn.yuexingan06.cn

[R70] 时间戳与互转
来源：http://xd.newstarts.cn

date +%s;  date -d @1700000000
来源：http://ui.lnxyls.cn

[R71] 日期格式化
来源：http://yi.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fu.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://kv.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yt.hnjuh.cn

[R73] 分割大日志
来源：http://zd.shxzukj.cn

split -l 1000 big.log part_
来源：http://hd.bjjhwx.cn

[R74] 批量重命名
来源：http://eo.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cz.shxzskj.cn

[R75] 导出环境变量
来源：http://as.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://kj.gzmigu.cn

[R76] 使用临时文件
来源：http://lk.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sv.muxihuayi.cn

[R77] 读取用户输入
来源：http://vb.nicolike.cn

read -rp "请输入: " ans
来源：http://fk.521024.cn

[R78] 交互式菜单
来源：http://qq.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uv.bjjhwx.cn

[R79] 解析命令行选项
来源：http://tn.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jb.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://st.yuntaijiaju.cn

time ./run.sh
来源：http://zi.521024.cn

================================================================================
来源：http://us.nszjky.cn

S. C / C++ 专题
来源：http://kx.lnxyls.cn

================================================================================
来源：http://nr.9csxet.cn

[S01] C：Hello World
来源：http://sd.nszjky.cn

#include <stdio.h>
来源：http://zx.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ng.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://pj.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://lp.huixinmuqiang.cn

[S03] C：读入整数
来源：http://ap.9csxet.cn

int x; scanf("%d", &x);
来源：http://yi.hnjuh.cn

[S04] C：字符串复制
来源：http://gz.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wk.jctech888.com.cn

[S05] C：字符串长度
来源：http://pk.wgjwhj.cn

strlen(s)
来源：http://fh.szsharing.cn

[S06] C：字符串比较
来源：http://bh.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://na.nszjky.cn

[S07] C：数组遍历求和
来源：http://ei.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nv.muxihuayi.cn

[S08] C：动态内存分配与释放
来源：http://ba.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qe.shxzskj.cn

[S09] C：结构体定义与初始化
来源：http://gl.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fg.jctech888.com.cn

[S10] C：指针与解引用
来源：http://tt.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://rl.9csxet.cn

[S11] C：逐行读文件
来源：http://ds.muxihuayi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ui.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lq.nszjky.cn

fclose(f);
来源：http://jk.colortex.cn

[S12] C：写文件
来源：http://sx.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nv.lnxyls.cn

[S13] C：宏定义
来源：http://hx.lnxyls.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yf.wgjwhj.cn

[S14] C：枚举
来源：http://jb.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://jt.shxzskj.cn

[S15] C：类型转换
来源：http://pv.shxzskj.cn

(double) a / b
来源：http://rf.hnjuh.cn

[S16] C：位操作置位
来源：http://ia.szsharing.cn

x |= (1 << 3);
来源：http://ab.chemitech.net.cn

[S17] C：安全拼接字符串
来源：http://nk.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://we.huixiangedu.cn

[S18] C：命令行参数
来源：http://uq.nicolike.cn


<!-- 参考信息 -->