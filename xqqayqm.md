代发 wailian999

SELECT * FROM users;
来源：http://ye.muxihuayi.cn

[Q16] 查询指定列
来源：http://wp.shxzskj.cn

SELECT id, name FROM users;
来源：http://na.newstarts.cn

[Q17] 条件查询
来源：http://wj.shtwfgs.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tj.nszjky.cn

[Q18] 模糊匹配
来源：http://wp.jianghongdianzi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uj.panjiajie.cn

[Q19] 范围查询
来源：http://we.521024.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zv.nicolike.cn

[Q20] IN 列表
来源：http://se.yuntaijiaju.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vx.newstarts.cn

[Q21] 空值判断
来源：http://jb.jctech888.com.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nf.gzmigu.cn

[Q22] 排序
来源：http://bm.yuntaijiaju.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sl.lnxyls.cn

[Q23] 分页
来源：http://iy.yuexingan06.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nr.huixiangedu.cn

[Q24] 去重
来源：http://iw.shxzukj.cn

SELECT DISTINCT city FROM users;
来源：http://oi.haigaiapp.cn

[Q25] 只取前 N 条
来源：http://cs.nicolike.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jd.yuexingan06.cn

[Q26] 计数
来源：http://or.huixiangedu.cn

SELECT COUNT(*) FROM users;
来源：http://ug.szsharing.cn

[Q27] 条件计数
来源：http://lt.521024.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fi.yuntaijiaju.cn

[Q28] 求和与平均
来源：http://ic.nszjky.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ix.bjjhwx.cn

[Q29] 最大最小值
来源：http://lb.nszjky.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ao.jianghongdianzi.cn

[Q30] 分组统计
来源：http://ur.newstarts.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rb.szxytkj.cn

[Q31] 分组后过滤
来源：http://xl.szsharing.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qr.haigaiapp.cn

[Q32] 分组拼接字符串
来源：http://zf.haigaiapp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ea.bookmarksfly.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qn.jctech888.com.cn

[Q33] 多列分组
来源：http://dr.9csxet.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zg.asd995.cn

[Q34] 每组取第一条
来源：http://by.haigaiapp.cn

SELECT * FROM (
来源：http://zl.yuexingan06.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qz.lnxyls.cn

) t WHERE rn = 1;
来源：http://dd.lnxyls.cn

[Q35] 内连接
来源：http://gz.hahajie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kb.huixinmuqiang.cn

[Q36] 左连接
来源：http://ry.nicolike.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://az.jctech888.com.cn

[Q37] 右连接
来源：http://yw.shxzskj.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://le.jianghongdianzi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wo.bjjhwx.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iu.bookmarksfly.cn

[Q39] 自连接（查上下级）
来源：http://br.newstarts.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gc.hnjuh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gw.colortex.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ie.wgjwhj.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://za.9csxet.cn

[Q41] 多表连接
来源：http://dz.huanxung.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://to.bookmarksfly.cn

JOIN users u ON u.id = o.user_id
来源：http://cd.szsharing.cn

JOIN products p ON p.id = o.product_id;
来源：http://wv.colortex.cn

[Q42] 连接条件附加过滤
来源：http://ls.chemitech.net.cn

SELECT u.name, o.amount FROM users u
来源：http://bb.nicolike.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rv.9csxet.cn

[Q43] 标量子查询
来源：http://fz.shtwfgs.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ih.bjjhwx.cn

[Q44] IN 子查询
来源：http://on.shtwfgs.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xq.muxihuayi.cn

[Q45] EXISTS 判断存在
来源：http://rn.szsharing.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://is.colortex.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dh.nszjky.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uu.panjiajie.cn

[Q47] 与平均值比较
来源：http://hr.newstarts.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wn.9csxet.cn

[Q48] CTE 公用表表达式
来源：http://rs.hnjuh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yt.colortex.cn

SELECT * FROM t WHERE c > 5;
来源：http://rb.bookmarksfly.cn

[Q49] 更新单行
来源：http://wc.nszjky.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bx.asd995.cn

[Q50] 批量更新
来源：http://oi.muxihuayi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vu.huixiangedu.cn

[Q51] 用子查询更新
来源：http://ga.shxzukj.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ks.9csxet.cn

