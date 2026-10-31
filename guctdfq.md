代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://ho.haigaiapp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vy.yuexingan06.cn

[Q43] 标量子查询
来源：http://ox.wgjwhj.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lf.colortex.cn

[Q44] IN 子查询
来源：http://tn.huixinmuqiang.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sw.bookmarksfly.cn

[Q45] EXISTS 判断存在
来源：http://zf.huanxung.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sr.jianghongdianzi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nh.gzmigu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hf.shxzukj.cn

[Q47] 与平均值比较
来源：http://cj.szsharing.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ru.haigaiapp.cn

[Q48] CTE 公用表表达式
来源：http://vy.shxzukj.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wl.nicolike.cn

SELECT * FROM t WHERE c > 5;
来源：http://dj.lnxyls.cn

[Q49] 更新单行
来源：http://yr.asd995.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yr.chemitech.net.cn

[Q50] 批量更新
来源：http://qc.nszjky.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oo.shtwfgs.cn

[Q51] 用子查询更新
来源：http://pq.wgjwhj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bl.hahajie.cn

[Q52] 删除指定行
来源：http://ea.shxzskj.cn

DELETE FROM users WHERE id = 10;
来源：http://fp.asd995.cn

[Q53] 按条件删除
来源：http://at.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ch.jianghongdianzi.cn

[Q54] 清空表
来源：http://yx.yuntaijiaju.cn

TRUNCATE TABLE logs;
来源：http://cp.chemitech.net.cn

[Q55] 排名（并列占位）
来源：http://nm.9csxet.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ck.wgjwhj.cn

[Q56] 密集排名（并列不占位）
来源：http://mo.wgjwhj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iq.muxihuayi.cn

[Q57] 行号
来源：http://qk.asd995.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://om.jianghongdianzi.cn

[Q58] 累计求和
来源：http://mj.huanxung.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wf.nszjky.cn

[Q59] 分组内累计
来源：http://mt.chemitech.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xx.huixiangedu.cn

[Q60] 取上一行 / 下一行
来源：http://zi.jctech888.com.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iu.yuntaijiaju.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uh.hnjuh.cn

[Q61] 移动平均
来源：http://vb.hnjuh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fd.szxytkj.cn

[Q62] 分组占比
来源：http://zl.wgjwhj.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wt.bjjhwx.cn

[Q63] 开启事务
来源：http://lj.lnxyls.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lg.shtwfgs.cn

[Q64] 提交事务
来源：http://gp.9csxet.cn

COMMIT;
来源：http://hk.bjjhwx.cn

[Q65] 回滚事务
来源：http://at.shtwfgs.cn

ROLLBACK;
来源：http://wu.muxihuayi.cn

[Q66] 行锁查询
来源：http://jv.9csxet.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kt.huixinmuqiang.cn

[Q67] 设置隔离级别
来源：http://oh.chemitech.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xo.asd995.cn

[Q68] 保存点
来源：http://gu.jianghongdianzi.cn

SAVEPOINT sp1;
来源：http://lr.9csxet.cn

ROLLBACK TO sp1;
来源：http://vz.shxzukj.cn

[Q69] 查看执行计划
来源：http://xm.shxzukj.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ww.shxzskj.cn

[Q70] 更新统计信息
来源：http://sy.haigaiapp.cn

ANALYZE TABLE users;
来源：http://nx.huixiangedu.cn

[Q71] 查看建表语句
来源：http://nr.yuntaijiaju.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://an.colortex.cn

[Q72] 查看索引
来源：http://sr.yuexingan06.cn

SHOW INDEX FROM users;
来源：http://yc.huixinmuqiang.cn

[Q73] 查看表状态
来源：http://ov.huanxung.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://so.hnjuh.cn

[Q74] 强制使用索引
来源：http://cp.nszjky.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ht.szxytkj.cn

[Q75] 日期格式化
来源：http://rb.colortex.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zi.colortex.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wf.shxzskj.cn

[Q76] 按天统计
来源：http://au.yuntaijiaju.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://sj.hnjuh.cn

[Q77] 时间加减
来源：http://pr.jianghongdianzi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jj.haigaiapp.cn

