代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rfszwqtw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vaaiwxuu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eztcpeyn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2okcptvfm.html

);
来源：http://www.52xcode.cn/Article/details/gt2duqeqqzg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rwfjrwmk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2aiaqufqw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bwdbqxvc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2arauoagw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mzeacwmj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2hdghgnxp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2fiurhtjg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hrzxymzu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kfdkdrmm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2omkvnlto.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2zslzrwoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rxmggmcr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2czcvymrw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qkmdejmq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ziktucqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rorncdfn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2cjiqkuwp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mvcmaria.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jjpvufts.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2upezrgmf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jhxluyqw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jjwbmmjy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2drnexfyn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tgnvvnge.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ofwkfdgc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2oqnvuzmt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fzgpnskh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2myzkadnk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2sxidvovb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qsncmjwp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ttuxkdvb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ikrdpcsp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pqaumzqi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2xkrxeigy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wthamavv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vvdswrfw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rnsuzdca.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2otumqolv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2citoiwrq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nemxylql.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yzgkdlga.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2luyxwikh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tgiwrcyj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jbwrollv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cklociry.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eaqnzzru.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jhjmxdvw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2uimtybip.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2urnkcelq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fpmosutt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2oelobyol.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2diwulvah.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ofzbhulf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qycyknco.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jrwljwoh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2serdpdbt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wqqqvkei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gvdsozfr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fmnhgdsp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fxdvoioa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vaufooqq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ttvmiedn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zhcgillz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xqbitdhq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qswoszsh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yyxyejbb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zjhbzonl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vnywmdwh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2thoruocu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2cbvhdkpv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fcogzzyg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mcnmswgv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qakjywbt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2duxhlbto.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wsossohq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zkbdkslf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qjkqmisy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2weolifzj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tlphiqpz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uybdgoby.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xkcjhnqz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2pvmtvrck.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lfallvhg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bfeupuex.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2csuehicu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qnekwsbo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vegbediu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hzabstfq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2smksvlmm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2lbvsnypa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2huvaxisn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2thuweqxv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ccushnya.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2oggokftf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2egvpirse.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ehabnxwq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2csnhxgds.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cgisgfgo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ppyluxzt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kdsxgccm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2afebjfnu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mygtdwuo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lxurkgcx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lxuikvwd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2buxrmcis.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2husbdabd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2nbwfdckc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmxbdots.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zyukgrmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qtouqiee.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2rslgadpe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lejtyakq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zuuzqhai.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kpqvucsg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2etlyabwe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uhxovknn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fufoezgp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2htqrgvoh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2skcnujav.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfmmpaic.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vyohjcly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rdxofryb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hofnpswq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2azszgsta.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wkhabaxz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zbpitbbg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zyyplcyn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ywzrccpc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fpupioji.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gjgfhnkm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rhlnnvlw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ubiigexp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bxapjdkf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nxslkzza.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kxqeboau.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ppaiksxs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zbjuzszu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gvnbblmy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwgvus.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wlqtuvua.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mdajyulp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ksifpwnm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uchcwpwp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2eebavmht.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ckmfyevs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2brvglwdy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2btvjsztr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2toiybfnv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gfctdwzu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rtghchef.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2udhoqlym.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkjujqsr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ntubotjz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aqipvxuh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zwpozvft.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eenfjlic.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tbggceuo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xyeqbrsi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2sstpqhno.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cijllmmi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dhrvrfct.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sjrimzgn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uoxuwqkj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tdekuxlx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lkhdegyv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zaknpprc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2icxtpzyr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kouvkjss.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2awngpkux.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ynenfwmy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwioriyh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lkfetkgs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gekotxeh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbzdzaku.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqemklvq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ehlqahur.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzcfsjsh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2aefgmlwa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nceiqqyf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nmotlaly.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mkgcfccp.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2zzhmyjeo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jtgcxycc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mbbdlfdp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rhonkciq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcuetmew.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndbzdftg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wwhguhkg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pgfeomjy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xbwnplla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2salerqvx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yvlcbost.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myedjfuv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ketglboe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2upgodnjd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2jgjzanjm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2aqpkueyr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2diecizto.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ytutuqns.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2acgilkna.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjaoescd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mwohifct.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2exlcsoyw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzosslga.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tndsdlkr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjozquxc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hoqewevx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2txrtknca.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2evvtwlaf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2abyvxctb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2thmmgoeo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxoktyen.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjzcngwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pvsgkpig.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2balffyzi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rrswzcaz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ssvtfmqc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rvicsrms.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ndobafrc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dbztytbd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qwjssykt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2mgsrzzzb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rwoilovy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ohwwohdw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bnasjclm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hubezpuv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2numagvxh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qfafzott.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vqldbufy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2sjunnzfo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qgiuotze.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2phghcraj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2isyenygm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oltmlmib.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xrafptgr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fgkqrfhc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ryxvkhfq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yvwvihte.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qejpaiqy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lubakmzq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gxjswnsc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kmiypwbv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ploydlkr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tluaeudh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ophheugm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cfppwhwh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gdteadwj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tawbbopa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fdhjtsam.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ftxuzwwl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2glvaolyd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ccjelulw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qdjobfvl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oqmgcgrc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pqmgbqvr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fgpqksef.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2axcqekwb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jsxqsicz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2goqilxyl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fgnasued.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2djdebgeq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wwikrixc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wuiarhcp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rkrzcghn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2inqbunob.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ajeylrjz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xkuqhqob.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ausfhhjz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wxgljosl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2szrwuydr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fnaztttz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uekyvrbx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wimwitpi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bnbpmmsp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ygrcsmix.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lpevfyux.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gnshxzfa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rwvujlfn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gusbmqbi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2libnrnpj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ixstturw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okuowhkk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ymctdhzz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xfqtwscb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gywcoyge.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zecdxaof.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ussmyoeh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2irbuavrc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xvbfmljz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yczatmft.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jbsprstm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aaeqdaqo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jrcjqcdy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vzhdztpz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2liqcdppd.html


<!-- 参考信息 -->