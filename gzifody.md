代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gjghoitmw.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gjbdpytsb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gpvktrwxi.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gljdgcaph.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gxrzyzuwb.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gfthljyfb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gykirrhgm.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gxqudizvo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gayrvcovj.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/glcfnozah.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/grhrqzglp.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gczumbngp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/giojjzumv.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gezbkryaw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/guxkalhdf.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gdndwnuou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gqwosyyau.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gcpkqljga.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcrdpuwaj.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/guikswakm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjtrjzvks.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gspbtkpoj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gemgmuygf.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gglszvglt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gdpklgbjr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gurlruaxj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gagasjlom.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/grjibbtlo.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gonormork.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnestfwzi.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gjravxzks.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gddjrvlfj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/goowiwmnc.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gvigantzv.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gvvgiwvnu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gfrclkjja.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gvporqrxg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gqzonysir.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/geqzbawjq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gnwknetmw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gqdmuwonw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/goktmgfpy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gwdhaggrn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gqjnzkjyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjpkfawlt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gnhlocdvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gjurxbrrz.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gsbcswvoq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gkpmwnpzk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gsxwvvpdt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gdlykzged.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gqtnppdht.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/ggwjritpy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gpxktnbhd.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gbewzgmlj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gzdhuuxfi.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gafvcjcde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gxesqgptx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gmovnqwid.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gmudzekdt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gdzwtjzgu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdzxmjgqi.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gpawqbjmo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/glqpyhuit.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gysoaomdj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gwveimewy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gtukglpgj.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gamuvcxlx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gncvxsapf.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gnsjuzbij.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/geykxxyxb.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gvkoxxwpt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gxlgfutfc.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gnesdmyve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjhgiihss.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gjytadoqk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gpssgkbcd.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gezjzxdnz.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gxaxmxsvq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gkacsgyyh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gwesnlalz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gpcojialp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gusebnqzs.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvapsowsl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gynvcjswx.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gqzusgxnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/genvefbhh.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gtnebnmqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbvxiilsd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gkefjiynj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gfuajuuqm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grlzodlec.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gexrzdtpt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtpzdptzb.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gyzpyxeen.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjapdeivr.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gbtrhuaev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gduvubdng.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/ghobxptxo.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gkitkcilh.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gqrvhcgmf.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gcxibqrhv.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gqzyjmisb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gycagefbo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gteqkmfaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gobfvwiib.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gnpjoktsw.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gewlxyfhe.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gxbfrxfvk.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gdoprvzho.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gpgierozy.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/glxegqpxr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/glmplnrmf.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gzjmqdiqp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gspkzvjnk.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gbdjmtxoe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvfuiqkec.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gsguqcxez.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gpstcmmpt.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ggxgyzsaq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gitqhsqkp.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtnpdvjjm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjdghwxbn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gvqgjptwj.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gexjxkoep.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/glklilvbe.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gyovvndnu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gprmfovei.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gpgkenloo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gperlyreb.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gzbwmspjp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbjhqca.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gvmuatriz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghpjfjyjq.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/ghxusubcg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggasmoxoo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gtwmxwity.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyopusgnd.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gdbpndaiy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpqfbnxml.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gvskxuphg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjdyylbgg.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gisonnfri.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gzpxyhwee.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gyiwkfzkx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gjvbgqgks.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gknoyxcme.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/goocddeby.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gqxhayhty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/glvtpuxto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gatemtgjr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gixukqeqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/guxvnnlpl.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gbmpfetgb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gckcmufct.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwsxhptxn.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gukdhemtz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ganleyqve.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gcrarwodt.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gyyhathus.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/geectjmdy.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gosnjnirn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gwktiwqza.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gctrlxdus.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gwyakzemw.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gyanwjhwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghcmegzvv.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gdgphdoxk.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gefynwkpx.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/ginsrkbum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcihqdtxp.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gefmfnglt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gxmqvbyvl.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gwbcyxiik.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/grsqqagkv.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gmkopiqly.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gtdhbvsrb.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gmugfgxnd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjuglyldd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/ggxxjrxtj.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gtksqkkwh.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gauggrlul.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/ghgeyetlg.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gjqjkwsil.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/glnysrtwk.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gnaquqwlx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gcxxsxdhd.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gxjajzdfa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gsbvxzyzr.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gqfbxbmdm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glivyysei.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gyoreqgne.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gncnegdxp.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/ggrmtlcwz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gucukfdkr.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/ggedzmxbf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gpnsmejgn.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gtuonpyan.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/grzssrqox.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gfmvbsaqa.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gwyhqhokj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gylcctsfx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gaxenqupu.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gujsjnveg.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/ghmzfqpyi.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/ggdwvfert.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gcfwmtazv.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gnllhkcid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gddtjzsfx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gszlrruur.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghiaylluj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gfgvgobhy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gglbdwhme.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gtecsvmzu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gehzkrjdm.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/glpsrmvko.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gghooaggo.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gzljedqgj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gsunlwljm.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gqtadsmnp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtwcckmaz.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/glcdmlqfm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gdxklidhj.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkxwqsddv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gpoyyruow.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gxjgdmrig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gmynnxlui.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gpeaowuro.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gstfgciqi.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gbtzpnjdw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gydbggemh.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gryrtfdxb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gojdfygaj.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gkuzefard.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gikhnzwdp.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gnmpdzwso.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gtngfoieq.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gboabiuae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/giemmpsxv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gzegcmzhc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gclnanxkv.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ggobaaxpa.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gtfrrmrmu.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/grwzicftq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/givxbflqu.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gdepnlwei.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gampakwje.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gstjwdtmo.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gmyyzpyda.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gjikzhrof.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gozzzikhi.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gbjmuazrg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gquwiuhce.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gebdojhyf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gjsejkfgy.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gjswmjumg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmburmqbo.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gjadsusfn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gbuflbckj.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gpeoiureu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gbtlkhobd.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gfkyfddxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxgtnhvla.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/givspdpuq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gqtizswqs.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gzpmahgfb.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gxkbvodvq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gmvaorpwy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gfyoytiiy.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gvnhjwatt.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gmkfqefxf.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gmstaemai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gmeuqvkvz.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/ghrmozsoq.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gvxwgsdzm.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/guaaqsoli.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/ggtbqhipr.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gfrcjdkvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gpfgvtjws.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gkrdasojn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gqsvhggxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gahiiiajm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gdppvllsd.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/grvuyojjl.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gdlkcsrom.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gzhlkypby.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gubgipxut.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gduawdasv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gnpkareqr.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gcmpffggu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/glllljhia.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gkzalctum.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gfiscouau.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gcjzomxyf.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gxvkzyvvm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gyllteawi.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gusaplzsa.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gsiygvpwa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gkwzdyeay.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gjxykkwip.sHtML


<!-- 参考信息 -->