[Q78] 当前时间
来源：http://li.newstarts.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vh.yuexingan06.cn

[Q79] 字符串拼接
来源：http://yb.huixiangedu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hv.huixinmuqiang.cn

[Q80] 字符串截取
来源：http://bs.hnjuh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bc.panjiajie.cn

[Q81] 字符串替换
来源：http://gy.haigaiapp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yk.hnjuh.cn

[Q82] 字符长度与字节长度
来源：http://fc.colortex.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cp.bookmarksfly.cn

[Q83] 大小写转换
来源：http://nn.panjiajie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ow.huixinmuqiang.cn

[Q84] 去除首尾空格
来源：http://hw.huixinmuqiang.cn

SELECT TRIM(name) FROM users;
来源：http://dq.chemitech.net.cn

[Q85] 数值取整
来源：http://yc.521024.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hv.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://pk.521024.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://un.szxytkj.cn

[Q87] JSON 字段做条件
来源：http://hs.bjjhwx.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pj.chemitech.net.cn

[Q88] 行转列（条件聚合）
来源：http://wh.yuntaijiaju.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yj.lnxyls.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eo.bookmarksfly.cn

[Q89] 判断表是否存在
来源：http://ct.szxytkj.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kj.wgjwhj.cn

[Q90] 生成序号列
来源：http://sq.newstarts.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cb.nicolike.cn

================================================================================
来源：http://bv.lnxyls.cn

R. Bash 专题
来源：http://vg.521024.cn

================================================================================
来源：http://sq.szxytkj.cn

[R01] shebang 与严格模式
来源：http://ie.bjjhwx.cn

#!/usr/bin/env bash
来源：http://mo.jctech888.com.cn

set -euo pipefail
来源：http://mc.hnjuh.cn

[R02] 变量赋值与使用
来源：http://kh.huixinmuqiang.cn

name="Tom"; echo "$name"
来源：http://rw.9csxet.cn

[R03] 只读变量
来源：http://ck.bjjhwx.cn

readonly PI=3.14
来源：http://ce.yuntaijiaju.cn

[R04] 位置参数
来源：http://id.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bc.jianghongdianzi.cn

[R05] 参数默认值
来源：http://ka.shxzskj.cn

name="${1:-default}"
来源：http://wd.huixinmuqiang.cn

[R06] 判断命令是否存在
来源：http://ty.colortex.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ng.jctech888.com.cn

[R07] if 判断文件
来源：http://cy.szxytkj.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xr.haigaiapp.cn

[R08] 数值比较
来源：http://sq.szsharing.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uz.haigaiapp.cn

[R09] 字符串比较
来源：http://it.huixiangedu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wt.lnxyls.cn

[R10] 正则匹配
来源：http://so.yuntaijiaju.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://og.newstarts.cn

[R11] case 多分支
来源：http://ko.bookmarksfly.cn

case "$1" in
来源：http://em.huanxung.cn

start) echo "启动" ;;
来源：http://lq.huixiangedu.cn

stop)  echo "停止" ;;
来源：http://wb.szsharing.cn

*)     echo "未知命令" ;;
来源：http://ul.muxihuayi.cn

esac
来源：http://gs.szsharing.cn

[R12] for 遍历文件
来源：http://jd.yuexingan06.cn

for f in *.txt; do echo "$f"; done
来源：http://da.jctech888.com.cn

[R13] for 计数循环
来源：http://pw.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://af.asd995.cn

[R14] C 风格 for
来源：http://tq.shxzukj.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sg.muxihuayi.cn

[R15] while 逐行读文件
来源：http://wd.lnxyls.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yt.hnjuh.cn

[R16] until 等待条件
来源：http://ew.shtwfgs.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rj.gzmigu.cn

[R17] 数组定义与取值
来源：http://hg.nszjky.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uw.yuntaijiaju.cn

[R18] 遍历数组
来源：http://zx.nszjky.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dq.huixiangedu.cn

[R19] 数组长度
来源：http://zp.shxzukj.cn

echo "${#arr[@]}"
来源：http://to.huixinmuqiang.cn

