代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jlrsacuv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mahopivb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oyglourm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yrrlswjq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xfvvvlss.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yypkhjdt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gtdzypyv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tkshxfmn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eiwjihfx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2anlpujhs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2kketzohh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mhpjuzbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xewnvoaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bdevywql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgnmzwjs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2snjzvsnl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mmpfvjpw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zjyrpofi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fbemhbxi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fktqoonq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nizbzyhc.html

);
来源：http://www.52xcode.cn/Article/details/gt2pwwffasl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2zeesudgw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2emeolwhr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uwjazpkj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ukutfhii.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oejdtigd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2aismdsxh.html

);
来源：http://www.52xcode.cn/Article/details/gt2ikannuda.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dlqtkqeq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xfaalnqw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2ghigrbli.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2cydimapm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2nkuekbfc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wlgenknt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bsdevqcs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wyezuatb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2njiwkhxd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iejwbccb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mbghmowp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mwcstito.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2fbkwhkzs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ieqhasai.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fsbqgzju.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aiwkwfmg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2tpijoybg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yhnkeaqx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hehrztjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hxzwyilm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2qweioqqe.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2atqecflc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nbrjifdj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ovigkqqr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2amkrmkos.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mvtbrhgj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vronvewt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mfohafhb.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2swdvrphw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ridmqgtn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2accvhqpt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjakwrbf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xhlbvuei.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zqphavse.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2htrhpiqs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vnijimdt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mqqchrtj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2limewjdu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qqecckef.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2pffehdcm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ddlqmrbj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cdgqcsif.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lzurvgaw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kdkjejit.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ebhqebqw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jponbxfe.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cohxyyct.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sxhajthk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2phlmzuzg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2coxfnavc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rnzzlggl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2offbvddd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2uqjdszcc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yoapdqep.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fquqhnwd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wuqveaii.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2opztfpip.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dmykqqhg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ccfjorwx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mxpnxpta.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zdriafzd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nmyklrwd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ygvvwthw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wpxtrego.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wkrcurty.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2bzakdrqk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2logwayiq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xwpsuwkg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zmgfuqqa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2alhiwhxs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mwqepnnn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjwhsooq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2luzuhzrf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2hvghqgxa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2phbtiung.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rshfmtby.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nxudggli.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jrpwyzph.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2aykntflc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wzrldsmw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vkzwptez.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2dzhoewon.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wtpvncus.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ymtesdki.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2rsipfqup.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2evkkmbgk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tvuiibub.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tocdwfxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gawhuevs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wlqqfdxz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2juifgmmf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zucjkppa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2udpowkvr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywuuqlrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xfonrqib.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pdiixuff.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fkzjqljn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jpebupbe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ecuppbnd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zhvrxtsq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2uiorette.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ebemfffc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nxjuwajw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ycxcwryh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sqxhfdeg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2grhlblmt.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hkrhswiu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcduxnij.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xkwrwghs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fmqfgyjk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yezdnjda.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jlwhviis.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dhqqvgzw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2inhhubfx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2siczinzl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kmchvemi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2euvegmux.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hkfmkbcz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wrpuxgjs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rrirksoa.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2faypifkg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lmjswugp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sueuwfyt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rfwndvnd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vvgyoljk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2djwddlme.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2flvqwvfa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vbeapnnf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gtsprmax.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bocdzavl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nsolpgep.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2mhjncjxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wupbevor.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bnjjakar.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ynjvnefo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nfcjghgp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sreiezjk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zzwuaejr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yerkkrft.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pnngkepa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yijuwwmg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mdrjqbpo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pizsmdzp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahucgunn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oturhczw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fmuxxzhw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2iopjmsfm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qjdamism.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ggquplyd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2uniidnum.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2csiiqiwn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdkezsrz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tcwxbdsa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2husoywte.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rjyrlcnr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2saetmndq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2enzmslyl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ofurlmcr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ibsktuth.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gpssrzxa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mxqpxijg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lkexgjja.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2nrgksjrp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qiqzjscb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qqycodqy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tptxwwpp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qrcldjje.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ophxldpb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffwcftjv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qiiiooob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oonacduv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2iggcrxvg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvueaww.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjelvezt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvusdp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2towshscv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lkllaclu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bxpuiiev.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qzjtrgyg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2btvkxulo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vwwbxwjj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hdzhnhri.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2lrwgvajf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qzzdexsv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hlhvhkug.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnswbjex.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tmptiwaa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xgmzxhxo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2slvedphh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bvlcamzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqstbcud.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lpjloils.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2murbmema.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jubemjpg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2llzhxswz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ptskeami.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ytdvmsji.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pwzkkbwh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rqxeqkgt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2imtxjhyy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2miufkerl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wexcjjhc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xroficqe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lcprdsvr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ryxyenpr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehyvgbrs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2raewxglk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cqhftiwr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kecvlowd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jsiybtat.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mjtsfyop.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xxignpvj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2goineily.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rqryobzk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ucfzbash.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2idvljvzk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vfnivxfy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eszthbyr.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qkpvadao.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uglljqad.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gbbdcbum.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2tujstgsb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dulzcybj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cblhziha.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2aaqnljmc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2olhaqemg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mislxvpe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tlhfetdh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wsmutfuy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wskanouc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sjoxkjoq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2obrwvgdl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hupdfktt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rsiczzub.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pfkhpoxt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hxmaacyd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2awkxbvwm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ooojsrcp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2oeuuyanc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hgialnci.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ovbiatvj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptdttyxw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmfgqkim.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pgmxmzgk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lhxzbqrg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2isnrjdoq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pbefqius.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fzawufnw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tedexmuu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ptcggicf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2hljxvifm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wgfxkllz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mhdppmbm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2csicqcjo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vltkiptr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rdzfemrc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qbewgpnv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2igfjibth.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sskzimje.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lwtnotow.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tivmcsxg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbjhole.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pxdvacjl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rdfdflhn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wfpcozep.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nxlsmntq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xyjgacdl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jiukfeak.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uysvupfz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2qpdcpijx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2onbzlbmp.html


<!-- 参考信息 -->