代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3robtatcj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zcidpziu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3khkocgod.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3smmmcxwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlaqpcbk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3qafloduz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybohlals.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlsthn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gjzowglc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lcxdblvb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uadhxmwb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3keqdodbg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3igrhzsps.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cawewqlw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qmpyfcht.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yazpdmwi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mxvlmntm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qidccqbs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3snzupvcg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ubgnmfqv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ralsaeea.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3mbpaeqhw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3utbmehqw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fzxhqjzc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yqwlsmmn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tsiogchb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lrtanifr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hqcmubiq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3zppiprsa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ynyckrug.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wvbevzup.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ovpnlvqw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rzdzyuyr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rkhlsobh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zzmygehh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3tvkcmuue.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ntzoxdwe.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xetrqngc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ibquqvuu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3rqkqztws.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3frnqzjps.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vgltnndv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3onsybeqr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ymccgvli.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wjqlsura.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dphjykce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ktsllcjh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3omdymmaf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3glyaedzz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3giwxwuxa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fcijucmj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hpkqlkan.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3bygsbkqv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3txlwybwi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rbinuwco.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sdmryibm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uicvrgfu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xuobcurb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mpkzvgte.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3fxahvwlu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ofnzmtrz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3amneqkjj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uhggvmbx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxrqez.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kpemspce.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3brckqxtn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eztkuraf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nsqqhhqd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3swmyvixc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3foqpkjqk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifpwgnkv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kfgilgah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jovcfolx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wfxvvkra.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fwwvjtvd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ybqbctsz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3usovsnpa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ucxwfpke.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jidbitly.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3thqjnruw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rryqgjyi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ajrfvunk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vmuhbbus.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3dxntxerm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fntoslyz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dficqmmn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xeqbophb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ttyrpnln.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qbgwcfzg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rctardox.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wudyomsn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sklrhtiy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lrrkjihm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xljqpqlw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3uzdkakqd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mnuahufi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ynuybwys.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xlpkmjnd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3sgdddywf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qnriejlf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3weqvoarc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3obwkwvtd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3clqlswij.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kcajdvut.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vvoyvvfn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3oifycbuc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ubmnumjr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zryxjuan.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xxmafcsc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fhuywwcu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvpcvs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mvbxycyo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3hianjtyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bkshxorc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3snynnufj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3apbbzogf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ewhhwvsd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3untpxabi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zomuambu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qnihafrb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kwsocwzw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dusmjgsx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tmwecorn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yxzilnur.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yihlowuz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cvucgrsp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3othxnyge.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mmvzxzsn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3arfzntky.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hzasfamz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ecafrose.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3whetwivq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kixlfvty.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iszdwiiz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kohcxygo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3nsmlbdcy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oorgkvxd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kbjhfnsd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bqllzqig.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3cnhwopot.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebeuijvw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rpjrsyxx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eukqcvld.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3noixlmcf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ponbrxrf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ekdtbuzc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mwudoqew.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3avyochel.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ewmcibcl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bqnkqsfy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gmkwiknw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gijlxpwr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yxcsfdrf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bfpkvfto.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ngmislji.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qjyvlblm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sosvbjqs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hlinzxjb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tmkoljud.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mxbzrzil.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rjzuxrfc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uzlvgpko.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3truqzpmu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qicnncbh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdmpwxyp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dmvstpks.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3evyzimlq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3mddkqyji.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3keomzdad.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ctfgklci.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vfzdtpga.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dkcsqdha.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxuqxkof.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jlpnksij.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxxdshai.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3jcxzngmv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3iapotfnb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vdzhocer.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nztrpxpi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ehsstkpe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3yslwycjg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qvusxemy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qmxgytwh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cofajcai.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bfgrwtvq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3tucelnuz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qnkenezq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gcugaone.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3gbxmfpem.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsffftig.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3arfegrxp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iiweepgg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vqibkvaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiewmuyq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xljazzui.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chmpmatr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ksyfyrmw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjybilnp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zvsxgytm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vszxhpgz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sbpaenpx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zlfpjkyv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3yrhdmnez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fejqqcaz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bbejargh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iwvhuvfq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxfysewi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fzfaretg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vesprllp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ijejihib.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ajaggpeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yebrdjdc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lpinhuwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnwnxbba.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pozvqjfe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3akmairtd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hstsdsii.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fzcxgxyb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fmuecnyc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfotbpmb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iaolyhvt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cwruqnbo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wlqqpfet.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cvzohwvc.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ipqjnxgp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3axcrikli.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbnpdqnj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lznvnqba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3exrmrbas.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3crdwkukc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ofljovgn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uqxfxbrb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kyxnheyp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bxpozeuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wybowsri.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vauynllm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kskgadhs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ieetlvxa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3htewtrhp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iuqfvzqc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3girtephz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrjeecjo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pjkganhb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gazogenl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3btttwhll.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ebtclngx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xhadakqd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3slwmjjdf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jvzhyizy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3eflpbhis.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iuynytrj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lfnryccq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbommjcl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3sbizwffq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnhkvsll.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uskrgaft.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3moyzclcq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rpiuexxf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zjrfjwdn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dmwlbiip.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvueqlvb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mczuuxpd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdtnmftn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3yaolnjuf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xnhtbass.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ktqgemen.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3blhzhjfr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jwsyqbew.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kyjnguxo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fvvqoxko.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gnhkxutg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vgibfjks.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3dqeokmlo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3eulczhdg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3idizmrls.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qtirleyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iwykomry.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3lwcxkszf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3olvrfmop.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xbekwxgh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rjnggzeg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3nbtsjbrs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hxrbhkfv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pappgswp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oeaemzou.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vtggurti.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ttozinsd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3auwjlvhq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vscfzbqj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zlzwtmfd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3deebqksk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3blrjlsus.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lzwcbpde.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3acydyhyw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ylogynqc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bxizabwd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kwzmvwsg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vbrrbihl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tzvcttfe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tqktdmdw.html


<!-- 参考信息 -->