[R20] 关联数组（字典）
来源：http://yj.huanxung.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xv.bookmarksfly.cn

[R21] 字符串长度
来源：http://mc.chemitech.net.cn

echo "${#s}"
来源：http://mf.shtwfgs.cn

[R22] 截取子串
来源：http://re.muxihuayi.cn

echo "${s:0:5}"
来源：http://tr.shxzukj.cn

[R23] 字符串替换
来源：http://ij.muxihuayi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pe.colortex.cn

[R24] 大小写转换
来源：http://gs.shxzukj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aj.panjiajie.cn

[R25] 去后缀 / 去前缀
来源：http://hg.newstarts.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ph.gzmigu.cn

[R26] 命令替换
来源：http://mb.9csxet.cn

now=$(date +%F); echo "$now"
来源：http://bs.lnxyls.cn

[R27] 算术展开
来源：http://mz.newstarts.cn

echo $((1 + 2 * 3))
来源：http://lf.gzmigu.cn

[R28] 浮点运算
来源：http://ey.shxzskj.cn

echo "scale=2; 10/3" | bc
来源：http://bz.chemitech.net.cn

[R29] 定义函数
来源：http://ht.yuntaijiaju.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kw.bookmarksfly.cn

[R30] 函数返回状态码
来源：http://ug.521024.cn

f() { return 0; }; f || echo "失败了"
来源：http://rt.hnjuh.cn

[R31] 局部变量
来源：http://fm.muxihuayi.cn

f() { local x=1; echo "$x"; }
来源：http://zf.lnxyls.cn

[R32] 参数个数校验
来源：http://lk.panjiajie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pp.yuntaijiaju.cn

[R33] 捕获错误并提示行号
来源：http://az.nicolike.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uh.521024.cn

[R34] 退出时清理
来源：http://oc.gzmigu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uh.colortex.cn

[R35] 后台执行并等待
来源：http://ja.bjjhwx.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://us.huixiangedu.cn

[R36] 并发执行多个任务
来源：http://jr.521024.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zh.yuntaijiaju.cn

[R37] 把输出赋给变量
来源：http://jn.yuexingan06.cn

files=$(ls -1)
来源：http://ac.huixinmuqiang.cn

[R38] 管道串联
来源：http://pu.bjjhwx.cn

cat a.txt | grep -i error | wc -l
来源：http://es.nicolike.cn

[R39] 重定向标准输出与错误
来源：http://oc.wgjwhj.cn

cmd > out.log 2>&1
来源：http://yd.nicolike.cn

[R40] 追加写日志
来源：http://nv.shtwfgs.cn

echo "log" >> out.log
来源：http://em.nszjky.cn

[R41] 丢弃输出
来源：http://jz.yuexingan06.cn

cmd >/dev/null 2>&1
来源：http://zc.szsharing.cn

[R42] 输入重定向
来源：http://db.huixiangedu.cn

wc -l < a.txt
来源：http://uy.jianghongdianzi.cn

[R43] 按名字查找文件
来源：http://vt.jianghongdianzi.cn

find . -name "*.log" -type f
来源：http://jk.colortex.cn

[R44] 按修改时间查找
来源：http://hq.shxzukj.cn

find . -mtime -7 -type f
来源：http://lc.gzmigu.cn

[R45] 批量删除
来源：http://gb.huixinmuqiang.cn

find . -name "*.tmp" -delete
来源：http://cl.521024.cn

[R46] 递归替换文件内容
来源：http://lq.asd995.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://of.hnjuh.cn

[R47] sed 单行替换
来源：http://am.chemitech.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cg.jianghongdianzi.cn

[R48] awk 取指定列
来源：http://da.hahajie.cn

awk '{print $1, $3}' a.txt
来源：http://pa.jctech888.com.cn

[R49] awk 带条件
来源：http://be.chemitech.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vh.asd995.cn

[R50] awk 求和
来源：http://pw.chemitech.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://df.panjiajie.cn

[R51] 排序去重取前几
来源：http://yu.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bl.huixiangedu.cn

[R52] 统计行数
来源：http://ms.9csxet.cn

wc -l a.txt
来源：http://fu.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://jo.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://no.muxihuayi.cn

