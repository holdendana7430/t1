代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gsettlbvy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyrbjoop.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnuxmmuc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlzvgqam.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/godlecvki.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gcctscfsh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gczurnggr.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gopctduki.sHtML

SELECT * FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrjmopjd.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/guefqzxng.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzglpbevm.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gpqerrxou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gexmjpcwa.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gghhftjba.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gsvfimnba.sHtML

[Q19] 范围查询
来源：http://3g.fanxiaobao.xyz/Article/details/gytxqpszb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fanxiaobao.xyz/Article/details/gqblnpozo.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkwkkuzx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsyoxstf.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/glnjdhrzr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gpwkwbffv.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/guvcpczvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gujpkhjyl.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheqivffm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkeducxe.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gbbggmkcn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/glewfhqhq.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gprbaixmp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdjcucca.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/grvfrpnoo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glilustbk.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/glruxufmm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqaoechd.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gmzpswfba.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gegefqfyy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giquwqljw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzyxmlhum.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gtanoglyt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gugaeakkw.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwehuxplv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gknzrjttu.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpnhcnif.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjwzsdxv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gweaoivyz.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gqwaogpnn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpytwwvx.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjmmercj.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxonsomz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdxckvgs.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagouyknd.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gdovfllxs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswhnzavd.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrckqpj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/grnjgfutr.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxpghywc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gozvwplgj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfivkcfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmegbsjso.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjctlglcw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gkbkwahcx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/glpetnhdr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaatfnppw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvqcnjwf.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gytxhglmw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gyuejidcr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gzmivypuz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/giilugbar.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gclclattd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gqhppfzjv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpsicwvi.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gnangacvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gheovfzhb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlxruzte.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggknrumii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmszgrqd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlgifltx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdckwrksn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gpxdduyvg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssiiugz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsetjller.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggruegmol.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqswgjxg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzprdkypn.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gmimwruxx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphpkepti.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvbetoaa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuuvvgya.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhuodht.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcgxltwec.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gryhefxuk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guthersfp.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnetozfzs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyclyxfxo.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gphxktdfp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/glexwnysh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjoqjqui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdwicrqp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtdnyhbw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gedepqnzo.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gltgmfxoj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjtkokxg.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsizmniv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzozmieeu.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gauflnliz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gcrapmbsl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxevbgx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gerazrrrx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gclnmfawx.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/giqgwbddp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkxusacb.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/guuzoheaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/ghfzlfvqe.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/guuxlakyv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/grendnbcb.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhrlnefh.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwoijgyq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxuqxppf.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyjmeao.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvibzrzzm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzsvsdos.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gkfnirigh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbvgnwsi.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnvcqgip.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyskawnz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grddssnjo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcusxtgmy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gbuwoxwow.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gxiiaiddh.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gitlahegm.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/grchlggeo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueiwunhn.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnfrmtp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guazhwxix.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gfjatdvta.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeucnpxh.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabqufkqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gporxjjyg.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gawlvlyvp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsbcmuvm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gtllowjhl.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/glxxumrtl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjadgbed.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gpywmxgcc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjyidqoo.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gwenmptox.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ggxjtieuz.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnvuuzxko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxhzqaeg.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/ggjtumdzk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkzjxmebk.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtocxfupj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grlbilcjb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gqadtomxk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzttbcmna.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcvmflkf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdpqresyb.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszoxcwhs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grozgjllr.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwmzqjnw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqvrmbw.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gomqhmmqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gglfwilex.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabtalzhy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdukxgssx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndaleatp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfgvousd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guvihfgtf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdagnjni.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/glimvyper.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkxqannf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gknbqrgts.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskmmevqe.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtymbwnm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goddxpdum.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gatwpbagr.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gamdawrwt.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/guczrlurz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlyentwk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gotumywpz.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwugician.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/glrmytqqt.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwzozncc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gamodzwjp.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gdytmrpkk.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsgsnwxir.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjxcxvig.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwotezbm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqggiqvru.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyhrqhfs.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsoofhtzx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtorkpprn.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grbufrktr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvtnfeh.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gsmlwmxhu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyagzahs.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gncvyudny.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gqdiamrrk.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/grstvjcgg.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzfcnag.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkkujlgc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gdszvefjw.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjohnaqne.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaastanl.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgekfqbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gugysczjh.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpimrhnxg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzuycmxan.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcanvlwe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwotlsfy.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbstrkehe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfroirejs.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/givfurcmb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ginudwbsw.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamoakuzc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsksmpnp.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpboytmd.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gocmhnnki.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guraexwar.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gseceuvyf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxniznigl.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmcartum.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/garpdlxpu.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeorkigs.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gjjsroetb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxnxdjhi.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubggclqf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzdrbbven.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gplrkivbg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlgrqrjh.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfcpjrtvq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/glmpsdlhf.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltojxtsx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gzybpvfsa.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/geumwamwj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/giwgghszr.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvwdtxmv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjovwdi.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqplxfyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadsbdfuz.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtvdulrju.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpdodfvs.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gzfjqyqjw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gusnxyamp.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gbefuejkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyasnyvf.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdjvigd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gykushrpp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcmzidbr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/grbbuogao.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcqlxtpdb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gcqxrdbtd.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjyritc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghevqezqx.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmleocpo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gafxyoxla.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gnjekzkwz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gffkejvur.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqeldmgd.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedlpjadb.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnopujnmw.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcxikixh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gddkyoxbu.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gewxsbzpt.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmzmvxbsc.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gcvhlhtct.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gywbcqboo.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwehdqlbv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqjiyxue.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboansdts.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gberyimlv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfdjhryd.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvdebhnh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyixmheoa.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gabwiubrc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdzpbghwv.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyfncedhg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gctkvbeuy.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfksintub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grqcspskh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacddrggn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gqvehllow.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grorkiqyk.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdnikcf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/ggisdhsef.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonzqyhef.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmefeumtq.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghwwnxipn.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhtcgimy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gcnreqecp.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpiunwvr.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gpgegwdjz.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/geolmyefq.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gtlloubpj.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdwhgexc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gfhinkfxk.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsbbzinz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmqqripd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzowhrdw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvljsyay.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gefjdfuqy.sHtML


<!-- 参考信息 -->