[Q52] 删除指定行
来源：http://lw.yuexingan06.cn

DELETE FROM users WHERE id = 10;
来源：http://so.nszjky.cn

[Q53] 按条件删除
来源：http://rp.hahajie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oo.huanxung.cn

[Q54] 清空表
来源：http://yy.panjiajie.cn

TRUNCATE TABLE logs;
来源：http://vn.colortex.cn

[Q55] 排名（并列占位）
来源：http://ov.gzmigu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wr.huixinmuqiang.cn

[Q56] 密集排名（并列不占位）
来源：http://sz.szxytkj.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hn.yuexingan06.cn

[Q57] 行号
来源：http://rn.panjiajie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://la.wgjwhj.cn

[Q58] 累计求和
来源：http://uu.nszjky.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uo.hahajie.cn

[Q59] 分组内累计
来源：http://ju.gzmigu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uv.muxihuayi.cn

[Q60] 取上一行 / 下一行
来源：http://jr.muxihuayi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ib.bookmarksfly.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qr.yuntaijiaju.cn

[Q61] 移动平均
来源：http://dz.szxytkj.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oa.huixiangedu.cn

[Q62] 分组占比
来源：http://rw.hahajie.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kk.9csxet.cn

[Q63] 开启事务
来源：http://to.bookmarksfly.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oy.huixinmuqiang.cn

[Q64] 提交事务
来源：http://ic.newstarts.cn

COMMIT;
来源：http://de.szsharing.cn

[Q65] 回滚事务
来源：http://su.nszjky.cn

ROLLBACK;
来源：http://lf.shtwfgs.cn

[Q66] 行锁查询
来源：http://ib.huixinmuqiang.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pz.lnxyls.cn

[Q67] 设置隔离级别
来源：http://co.yuntaijiaju.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dh.jctech888.com.cn

[Q68] 保存点
来源：http://fe.huanxung.cn

SAVEPOINT sp1;
来源：http://qu.shxzskj.cn

ROLLBACK TO sp1;
来源：http://iz.jianghongdianzi.cn

[Q69] 查看执行计划
来源：http://kq.chemitech.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eb.nicolike.cn

[Q70] 更新统计信息
来源：http://hj.yuexingan06.cn

ANALYZE TABLE users;
来源：http://dl.bookmarksfly.cn

[Q71] 查看建表语句
来源：http://wz.szsharing.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pu.bookmarksfly.cn

[Q72] 查看索引
来源：http://pw.huanxung.cn

SHOW INDEX FROM users;
来源：http://vf.shtwfgs.cn

[Q73] 查看表状态
来源：http://wh.colortex.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oo.hahajie.cn

[Q74] 强制使用索引
来源：http://yw.szsharing.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ds.wgjwhj.cn

[Q75] 日期格式化
来源：http://yh.jctech888.com.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fh.nszjky.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gd.lnxyls.cn

[Q76] 按天统计
来源：http://jg.yuexingan06.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zl.lnxyls.cn

[Q77] 时间加减
来源：http://zu.nicolike.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://px.shxzukj.cn

[Q78] 当前时间
来源：http://yr.wgjwhj.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bu.jctech888.com.cn

[Q79] 字符串拼接
来源：http://ik.hnjuh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://km.521024.cn

[Q80] 字符串截取
来源：http://lj.hahajie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jc.shxzukj.cn

[Q81] 字符串替换
来源：http://uy.9csxet.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yy.jctech888.com.cn

[Q82] 字符长度与字节长度
来源：http://cp.nicolike.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sv.muxihuayi.cn

[Q83] 大小写转换
来源：http://rl.chemitech.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qf.yuexingan06.cn

[Q84] 去除首尾空格
来源：http://go.9csxet.cn

SELECT TRIM(name) FROM users;
来源：http://hs.gzmigu.cn

[Q85] 数值取整
来源：http://zz.hnjuh.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ef.huanxung.cn

[Q86] 读取 JSON 字段
来源：http://bk.huixinmuqiang.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oy.shxzukj.cn

[Q87] JSON 字段做条件
来源：http://wt.521024.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://id.szxytkj.cn

[Q88] 行转列（条件聚合）
来源：http://le.szsharing.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ch.huanxung.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bq.hnjuh.cn

