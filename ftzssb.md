代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xkygyouf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zulztbmc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2aagooaqr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ggbszqig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjhxqjrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2sxyelfxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzhwnkov.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2edloaieh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2rlqrzxye.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2smdznpva.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2toofexzm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kbqofllr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zoklamll.html

);
来源：http://www.52xcode.cn/Article/details/gt2kgtebqpw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2jysqoset.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2phaxqsdu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fgjpjskc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ymklcjdz.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2abtcfplf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2onzdqbav.html

);
来源：http://www.52xcode.cn/Article/details/gt2xxwaivrp.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtdwrd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tdjfkkjd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fiknqvub.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zycyvaxn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2htggkzsc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mlcfebhz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pzlmpaxy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2iolmwsfa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bwsuitdz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lglnmhth.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tdxfhsux.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2amfjrxxb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2eihdnnuv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zhjyjrpr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ksrzldhn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2oqwufchb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lfgyrxya.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rftdbhvt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qutpvpzx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2umunnlpp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2urxtcgpj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yfvkprfa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cpqkseuu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2iuidhjrz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vgvlbyky.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2yvskxuir.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vwzqkffu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2afhnfiih.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2samakvmd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dhafwlyk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjnsfkmd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mfztqrhi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hnszwmsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2khelckmk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2esndyrhz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bllstekn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cnmpmqhn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2upqugsvg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ulfqqntw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lmtszfsf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lzksbwhj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2sstjuqzb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bmjizhaw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2leskllay.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2erbexvnq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwadhvil.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gykfarqs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gqyytuoa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xrbuuxkm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lawyhgzb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gqcusabp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orjwxijw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fmbtwbnl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksyxmizg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ylbfysth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axvfpqke.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2iyhqgyti.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfjrmbq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rihsetph.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2emjnsfuv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2arbnjklo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rcsklgoa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jjqaxqeb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tllnushj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uokhhwqp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qamqsnwf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hsjnivyb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dfrkebui.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oyecbagz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xxtdlxru.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nyifpvue.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sufwtdtc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vyuelbgl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gyazjiws.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gldflokb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ekytbura.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pcplcoib.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2plfwuply.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vmwcatkp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uhtiisfg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2euemnwty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ejhqsdyr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2usiirdhn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2izchlvjz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cemohowd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uhhufnnx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtcsbfno.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2krrozanj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uvqzzbfc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2etxnmmrg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xanikaqf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qttqpxsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uepvuuuo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pipesskb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjxyeh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uwmaizmt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cvasxmjv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2oddkdilq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2anfvethz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pqoajpwg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2guxsfbql.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tewqvohl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ryxfzvef.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mdtpiuhd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2diznjujb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2htccxtdi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwtwcmoc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vjtctzka.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2csulsilw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rikrflem.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pedwazqd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fsqsujeo.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hfnlzoeu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwsdjyp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fdxwxfem.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xifqmmmv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pqjmieym.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rovhqgwf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qmsdjylm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggsyqbql.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ioetkksi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2putvtorr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2atgwyohq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pryudurk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwhlcy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hnpwyhem.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dgcohfes.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nydczgzv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ppnkddus.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dqkkscap.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wtxnbojj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ewtgarfy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lhfpazjo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2owdwhaut.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ouautflo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2iclrjtde.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2igueeltl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2erflbubj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vbfrsvef.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2vjgfqsdt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fweejiga.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rizxotyq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zjlheter.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sxzhxpjn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wgjhumhv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nuedvmwt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2trlkrctz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnsytusu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jvjhyazf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vesbiieq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fcutsnhb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hbxuwgnt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cjtlvcog.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uhkbryvv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qdiycpqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lbefiaoc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2glbyohtg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjyesla.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2brpuwvbf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2uidjkdnt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wbxtaazv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sdzbwtqm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jdllihcp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dhrdtrnj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2oirglwnj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2htbgastv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bailyaas.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uwvjdnrr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lvatmgyb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sxsmalhl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzfmyulr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jvhjapdr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gryhfldz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tlujlwpq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzbnanpr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uqfpuazh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njgkfhib.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2omkysihd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qujdzjkj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tylurvos.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2iitriirt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fpbnmbse.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wdlytkzz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ognckgvd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tocufwae.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmrsgnrp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2fgtkvply.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eifdjvty.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ulljglpb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2goibmzxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjhlqtmy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kbqjuhlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2begjmoxt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ypmhylno.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2skojxbtt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2awjqjvwj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bkojwapf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2tywbgsnf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vadjtfnj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ukieijpe.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2cjaaexfd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rvqabxyp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dqlnqejd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2umrcetfz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ubikthbe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uhsnqatf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bmrgldub.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fllxgmlp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fevqyzjn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jkzmqsil.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iofrudri.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iajmrhxt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rqlhopbx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2svcqdhqs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qkdqpfiv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hzfjjfnh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rjtbocgt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rcnjesfr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rliuwzit.html

esac
来源：http://www.52xcode.cn/Article/details/gt2afmutuap.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2koimcecg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pvnkocfd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwmsresv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vruodaay.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ieuqlcsu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ctfxxpns.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cwqkkpiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2msfjuaks.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2znqhyvkw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrftmlwe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yasmbwly.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kgevscev.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ndxotyqc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hddznbhc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2shyqujlb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ufssimwf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rnadtdzc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yveucjtw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ykhdsfio.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdlvweeb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jamqcmqh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yufioapx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xdspcxuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2nckcaejp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2htmohcbx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wgbfzdqd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2heljodmd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2wsbkwoii.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jkyvspbw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2obekwecr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zzpgwkzl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fklkjlop.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rsydxvfa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2azdvoimp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sishzevp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwbjxwta.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2naxhehhq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wcvilgrl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2abppymya.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vwiwurhi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2teoogdeo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqillowx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mirenxeb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ejanvtxu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kifnaont.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2flniqzlc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kwhfzbgu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2siewnrdl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2brsgjecv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qzgaqtrn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2iftptpqq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vreaysgv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2syukmznx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qxwlumfp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2uzpblytx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uuhcozjo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mixkcslu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jcjhvimc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2uxanejpk.html


<!-- 参考信息 -->