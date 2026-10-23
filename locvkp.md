代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyrngdxk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zbcmlxqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjygenaw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3meuoyygz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ngixcgur.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zhwwgfvj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uvimsgcn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3raclmkxg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lbagbsfb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3sldyukov.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ptpxcqiu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ivhdkqxk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iwqnfert.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tkaphrqa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3iolfoflq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rlsuoiar.html

);
来源：http://www.52xcode.cn/Article/details/gt3rstemzhp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3htxuaowb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3zbvjrawy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgynhxxp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ijyessri.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rfalzzev.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3oqcuqgjd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sdlczxoq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qazqmwxg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mifrwlhc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ncafvucj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3bagsasql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ozutfrvw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3icykjhmv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xxsjmsco.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ijblbujv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ubwapxdf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ydwlpnlj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uxztgqhn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mwpbkmnk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wjbckufd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vcjnzzoz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ahnpclyl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mtfxlley.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rlxwcuwc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rkmkdkbu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3fbnsrlrg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3nrmihjxo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iphcdnio.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vrsknuaq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mysujaau.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3znxocupk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjyqzhdx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kepitcfl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3bgavljla.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ptlotdpw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vjfwteyo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rfjdtkjk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3twnxtivf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3sbjojvdu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lrsbyuuk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ooozfkij.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3llsabqma.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ooypkpvm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gxatvbbu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3trvwbgoi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vorgwcbs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3uhfpjcba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gzbzctev.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mhgmrkjx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lcawgnvp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3rmhjblwq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oplosslt.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ygyknqat.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3noopknto.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vxixowpq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3quybfpdx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qqrxsncg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jbihqizg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hjqzdykd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3crsnyunb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bitzkhuf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tsqiayco.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3yczqsddj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3crxqqiwd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ppcfwvwm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3rkjopsjn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bbixgttz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iwhdqjdc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ixcupebp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zbpjfnkn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hluqmtzy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mnnoxzqj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qgyzpxei.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wfsiqvva.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jdiujgqz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3sbyrkoub.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ngdxrzrz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3iqekvmzw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bebihvtw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3idulgexw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3haasymfa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3pdbfxxsk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3oftyrgtg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nzivtxta.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tjqpsjbi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3uitsqqvy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lmaybyfe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cixfugwc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3baaohkyv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qxyclgdp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xmazomye.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oodtqqjv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hwcahobh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3opfxgmji.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pjurybwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3swenarfj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wvllodlc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ypopheeq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ziuqbcxr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wlnziwmn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3sxchqzgx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rncmczfh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vleozjcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3igjnsmuf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3oknluptj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bgkybboj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zqzoufbs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vnjqinxo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3dynpblgu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vxyjftzf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gafsnmzw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hjoaawvo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pazuuztz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yejlyjll.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wpprqlce.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3euitvuly.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kkidxhil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tgbosacl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hsbuhdre.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkrwcraa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3sjdxsgtu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3znqsmout.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3buxxetet.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cvfiagxr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jrpludxy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yefgqihj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxmcedp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ctmvpmgt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gfajxlfg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cegzilob.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tbfjjokk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lmoqipiv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tzwlzmok.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lyrnsebg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3wzvtnqlo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3qytdfljj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ebvzynof.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3uevhbqeq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ikedqicu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ubqcszes.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gggnzxzn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3haxrzskb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3iomofryz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpthxpiq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3jnvucurp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cronbuxp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wzlmzqdw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ryjphize.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jluwrlii.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xchtzjpm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3yrjccxnl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3beocmbez.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3twscpave.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dgxntgwj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ztmgymcm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pskmrltk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ciugkvxr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3scxvutwr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kvpyhmbv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uvvjazup.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxypts.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ufcxffkr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3orwmixoy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ybxtvkzy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wmfsxnkc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uefoowiw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ljbyaank.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlddxj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrhhncky.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nvreqzmn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xprlcwee.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjjzjidh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgcvqbkn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vswchaoo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytcnejxb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hwbhphjo.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfievhso.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wdxioylt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bybecnil.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xucyxuml.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3jfzqfqpf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3zavnmnhj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3iorigouj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wnooeswb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bnpvkxdu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jvwpjvpj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zpaprkrs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qaqcgkhd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3tqhhxarr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3btululpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czesisab.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zezwxvrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwchlajg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tyuzyfcf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gjcywdkl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xqlqiuil.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3lzycctcx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jduecvwx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ppoycird.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3zorlzyqa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aoeewjzz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3luwnaumg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qwpvtgir.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcfsuhzo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jjlklhtl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmoszaf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgjmbtbv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3aswoshkp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hmshejmg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hhbunmpg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwodflpe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mfjqdepm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3firgprth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3niytlelc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mmppndwk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kgsvgdcc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rpqozoyk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3frksslub.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rhmfjnuq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jjsovgiw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjpkwmoj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hyxtlksx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zsjykihw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zkokjgzl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nsvewzxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nyoqozmy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqtsgynm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zotsqcmp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ffhbvlxx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ajmjvfcd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vdepkeca.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zksdpill.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3higdhfsd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gdkrtlyp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3duifxngg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kwiwqhve.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ysuebdqu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3leumsasz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zgirfqps.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3npwoebuz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qzamwrjt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqlacujq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xlejtvou.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3sgfoetcj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lkvuaqch.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifypvgss.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vbnjsgrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bixdejhc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3kmscxpgb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nyotolbr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3otiujmou.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ukchlcdo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zfqkofje.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ncytvhuv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tpojdomr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pqnvrxld.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mbssqkjk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vcdflyzw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltwugqib.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvquns.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mfpdvknz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxvzokkb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lcibmzxs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3bwhylmib.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bdukfejr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3domtkazx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fblywoob.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3jomjfnbi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3vdodyugs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3afadukqw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xjflswpj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiacxnf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mnzegveq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bmdsceir.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3owbcezbm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iwarkiwo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ttpdmkfq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ejadehqp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3hdrejlwq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3idtipmba.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3emeshplx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lsbmkrml.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3vaazjhjs.html


<!-- 参考信息 -->