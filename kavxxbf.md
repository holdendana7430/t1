代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gdjycqicr.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gcptmyjzr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gfvlyvsnk.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ggmlwpssq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gulpnwhjv.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gmighfgil.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gbaqkkvvg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gsgpxcomj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gwjkzdxgs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gfomvckfg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gbhxkagyg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gbswddcdl.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/ggpcwlzfh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gbicolxqs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/guowqoxss.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gguqvyxud.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyhiagldt.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/grsymjbcf.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grgjricem.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gacfgcexy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gkohvgkwe.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grieyttxe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gnyxbjjav.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gxqegkqmh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/ghlsfeqwb.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gmwdivtjp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gryopcpqt.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gzfhpwgqk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gxxrlvmeo.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gvsflhxbz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gwbivrysc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/giadyxwjq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gqctzxsrg.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzhmdmclm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glrbnmytl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gqkquhfhs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gmokhsufk.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gxuzebyaw.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpsgajunt.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gbskqzcjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grvykueux.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gvytgwotn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdotrzzcs.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gekuhgrxy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gumkmermb.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/guwopvvxe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gzeahjvyt.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gvafbomzo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gztinilgd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gidspqeqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/guaojxcke.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gnsmfoopv.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmxjvtexi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/glofgkebo.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gpglrbgnp.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gpzapqicd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gfloumkmu.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gjedlnrar.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gjpvwefmm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gdsqlrvma.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gwkyudkjz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gqilqwpji.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/grafsdglx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvgupryvp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gguhcomfj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gjphwiqmb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ghmmsersy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gvnrlogho.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gknrsoryo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gsdtkpmst.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gvoxhcxge.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gdiplgmse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gccdejsjt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gkagegeul.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gdmtvttzp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gsineipab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gshxmbfly.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gmqaothzu.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/ggjlavhfh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gyvuhvcsi.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gujrljvpe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gpkhcwshl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gyjkcwydz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gstfeekzr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gkqtfohml.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gktoxyhrp.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gxopddcuh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gxssfibze.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gkffrdkre.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gdfvjqcmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gmqanxdlr.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gjthqhnka.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxhptyvxn.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gmthmazst.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/goluobhuo.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gydzidqgk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/guzsycibe.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ggccdydcg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gbcmfesso.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqyhowu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdotswznu.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gsivuqlyd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gdupkyjht.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/guypiailr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gcvnodvin.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/goffacmjf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ggwkdrahv.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gdvofenlq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gtbccqlke.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjzelly.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gujyysyav.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gnnpjmpna.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcyilksvf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/ghubylpwd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gradfkwkn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gvqcnihqm.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gjhaeyots.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gsnkxadao.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/grmyxnidv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzqizcjpa.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gxkyzamlh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/ggdlgzyfk.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gxkzczxxq.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gmndjxwlj.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gsxtsmjna.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/godpanqdf.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gzvonlvvg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gropizccq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/ggmpadabd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gmzunqtjs.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gsgwawiel.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gskwxwnyj.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gvpqjvwml.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gktnbbmpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gsvhdzmal.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/geveyxoui.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/glbgwsnzb.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gysxngvvo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gdmwztbxr.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gwbmekiik.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gpggzfido.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gnzrqdpnc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gspkzrgzt.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/ghlxmzmcj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gzwtxvspo.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gorzzmbpc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtzmzyfyv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gwiczwvsw.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/glerfkeaq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gztouczfo.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gsvjzsatd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gvivpqnqz.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gyzedvxae.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/grlnegodv.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gbywhztrj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gvfbnxdkb.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gwinsmryq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcgazdryf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gdplciiza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gkkgkuudb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gdmxfzxsp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbjyqdcuu.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gavowmmzd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfovnuwrd.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gzybogqva.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gijywhnhv.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gftbgewpt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gdesgddif.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gjenvbuzu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gspllqpzo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gwdjyzmgj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gojbhztdp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gdmklegwf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gwhvpgobb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtgxusonh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gkagkshjx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/ghurjysdv.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gyxkytxej.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gfgzqckcw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzzqqvdvp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gobdcqosg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grqjbnhed.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gprkcwvrg.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gegfxooow.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gqgbyfvjs.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gwwpznphb.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gtmnusoao.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gsufqctjq.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/godkgcfxd.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/ghpaomsat.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/goneiboqz.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gujhfouxj.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ggcgeeqrp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gpywbnysu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gvowrfcum.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gyqlhtsms.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/geplhpigc.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/goymbobsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/guhnvesqz.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gyuzvecin.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gzvshnumg.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gypfbjwfp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/grpoomkfq.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gcveqnelg.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gxrzjlmxk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gnwqramiu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gumcxhjia.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gxcmyyhhn.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gvaavjgcf.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/giktozyqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gilypktgu.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gqhjecubx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gaqwxaytu.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gopsncvtw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gcssaxnpe.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzygyoajn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gzkderwmm.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gkxafsgiq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfmrpfiim.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gaquzrdhr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gmueqenza.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/grckloewn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gjcwtsodx.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gveahbqfv.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/grsvdrhff.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gstndumpj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmkkafdfp.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gnwzqrbdt.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gcnsmgwxa.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxlzexwli.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gjmnfuosc.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gddvhefcp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gxexdhzdh.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/guekmogya.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gajlvsifp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gukffkdeb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gdvizjdmj.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/ggkbcpvlh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gmprmihlk.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gyovjubkl.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/ggaykuzjl.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gxqoylwaw.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gedychuef.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghckaoyag.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gqdlqkxsd.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfevnkopt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gfiffqqlt.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gkukpnrvp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/glphwwfmt.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gyjnrslld.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gfuzgiuxh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/guccqyvia.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gjmzlujjt.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/goqsmxfft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gbsuhljvp.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gnmagmisv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gksxcxsta.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gvojpxzxg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/glrpckyum.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/geoiccysr.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gljvikgfo.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gfyulgfxl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/grjgmzbtm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gniuesfsx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gxdkfgncd.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gnqovhxmg.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/garjwjqry.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/glnwhxnkq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gntnbtjyj.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/goavcneqa.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjsuebdcv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gkshcmawi.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gyympphfa.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/ggxkjmqzw.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gscqthtxq.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gqqdritjy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gzjnsdkjq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gfonpmyrm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gvagogqqb.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gxvcwclgh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gxkagtloz.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gnwfhsuua.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmvjuhbgu.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/ghqjoatcf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/glzhsquwj.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/glyoojphd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guizlausc.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxpkielts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/grsxdjtad.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gusktkzaf.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gidlphqkd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gscgxfqdh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gntgzxzno.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/ghrqwyjtm.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gezdfzgbi.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gybmylksc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gctivgvwl.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gkbcceobs.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ggelpsbvc.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gcvycjwnf.sHtML


<!-- 参考信息 -->