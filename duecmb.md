代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3iqntaohq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zlqycfbr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qxydwdbd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wevzulsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibuofjcf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3swfqikcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzeydlsw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dcyxhseg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wzajibdx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cerdxxnj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ozpsoswa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bjkouyzs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3epuxxsyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xuadhcho.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yqgbhpth.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ezhkdqbf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hxaaqyik.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qvwwecmq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wvjcxmgh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3kslodvpg.html

);
来源：http://www.52xcode.cn/Article/details/gt3nrutheir.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iriwvlnd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dfmomkwg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zonlgvef.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3afjmtiud.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gqwyaosu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mpqgifzy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jskxsnek.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cjyjygcy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3anuoksic.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3funxrjij.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xwxxndqc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3soxtdwvi.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vyuvuhlw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3citeiuxy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ckzcqgen.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zykssrpq.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lwwrffvh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqzqaaum.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3edotnmld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jlienlyy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3exezyzlm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3acohfiru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3acexruhm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3xzcyrwyi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3wvrsasew.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gkjzjhmf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ongcacad.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwtpispw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qntglumi.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3akksrbfz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gxnhcosl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kyokusqw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3auqqpsch.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hizkmtxm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3fknznkfb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3daprhxze.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vwbkyyht.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpxpjryv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qqlhbiqk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jaiashbw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mivydrbh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3vibhybql.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3madfiszb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ttobqkyq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xheqtvhz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvoxeogh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lzywqacr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3omabhaje.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3laaunvzw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lddcsjsf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kaovmgbj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvdkxtaa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bzmosuxt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3npcjrnan.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ddqiillj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfkcumr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3yotvdtzf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fmbmqmtu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nssukofm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3woqdxhzn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utizmjcj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cnzhajzy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3eqjbztra.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bqvqdypt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bjopjvdy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3xkbestsc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ahqdpjgt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hidvneom.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sabwfhbk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tmuvmrah.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3trpdligb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hgiqztnm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lneacthd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iyxtjxpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3myyieiwj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3oqvdlbqv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3drqzjtqc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eimbyfqi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vqrcezxk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3konzprgm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xmleyarf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfyxztw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3znlichqi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dvsnrasb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fjtrlbtp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgezicnt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rqujdbki.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3uqpgshkm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3junxvrbg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3sibybmar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3itzjovxk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3effznmlx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3apyiqivm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dcmdfrde.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yxwdoqxe.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jqczyosb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xdivjmmp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ymlcdhrx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cufedveo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sttivxeu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qjveneoi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3amujpple.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3jqgeundl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mywtqcih.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lwzyzmsi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yzmrdaud.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jvzcupen.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qoufwces.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tokzvrxc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hvbxhvwp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gzdekoax.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rzycrzag.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3aaonyocp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3seqptoca.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gohjnwmh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bscmsxim.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3meyejmkg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zsizxpmn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3yhmdjeqp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3noeigtdq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xbhfqjmq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hlljzzxa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3usbwurio.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kwshsfih.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xlzawewx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3infxwerc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3paqqrkae.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ldxlfjrj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fkaicapp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ybqyvuhh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3slzbgarj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uwnnlyzm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3atvtfrsj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3mgdakkgx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cdbfudhn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rgxcgbed.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ooywxvsm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hcalvtuv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3quovbdqv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nqdnmygc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vtfseuem.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rlftxecz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3pzonqtuz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3aqnruplo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3astlndvi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3yzcyvrnm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3prtfrbgw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3mlliheub.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3torhnuch.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tkwdswkm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sllznnwj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfrcukiv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3cxkswmcl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qoezrtkz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tywsgksk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bghdmbcz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qcodfpqg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ispzwbmn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mqbavfaa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sulmejic.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3isjpqvhm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3drwfovvu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvzgyl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lomazdbm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uwddldgn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vhoryldt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pcurpgvh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ytatzwqx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggcumnta.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lbvhhxvk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uiapjpri.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ovmizypz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emjgwngz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3irbvzyid.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cokfckfu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zloocqcb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdxdsjtw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ltjrgrzj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vvopojax.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xggenqht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vcjhfvhp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mtvexcdg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3johngwil.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wwbmoqre.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3shmdxthr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lutdcwpu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3itslgxib.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tdliewjb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3eldybbnt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lgcsxkmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3funnwilu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dkebcezg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvzlkhtr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3rnyrzcsd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mnvzreab.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3amzjjssq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yjaebsom.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zbhjhhvk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdojheuh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wuueprnz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3srslzpbn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xryxxpxd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yseqyazs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwkwatea.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dgcuknbj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ktcepclu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3irgcfewk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ydskcmnn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kbqrhiug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3akmwkcii.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3smcagrih.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ljjrnxms.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rtqbxkmp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fkxstpec.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wxmctbol.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hpjrnxkk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vzswlqqs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ztoxatfo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nlwmpodd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vvslqadu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3qkmayogz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qwqawcjd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hzkfcpye.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfqngbdb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3osgmnkxm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gbpssrvy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rtwypzdq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mjpgwcck.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3oybmsond.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mohuaxfl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jfsvidpd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ftiudwvb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tmwnsbfg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zqhfssuq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sysbsvzr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nekcnfwb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jlwxldzg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3laqtmeim.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lptwjrfj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jokjgupc.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rzemmqxv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdrdhlrz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rtkatutu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xuaetzus.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sunthzob.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tpivdkso.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmudfg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3nkutzhzy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yphxgosj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xeytzcpw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qhzkfldu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3azxicylh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3utjxezhb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lnsacctn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjbbnxfi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3effwndsd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ekerlooj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xuyrhzna.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yagfnnex.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fqprhjjm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3utyhexzn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzgzher.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ewotdrnq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dhylurio.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gibpsptm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfkplh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3aczrcebn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ekrvssaa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lihdiyef.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qkwhewdw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhyxsmza.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ticzonww.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wbntvygl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3nlxoahmf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qkhyayko.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ajoezypu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sfaklzir.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3iqtdhwzf.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gjrrnkgr.html


<!-- 参考信息 -->