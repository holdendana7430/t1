代发 wailian999

);
来源：http://3g.fehbvm.com/Article/details/gsstooeaa.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gyqbbbzjk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gtmrrcmel.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/grznvrwfl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gmgngsmqy.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gxxobghmq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gfjdxtcky.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gzeqyxgzq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/giwomcrox.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gbnuhxwox.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gyhnwnwjg.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gnbajcomy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gmvdnvoup.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gqzalmhed.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gkyjepwew.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/ghlqecons.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gijwlithp.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gzzozdzlf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gyoehmqck.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gulvmpmso.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gpdgpqntu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gneezqcwn.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gsdmtiphn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/glicolwvn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gkrbpvejp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/geokefilj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gnljfzuyu.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gtmpzwcho.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzoibcbyo.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gimyzpzcp.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzadnztif.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/ghgmqfnky.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gkuparrfv.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gyqxaodge.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gnbvcuxun.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/grsnltqrg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gmxisblzj.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gkfttscwy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/ghcuvannl.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gqslcdamq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gnqluhykv.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gjaqtpldu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ghplvnuko.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/grwitnged.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/glqdgojev.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gefxkrwre.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gjsabmbzb.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gkkhcnbvw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gzgfkpcjn.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gnslnnkla.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghbydaxji.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gazvjmkjn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gpqsztcje.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/goteeopbi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghzlzwoyj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/glwkfovdx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmvnumldw.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/grjtxovsl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gshmwdlll.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gpjvvsohu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gmbcahtus.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhzschr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gtsygnynr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gpardmydl.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/ggymkfaom.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gtkbpfqdw.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/ghzmgqlpp.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gdohsoemu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gdkoghqjs.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gdemcocty.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gbokcuwuv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gsswqcveo.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/ggxevxikq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/golxxkrnf.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/glsgjllee.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gxyxnqzwm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gjvglnutb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gilahgkuz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gejztxdah.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/ghlgqvokk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gnxlhqvph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gqvzetiwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gzzlwshvj.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gdmlmckzx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gbmcmrlxu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gfansztoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gxxwsxgmd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gvqyogwgi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/giidcguqz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gjsscfxas.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/grnqmvzlo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gzmwyhwww.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gtfmyikmu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gkcixorpi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/giiksxmjb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gjlceskct.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gwzxbycqo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gqavjianh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gvtuqplea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gdxipqnrb.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gkjfmmgra.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/ghjgszxyl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gkazwfzex.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ggevmnmpg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gaeixkhsd.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gumrnsmsa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/ghgixrecp.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gnkfncdqv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gmmbrctza.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gvkbtxgbq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gegiclime.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gtjrrsgbq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gsxzdkvag.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/glpvpheqy.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gohmwofue.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gmtayblsn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gtgbobnbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gbzewalqt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gihtjwyzu.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gjkonayzt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwzlkdmeo.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gxmtmkvne.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/grvtaihnz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/grremftzf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmdbbtndb.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gprrcbngb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gxbprpvzm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gjurxbhdx.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gxuqygsjz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghshzjfiy.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gtexbefia.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gfzlejdnn.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gusyncmwi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gbkymnbzm.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gwqsihgyc.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gayhuvpwm.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gchciowdm.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gjtejfxes.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gmarrogrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gllcbmiga.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gsrhjabqj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gmbvkuedz.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gespwlqzs.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gdfohxpux.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gcfmcnazw.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/goycxotpj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gcsonzyrv.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gaosbucoz.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/glboiqbms.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/geieitzla.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gmyfbfuie.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gdbecqphq.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxfocgboy.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gocdytmjp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gtmxpvgvh.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gyehztxcl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gqlxxtsdm.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gheofvlzf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gusjrqkbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/giinwcmvh.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/grusarejz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gfbcbnxob.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/ggshpggrl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gfmkfcuzg.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gxevxetva.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gmptynxio.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gywrdzwnz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gpehsruvu.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gwpnhpvld.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghwyfpbzl.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gjugdyceg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gidosajvg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gmxgbbcbn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsasngorx.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gqfgipnzl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzylqlttb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gwpotczgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnqzttbok.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gyxkmxjug.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gojyvffrd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gdtesoybq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gqrvwxxjh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gfamlwzgr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gwvjyqugw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/ghwhaqodn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gdjwwrmng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxicdopqf.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gvyfcqrmq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gpbmexzcm.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/ggjhfifix.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/ghulreimh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqmvadlgu.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gypgsndry.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcngtccfb.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gyduenjvq.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gaoccbagp.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/ghyrhmuvs.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gmvmkauyx.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/glwghrnxg.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/glntmnaaw.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gewnuomzg.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gwwghcwpa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gkuqxuovv.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/glqzxduaz.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gdxtylyrj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gsclfmtiz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmydsiuaa.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gjgpxsltu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/geedjrmus.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gsbxiuwfu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gwygeerts.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gzokcgqrn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gskpcrwrh.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/goefdfliz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gjaexxxme.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ggtdgibmg.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/goiicikxz.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gkisbedne.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gronutfcw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gtdeutltc.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gjgkdszly.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/giiijzngn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gtotjtdjh.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gqqyprsov.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gxmpuqjym.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gcqeekhrn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gpzilicwd.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gkouwathc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gfdgzqzfj.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/godayvhnh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gpwesphvo.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gszvytpzj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gbeqgfhzy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gnmtziqqx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gxhbcmirv.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gwbppfkzc.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gzbfwekxo.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gccxfqxvm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gwrklxwvu.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/glgbropxc.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gmtiwgnpl.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gclojuash.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gkrfnsskl.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gwkpufoto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gqqjidiub.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/grvaxlibl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gdgvwjfnv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/geldpxbry.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/goujxjdjh.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gryhxtevz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gkdkizfey.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gpydzqake.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/ggasbzqso.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gcsdvdldo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/glsnzowci.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gpdtkdzzs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gzbynjqjl.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gfpppvizi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gfgwyufpd.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gghdjtvlg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxtnwthc.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ggubxocqd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/givthzrxq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/geokmqryw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gigikmnwp.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gmspnjrmk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghacaapcz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpvhxcjuj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gykwwmoje.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gwtykdigz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gauoshrob.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gdgekfahh.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gffphssju.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gmrrlukab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gffzwfyej.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gglxxrfce.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gajaefjlk.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/goqmtulpx.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gahfienjc.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/ggnetgtqd.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzxnmbzfu.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gsbaoesbn.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gfwikniaa.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gvahunufv.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/geedmsdof.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gxwadfask.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gdrbbuwdx.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gkvskhvfq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gcqssxlsx.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gxdyqmdcc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gonanajkw.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gornhqrwq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfneneofj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gamhhakpk.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/guzltkydn.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gzoztlxxs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/geceenvgg.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gvbpwnwey.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/giphtvqoy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/ghgtptmpv.sHtML


<!-- 参考信息 -->