[Q89] 判断表是否存在
来源：http://tv.newstarts.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dr.szxytkj.cn

[Q90] 生成序号列
来源：http://hj.hnjuh.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://df.9csxet.cn

================================================================================
来源：http://ph.huixiangedu.cn

R. Bash 专题
来源：http://oi.shxzukj.cn

================================================================================
来源：http://kb.nicolike.cn

[R01] shebang 与严格模式
来源：http://ap.hnjuh.cn

#!/usr/bin/env bash
来源：http://ik.jianghongdianzi.cn

set -euo pipefail
来源：http://fp.nszjky.cn

[R02] 变量赋值与使用
来源：http://bj.hnjuh.cn

name="Tom"; echo "$name"
来源：http://aj.shxzskj.cn

[R03] 只读变量
来源：http://uq.shxzukj.cn

readonly PI=3.14
来源：http://mi.panjiajie.cn

[R04] 位置参数
来源：http://gp.nszjky.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zi.newstarts.cn

[R05] 参数默认值
来源：http://nb.shxzukj.cn

name="${1:-default}"
来源：http://lx.yuntaijiaju.cn

[R06] 判断命令是否存在
来源：http://lu.yuexingan06.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qa.bookmarksfly.cn

[R07] if 判断文件
来源：http://dg.521024.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jc.hnjuh.cn

[R08] 数值比较
来源：http://hy.szxytkj.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ga.asd995.cn

[R09] 字符串比较
来源：http://zx.haigaiapp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ch.yuntaijiaju.cn

[R10] 正则匹配
来源：http://ex.wgjwhj.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tw.newstarts.cn

[R11] case 多分支
来源：http://cc.huanxung.cn

case "$1" in
来源：http://ud.panjiajie.cn

start) echo "启动" ;;
来源：http://rv.nicolike.cn

stop)  echo "停止" ;;
来源：http://gx.jianghongdianzi.cn

*)     echo "未知命令" ;;
来源：http://kq.huixinmuqiang.cn

esac
来源：http://qj.huanxung.cn

[R12] for 遍历文件
来源：http://ii.asd995.cn

for f in *.txt; do echo "$f"; done
来源：http://nm.huixiangedu.cn

[R13] for 计数循环
来源：http://cq.bookmarksfly.cn

for i in {1..10}; do echo "$i"; done
来源：http://qc.huixiangedu.cn

[R14] C 风格 for
来源：http://ix.asd995.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ql.wgjwhj.cn

[R15] while 逐行读文件
来源：http://fd.haigaiapp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mr.newstarts.cn

[R16] until 等待条件
来源：http://nw.hahajie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dq.wgjwhj.cn

[R17] 数组定义与取值
来源：http://xs.colortex.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gk.colortex.cn

[R18] 遍历数组
来源：http://jd.colortex.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://db.nicolike.cn

[R19] 数组长度
来源：http://hu.asd995.cn

echo "${#arr[@]}"
来源：http://mk.521024.cn

[R20] 关联数组（字典）
来源：http://yi.lnxyls.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ws.nszjky.cn

[R21] 字符串长度
来源：http://ce.szsharing.cn

echo "${#s}"
来源：http://qs.lnxyls.cn

[R22] 截取子串
来源：http://nw.yuexingan06.cn

echo "${s:0:5}"
来源：http://fu.szxytkj.cn

[R23] 字符串替换
来源：http://ru.nszjky.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bt.chemitech.net.cn

[R24] 大小写转换
来源：http://rk.szxytkj.cn

echo "${s^^}"; echo "${s,,}"
来源：http://de.szsharing.cn

[R25] 去后缀 / 去前缀
来源：http://gy.yuexingan06.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vn.szsharing.cn

[R26] 命令替换
来源：http://ws.lnxyls.cn

now=$(date +%F); echo "$now"
来源：http://wl.nszjky.cn

[R27] 算术展开
来源：http://vy.yuntaijiaju.cn

echo $((1 + 2 * 3))
来源：http://dj.shtwfgs.cn

[R28] 浮点运算
来源：http://he.hahajie.cn

echo "scale=2; 10/3" | bc
来源：http://pn.nicolike.cn

[R29] 定义函数
来源：http://br.colortex.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yh.asd995.cn