[R54] 比较两个文件
来源：http://fe.gzmigu.cn

diff a.txt b.txt
来源：http://rq.newstarts.cn

[R55] 压缩与解压
来源：http://gw.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jc.shxzukj.cn

[R56] 远程拷贝
来源：http://iu.szsharing.cn

scp file user@host:/path/
来源：http://fz.huixiangedu.cn

[R57] 远程执行命令
来源：http://mx.newstarts.cn

ssh user@host 'uptime'
来源：http://za.panjiajie.cn

[R58] 下载文件
来源：http://xy.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cg.szsharing.cn

[R59] 发 POST JSON
来源：http://gd.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xz.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://od.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sl.hnjuh.cn

[R61] 磁盘占用
来源：http://ly.gzmigu.cn

df -h;  du -sh *
来源：http://so.szsharing.cn

[R62] 找最占空间的文件
来源：http://hn.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://kx.lnxyls.cn

[R63] 内存与进程
来源：http://vx.yuntaijiaju.cn

free -h;  ps aux | grep nginx
来源：http://rj.yuntaijiaju.cn

[R64] 结束进程
来源：http://ro.bookmarksfly.cn

kill -9 $(pgrep -f app.py)
来源：http://ip.haigaiapp.cn

[R65] 查看端口占用
来源：http://zh.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sh.newstarts.cn

[R66] 定时任务
来源：http://me.newstarts.cn

crontab -e;  crontab -l
来源：http://ux.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://xz.jianghongdianzi.cn

openssl rand -hex 16
来源：http://uq.muxihuayi.cn

[R68] 计算文件校验值
来源：http://ok.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xh.huanxung.cn

[R69] 生成随机密码
来源：http://db.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://my.huanxung.cn

[R70] 时间戳与互转
来源：http://lr.hahajie.cn

date +%s;  date -d @1700000000
来源：http://xp.shxzukj.cn

[R71] 日期格式化
来源：http://cy.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ns.nszjky.cn

[R72] 等待端口就绪
来源：http://qx.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bl.szsharing.cn

[R73] 分割大日志
来源：http://oj.panjiajie.cn

split -l 1000 big.log part_
来源：http://tz.wgjwhj.cn

[R74] 批量重命名
来源：http://ax.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eb.lnxyls.cn

[R75] 导出环境变量
来源：http://jp.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ol.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://fh.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lr.chemitech.net.cn

[R77] 读取用户输入
来源：http://bo.haigaiapp.cn

read -rp "请输入: " ans
来源：http://dv.szxytkj.cn

[R78] 交互式菜单
来源：http://ew.hnjuh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ez.shtwfgs.cn

[R79] 解析命令行选项
来源：http://by.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pe.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ee.hahajie.cn

time ./run.sh
来源：http://dc.lnxyls.cn

================================================================================
来源：http://dc.gzmigu.cn

S. C / C++ 专题
来源：http://zr.bjjhwx.cn

================================================================================
来源：http://jm.panjiajie.cn

[S01] C：Hello World
来源：http://no.jctech888.com.cn

#include <stdio.h>
来源：http://zr.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uj.huixinmuqiang.cn

[S02] C：变量与格式化输出
来源：http://jh.chemitech.net.cn

int a = 10; printf("%d\n", a);
来源：http://oe.shxzskj.cn

[S03] C：读入整数
来源：http://bz.nicolike.cn

int x; scanf("%d", &x);
来源：http://iz.haigaiapp.cn

[S04] C：字符串复制
来源：http://os.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qt.newstarts.cn

[S05] C：字符串长度
来源：http://xd.jctech888.com.cn

strlen(s)
来源：http://ei.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://eu.huixiangedu.cn

strcmp(a, b) == 0
来源：http://zm.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://wh.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jd.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://tn.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rb.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://bb.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sf.bjjhwx.cn

[S10] C：指针与解引用
来源：http://jm.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://wq.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://gi.hahajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://ri.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://he.newstarts.cn

fclose(f);
来源：http://es.lnxyls.cn

[S12] C：写文件
来源：http://bo.haigaiapp.cn


<!-- 参考信息 -->