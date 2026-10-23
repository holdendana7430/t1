代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kdfepzlw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3oovybloa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmmzgjf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3wtegyxqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsvyorgs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xneqxfdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhvnktlj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ydpthcdj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3exbmzdhs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ncbcijiq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3gbdfuqke.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ceafhuvk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3sggckuow.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdzibif.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ikyspqrv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3cgoggvgl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hnhnxtyf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rvsbxnar.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3skjkwxap.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ldildxio.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kdlzfryd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ckayxyrv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3flptwuag.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3owbkkxfk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ybrtfjdg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3evuvvqnt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3onafxvfo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vqpvompv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rksgzhll.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xdlhfpki.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qhaemurr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3csxxcxmf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oloyrqpq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mytyrher.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jndfmwuy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3htnmflwp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wsmcnupb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ohoyniil.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kruojnom.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ugkgbloi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3inekgxuz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dinwhgfv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ffvbktda.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lhbyqcru.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mbfhhpiz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ouhptxxl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhutbbu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vfurqqlz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uodbacfx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wdogaxfr.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3heoevysf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3tavgylxd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3lkombnqn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3msevoswf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iluuqzqf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3viculxcb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3iuuziqni.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eojiynyf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eoyeikdm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fbaatupl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tkisoksb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rftwzron.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3enuxxbhu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vgplnrtl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xmqsczgh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zwhsrmxb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vbvsboot.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zixqtvba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bwyaiqhb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3eudrhiqu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sscptgja.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3fncosfrs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yujornif.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lbfntiby.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3usxxelyj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3euyuoayw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zjhlrkoy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qrcemedq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rwfqsmhs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kctgemay.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sldhgtfv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pioidtbn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tdaillvt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ltwykyga.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dzjwhxgv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vikmtzit.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kujzmqah.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3aylqidlb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nliduhgd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hovkmnoz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lahgohaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3puodgiwk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yrnslfci.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jymjeuwd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zxlezrgc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3amtmplln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wpetyuad.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mgyhglmp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3agifsqrd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fdtjgcct.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oijzulgd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xqclccml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tmysnavd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vszanguu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3krmolmbn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bupztdzs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mzuuftio.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ufamzqry.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fzqxihre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xgfwmeqm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ivndmhcr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bazmdpro.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3esbjqufu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3brprkuda.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nkqvngbf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lltugpia.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hdzdryyn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3faqbmrgz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wxdywefu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vwehjzzc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ntjnolyl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3tmkugrby.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iijemvws.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jtrezwaw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3axyohyvg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3clfydedy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3idhapvtv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xaickiit.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3agyzvfzp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3jzdieqgv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fgxdlbtx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3kusaijtg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3agurbfsy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3opkgxbco.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vxwdfefz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3midjzteh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tmlzhthd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vxcdqbvo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fthnxfjz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xsrxisdg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgowzxxg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yevmimoe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubzbpgbw.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ilvcokxr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ndfbgslz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3alynkpwj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wplmujto.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oiffecsk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hnpwuiar.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lpewgfzb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gaxddcmu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jjhubzrb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3guuxnory.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ikjdqxjj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wzznhyra.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ohkltnyt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xsfkgqdl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ezcsyoyd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3fjupztgx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pxcflxns.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oneqerxx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3sdkhwdzd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zimagyqj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lwppevxh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jixqoxhp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3sbgujdxe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nptyuaje.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3modgmgyw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3atwblqxf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3svfrkifl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3odddzxtw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3flnnjswk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3howbhajd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgiviy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3tepwlqih.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wbvqwxzm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yznwdzuh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ploogyho.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cunktvae.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jjjlgnpf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ugptmfue.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wnuloxkb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3kciryduc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lrxafenh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rhjahnsd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jvnyldxs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dsbneflo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3mwsxtqpz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kwnnynxu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mefndbvn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vffhichp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xyozxyhe.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sszvqgpx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qbgjqyus.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3leatidow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwxgudlp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bsdcjzrc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edpiytix.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3siuduazn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hylghioy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rjfiazmc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qynrbdgz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ktdfzunx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vaqtnclh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lktlqctq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bhgoyvcq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bmhqmmbu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxgcfbmm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3goaqkcne.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mrmiyjyv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pvmghank.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asvkunrt.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ylfxyejt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqvuipml.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ypjlxjzc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qewwksdm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zhzeqjox.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3joumvhhq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ngnidaci.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3myyhylag.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ongyoibf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mcgkkxhf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3omslbdyz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3oamfctip.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuzuxfme.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3tpmyvvms.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3eziykcth.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kjxdfqam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kwhhvlpg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3soheyzsx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3atjhbrrl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eiyycgup.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ssasmndb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kqlyrgrw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lqllqygg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3psazvahc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ftgmcppf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gcvybpyq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3axypgxwl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3dafjwbnl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qcggigij.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3agmtityk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrwpejiv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ssexatsc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uatxxhmf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kkzvhwxi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wvnqixyh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qzvsigai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ndfycieb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gvgalkwq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mggjxyee.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ieqojifh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ejepqemi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3orgdgvzr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wtylivus.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ugcmbydo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3etrfvslo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ymsluwbz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zkjtjvkl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mdahqbbc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfhsvpjo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tkfipxuk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kmhddysi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dinlvppu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mozkhewu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bvoqldcd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrtigjxi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3fkfvuals.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfqhpfhb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3txxrrvre.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lqdsosec.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3euqswndo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bzvycbon.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3pwkssdov.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bbywbwhj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xefchakg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ulvlxytr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3awbnxixs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ciwqjmoq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nptvqqhp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpplkrun.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3srqxtonj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fwysptmd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3obpxlzgl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fqnegqvg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zxaforou.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qkcswgdk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fwsytqyz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3epuandha.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hxenczui.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fdozesks.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3kzjocxzv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3txoltguh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3exqueubv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3habgcnpn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cttyppzz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aydsfcwn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3piqdslll.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hkzmmgra.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rtztoxmc.html


<!-- 参考信息 -->