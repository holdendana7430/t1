代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghfbisdqy.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqedknjhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gjkhufpwn.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gbejakqlr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gniupflxz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gisowbzdz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/grkpihpca.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/guwppymom.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gapbwujmd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gshfagoco.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gfonobpyv.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcbquczns.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gbkwruwyq.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/ghlgpytwl.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/ggocjjama.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gonjbmhzp.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gdctppnla.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gnnikezdl.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gqfgyvnai.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gupgubbqd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/glvgwzhez.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gnhmbfvml.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gztytrbxj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gsewpvuri.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/graodhaxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gmxjjqwdv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gpgsrhjoe.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gablnrhgd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/guxtsinfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gmzddgrnq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/goezilucu.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gbptupslo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gihjhkkje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gcqbfqqnl.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gfxayujyg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/ganzxlgvl.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/grvhwbjip.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/geblopmuj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/goxlkxysn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gpomdjsgc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gnyrqxtvy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gqczdouxg.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gukwnarwi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/ghiugdsfu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gxvbsqcjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gldioakmw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/glhmkhluk.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gryqloarx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/goutuvngp.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gjzymtdsu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gteualspd.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gjltpxoau.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gfamktwvu.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gzsvpvkvd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gyorhrwes.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gbcrnkwpd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gnrdngcxp.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/geaihhhle.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/godkmjtmq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gvetovtnr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gwscihdpv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/glznfziuc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gqlzljgwe.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gkghcehfk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggwkybsdg.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gjprioysj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfmliuotf.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gomcqfnrc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfbjjsqqp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/guwpaudoj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gxynmhxdw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzftebonl.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gvmjhlsoh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gudmssrot.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gnwsypzqs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtgehutim.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/guxfivfms.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gmnecetim.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gwuxnnwsa.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gijvbupgm.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gjxougsjq.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gggatxcbb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gprugoftj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gdukojfze.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gtxjxgikh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/grbqshhsf.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/geenwkoyu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdgcasdeg.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gttrtlshv.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gnfrufhkf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gemyqzgae.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gcsptdrcw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gxzyrojsr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gyfiywoma.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/grrczrsjk.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gxfeeqixk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghtzujtev.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/ghzwhwjjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdaceknhq.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/glhkkgmir.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gcfqmqcvn.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/grijqrzqx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsbcmrmwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gcwtqrqrr.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/giqbufibv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gzuylvffo.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gvaonpyvg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gajstojof.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gjhacxnqd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gtxptxwav.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gpfswzvns.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gezizatjl.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gjtjwedkd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfgoyohuh.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gbvfzqibi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/goluruvph.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/grmolhpbe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbhikhzde.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gxooyhtkt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmjfiycgu.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gstjvvzdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnrdnkgwq.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gtfrxnpgq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gjnpldklx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gvznrryqf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/goglqleiz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gjpplcnoy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gbkxysowh.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/geqtldimx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gaejemjst.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/goutsgodo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gmicuyqmo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gdehwujxr.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/grqbqmjby.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gvlkkiqlg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqxgnhvqi.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/grvylerxt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfknqdutn.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gxcftmtus.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/glckrdmyy.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/grfglpong.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/grnngxpau.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gerowwkws.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gmxhelbou.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gmwtecduy.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gypzusjnn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gydfvynzc.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gxrflpzvv.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/guiurcrkg.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gzezlypno.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gcjseslvj.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gojcezbts.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmbbnlqpv.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/grnxxequy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ggiqwtfkz.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gugskwaxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gpbhqrhka.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gzkgolfrh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gdldhojvx.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gmiehxpof.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/goelmaaoc.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/grhmftbjp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gakhzfdlh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gvlsogqwj.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gstkegrtd.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gnoxlghad.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gkuwpqkfn.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/ghgqgkeed.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gzqcjsxcx.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gyyvaihxi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grotuqulx.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gabyhseys.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gfcncrbas.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gbcantflu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gefvfjzss.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gubrznilr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gyfpsuket.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gnuviiqlo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gmdrzhddz.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gowimoeec.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gcjjgxixi.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gyxxzygmw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/grezpwnrg.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gbhnqmjjc.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gbxupjnws.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gaaatmdkk.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gdjdaqaka.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gcxltgpps.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gdjwjsdse.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gippzsled.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gitzrwvee.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gmyspcmxf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gwfmafnmh.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gwnrxosvm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gfokfjcnb.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gepoffeaa.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gogobbquk.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/grurzuluc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gawsviwhp.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gutmnezoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gyjxgehum.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/goiuushxi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gsyyhhlmn.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/ghgrmwfry.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gwmebalqw.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/ggoexrlbx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gpupnhxrm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gjsrlgapc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gezqkrrgj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gwtintvjb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gunfkoodk.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gxaeunliu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gccqapaiu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gkzlgntzj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gteygcgxx.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gfewkioxb.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gbxnhkwzn.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/grkdbbkwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gbmpalbci.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gqibujyay.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gkizhbjbu.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/glviyoame.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gjkmafmwg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsvwyaiyr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gysgtizaq.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gidqzmbjy.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gkemmmwrp.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gtnpubmbs.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gkpeknefd.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gcytpblkt.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gyaykkcqt.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gayznvqan.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/goqglnqvj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gndaagbrq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gvuyxvedz.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gvssrxiem.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzhcmdard.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gwlrtdyer.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gxbztzfjm.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gclbxpgwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gagyafvor.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gxsmkiavf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gjfwukbvg.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gcqemuuvz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/goiffjjxy.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/glomsgbno.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gpdyvjdaa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gcevzcawc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gauuhbccg.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gnxsjfitn.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gfrewlpxj.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gzdljzvcd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/givmjmdus.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gqocnwkve.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gioprbyhg.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ginvmybst.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/geruowjsx.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/ghhmowrsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gfmadhyqe.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gtfdvtgns.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/golschgou.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/girehexhy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gnuixluxr.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gnbyfgnqs.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/ghndjdrlr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gniffnveg.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gzievifok.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gbsdezdck.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gbjscqqmp.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvgnjtrth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gnhlzjkeb.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gevujzyba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/glkqwifss.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gtrprvzlr.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/glxewzofo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gqroweprc.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gnlndtojk.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gpnoiyfac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gevbozqfk.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gyufnlwhp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gazobrcel.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gwgtwntqi.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gefhgzhti.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gvrodlkdo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmonqpsev.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gholkkiao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxewjpcst.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gkienjzkt.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gqlghwsby.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gnmknjpkr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gvetgwynm.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/ganjsvzsk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gkjzjakih.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gcakvxdrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gzqnovbvq.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/grinhrtvf.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gzzxopdte.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gusozitkq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gxlufbkpq.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gxrlloqzw.sHtML


<!-- 参考信息 -->