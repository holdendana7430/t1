代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchcrinva.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrhgthtq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gukedhizg.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtvlbgsd.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoyjxoyv.sHtML

[Q16] 查询指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgplynxl.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmdcqna.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/glilpunot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmyskfrl.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvfwfedqq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoqjlzbg.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gyeekiwwc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmirvpe.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwyqcurl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqgxhixx.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkpeqtsj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmvpkujq.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gnfrmxrqn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcbzlual.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjrmhhdu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gojnwkfia.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnqrpzbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgsgcoyq.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/guhfkqzdk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzbcpyif.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjchwgxmm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsngofof.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gwwahopmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gziopgrfc.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyyvvwzn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaaqnyyn.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gltjfbrie.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giyevhgph.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/glulpngzu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuwfjoce.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuitbaqb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guujqbsud.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyiolbab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtncpjq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxgxxxka.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gpuiyasgr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjqupvlr.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gvjerltit.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxojogygf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/ggnsflhee.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrbbgfv.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gbcrlmnrs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrnlcqwj.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gypxbrlkn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gerrcffql.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/grsyfqoxm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/goyrznnay.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwiygfwr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkurhary.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goplnbsnv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdhltkfc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkkqqegvm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmskwmanf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdikroy.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfwxuvuc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyuqdiil.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gyiajtrrg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxyygzeb.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gahmscvxk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/giwtydqbj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnmcwcxz.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/glmcwkfdu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gjbxkhhei.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtohnqsee.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gwbdxqjzc.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gzwekuucm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwlziqgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gspdfdmtv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzioemgfv.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghknwupfs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhjetber.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhtasegc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gdilxxbdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gwvhjbdkx.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfnoecon.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gymedjkbd.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/guvauvood.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gwjeshzhl.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgmxbzdb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyyddmiu.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/guaivzqhv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnoadzsp.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmpwcfkr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gziidwmup.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqqnutt.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gloprbrto.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyeelzaze.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggghpegjm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gavxhgerx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppfjkncb.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnvytbue.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guyjvlceu.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlvutzio.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmtjibj.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gshupqdrr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grqhssgum.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gnekgiufm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gyhlowmlj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdyuoemm.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtddvgg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/geejaeabj.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/ghhbbjnob.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjfcgbha.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpoxtmpo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/ghfaaufzk.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gbtokafdg.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvoebaws.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gnbmwtwzh.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gjevwbxax.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnslrxvs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gdexmnsza.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gajyiqybl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmkynii.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/ghimstkfp.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/grdisynsv.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gusqducrz.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvutfauit.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/ghqdnfapy.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gkixzokax.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtpicysy.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gcgmqcsce.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrcuuohs.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gzrqycdwb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxfavggb.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gxrjsclme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqkcnqec.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/ganlqtqlb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnamwfwga.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsavaosiq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujytokf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbjletoq.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gmbgifgwz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxtcdexb.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gybjghqgc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gietsnkky.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhkjkrk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyjhxqmb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxvgnrcy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gzlgtkmus.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmduugcm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkolvklhp.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtgolybk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqowykau.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqondyy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gebvcgttg.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrpgkwj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpwluezs.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/glrijblny.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyvhhyuz.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gpvuukihv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gleksaqjz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcslvtsds.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gkuockgke.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gpskywnyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gojakdstz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/glysznwxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gdgkhwmtb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmbsmggr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwxlltldn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gchqwusrd.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gohajqktn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gepzgstid.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnhcaddpm.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwfvrfhn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxuqyidf.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmtzzybe.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghunlrhiw.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gjmqfarok.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gqcyekdjc.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/glzhugoeg.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsdaifn.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/giepzzyhw.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcaipppev.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gisvybtnk.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/guuqqxbsk.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/grkhvwtya.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gajuairmf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqdagdcx.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdsvvqmop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goxxnfvsk.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaddveac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzpeiceh.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefysswtm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gaiekjwxw.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwinzjhev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmzsfcxh.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grerlqmja.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmnoguq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojpsoktf.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdpfuqy.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gafcdamat.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gcvvldrtx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxnipahn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvmlegcje.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyupubwel.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gumussuxk.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gqobufvsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkhudtb.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwtzyyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkyrbwaf.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciwgtwxn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbultsqz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgglqbrj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwxcadqw.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkmkzrbyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gckngtane.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjzmvxreu.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrzygkzb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaheqzhb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcxnyiop.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmohetec.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqwwcxceb.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtetsmamt.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxgyqawhz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfyfrlj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gmhisokid.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyslsfqf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gigbnjfnk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpflvyhuv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/glaxuxsxv.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxxflekt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagqqtgu.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gzgfxflda.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjhsphp.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyufmfui.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpibjxwax.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/guaojaynk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkcescldl.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gumubxabt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gjytgeuet.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfwvoqhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhwfbkmr.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/galslzaqe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwrgnkdn.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grwrevynx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gggyzldhx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gwjjdgdnk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeskobck.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaomdnvj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gylsqzxsd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjuzncxr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gjuvauuvv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixwfwmkb.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqwzlicow.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqndbvv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/glcrymrhy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ghmkmobcx.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/griisqagj.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttkpdpoe.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbplwmajq.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/grxmwkyak.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/guqvbirmn.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gxpembgxo.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtoywkbz.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfimempky.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gavegjkld.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwcfwnnb.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gopqwkggj.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgykwvhm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjljwfxnk.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/guzvymvuh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/goordzmky.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbwksfhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggczmbdle.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbkptkwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gferyastz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwnhlra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvigjppdh.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/goyhgbnki.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzjexnsh.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxrgxeqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmraqcaq.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwjezplw.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgelpxsl.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gizewjkle.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvvfqptz.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndykovy.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gngytmiey.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkrwinvw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/glkzuwieg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfnagrkwb.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/grwwrsilp.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/godguyioi.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptjanyjg.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gskorbxgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gzciysknz.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ggvwiormm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbpphsl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdzywkfv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvbvbgn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycbtpelj.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/geqebtyin.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvumbpyng.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjelfmmc.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvyxghjov.sHtML


<!-- 参考信息 -->