[R30] 函数返回状态码
来源：http://gq.gzmigu.cn

f() { return 0; }; f || echo "失败了"
来源：http://lp.panjiajie.cn

[R31] 局部变量
来源：http://nz.asd995.cn

f() { local x=1; echo "$x"; }
来源：http://dj.bookmarksfly.cn

[R32] 参数个数校验
来源：http://nm.9csxet.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://br.jianghongdianzi.cn

[R33] 捕获错误并提示行号
来源：http://dj.wgjwhj.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ll.yuntaijiaju.cn

[R34] 退出时清理
来源：http://pw.muxihuayi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tn.lnxyls.cn

[R35] 后台执行并等待
来源：http://au.wgjwhj.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cj.muxihuayi.cn

[R36] 并发执行多个任务
来源：http://fa.lnxyls.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wi.jianghongdianzi.cn

[R37] 把输出赋给变量
来源：http://ej.szxytkj.cn

files=$(ls -1)
来源：http://um.yuexingan06.cn

[R38] 管道串联
来源：http://qn.muxihuayi.cn

cat a.txt | grep -i error | wc -l
来源：http://xe.muxihuayi.cn

[R39] 重定向标准输出与错误
来源：http://ro.szsharing.cn

cmd > out.log 2>&1
来源：http://nu.hnjuh.cn

[R40] 追加写日志
来源：http://qs.bookmarksfly.cn

echo "log" >> out.log
来源：http://dw.colortex.cn

[R41] 丢弃输出
来源：http://pj.hahajie.cn

cmd >/dev/null 2>&1
来源：http://dn.asd995.cn

[R42] 输入重定向
来源：http://cb.hnjuh.cn

wc -l < a.txt
来源：http://ke.lnxyls.cn

[R43] 按名字查找文件
来源：http://hl.lnxyls.cn

find . -name "*.log" -type f
来源：http://nn.muxihuayi.cn

[R44] 按修改时间查找
来源：http://ap.9csxet.cn

find . -mtime -7 -type f
来源：http://ak.bookmarksfly.cn

[R45] 批量删除
来源：http://pr.bjjhwx.cn

find . -name "*.tmp" -delete
来源：http://ww.chemitech.net.cn

[R46] 递归替换文件内容
来源：http://pq.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zf.huanxung.cn

[R47] sed 单行替换
来源：http://ht.huanxung.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vz.shxzukj.cn

[R48] awk 取指定列
来源：http://nt.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://tz.colortex.cn

[R49] awk 带条件
来源：http://gc.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hs.yuntaijiaju.cn

[R50] awk 求和
来源：http://al.shtwfgs.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fr.jctech888.com.cn

[R51] 排序去重取前几
来源：http://mg.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://at.wgjwhj.cn

[R52] 统计行数
来源：http://ub.haigaiapp.cn

wc -l a.txt
来源：http://qz.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://dk.jianghongdianzi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ar.szsharing.cn

[R54] 比较两个文件
来源：http://bv.shxzskj.cn

diff a.txt b.txt
来源：http://yf.bjjhwx.cn

[R55] 压缩与解压
来源：http://bp.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fo.shxzukj.cn

[R56] 远程拷贝
来源：http://oy.asd995.cn

scp file user@host:/path/
来源：http://si.gzmigu.cn

[R57] 远程执行命令
来源：http://fw.muxihuayi.cn

ssh user@host 'uptime'
来源：http://vr.huixinmuqiang.cn

[R58] 下载文件
来源：http://eb.huixiangedu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bl.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://wo.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yk.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://pr.yuntaijiaju.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tl.panjiajie.cn

[R61] 磁盘占用
来源：http://yk.bjjhwx.cn

df -h;  du -sh *
来源：http://oe.asd995.cn

[R62] 找最占空间的文件
来源：http://zx.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://ul.haigaiapp.cn

[R63] 内存与进程
来源：http://tc.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ow.chemitech.net.cn

[R64] 结束进程
来源：http://ui.huixinmuqiang.cn

kill -9 $(pgrep -f app.py)
来源：http://jn.chemitech.net.cn

[R65] 查看端口占用
来源：http://ur.bjjhwx.cn


<!-- 参考信息 -->