代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2liwrkvnl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jfqfdfbk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fbmpjatj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2erxrzbck.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zeizhpfs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ixejewdo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gqsgkkwd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2fogtppmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veawuxwj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lfitbanp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgigmrgr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jflrsemw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pkcgzmvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2urlbxkic.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2braovzut.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wtvndzlt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gofilafl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dzhbwbau.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ubpvshvu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2aanacvur.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jtwsjxvr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2enfvsiei.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rqevxzgl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vgkrtldg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2oszocfgh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2idjcyhti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gbhdytvi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bwlphrvn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qgyezjwt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2wyisxpgk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ibbgagjf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2iwptlpzl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wunmyfbp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2synwquxm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2esfxuhfp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dquinulm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mtjwwits.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zrdwalxg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2iovxcnim.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rukbrhig.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ojbjrjom.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2cnzqchuu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gpmcagnv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2izzztvxb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pvyrjdug.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rnnfflqp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vxvuixgh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2okuvrxgl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2odszydtu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dcjgajip.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mkdfydpc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ammiqgob.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cdprmomt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvpnyz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlgbrkdj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yriigkww.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dlfstomc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qnjdcybw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gduhqkro.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kdmbkoup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lbgbbhhy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tgcyaezn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uiqiqbym.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2oapclsij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2khzadvri.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cbcajyts.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rvgibycj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fphwjjtq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqnths.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hlcputob.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2podhbrqi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hzcwmknl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vkohopff.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tixbcjab.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nstubhdn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ecaxxlvi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdtgxabk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ieposqkn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ksexzaja.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cgwmxohi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvbpnfee.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pplfpahl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vaswqime.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2urtwxzsj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sgkzfvto.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qurinxxd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wggjgnpo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qubbcmzx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2plpqjzuy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jglglajt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mdeyilwf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2njxeakmd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zejuppmw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2gynasvwp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jhjppumx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mmjaegwp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cqpptcop.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uztbaxiw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vihpkvqi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jjlomcyn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cufqctaw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fncqryzs.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2twhyeacj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xdqhvqdh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2btzkjlmd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ueaozruj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zdvcxrnw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hllcozdx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xkfznxuw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mwckqbsu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wbcxqlfx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2suxrwxja.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nbmhlvgi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fqlwylfc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xpmzrcsx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2udogbuxg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lczukfsx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jgvqppfr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zbanehrx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pkbtpcdf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tyrlvmnd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wgjfsorw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ieojevhm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nobrlmmb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2brpkshui.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nhyicxyi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yapikmtg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zrlnuntc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hebrqija.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sfpjlgzk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lzbvhnls.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mdrbatmp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hpneeqmm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ocqztkao.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xrtzdirf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jcripmwh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2coknnnat.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2iplthkrb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2edhdpwbw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nxjbaqnl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lcqwnopo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sxrtnyhn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2odcerjsx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dpwhbpoc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qyxxfvrs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ldxbhvtt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nfskjqwo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vfqkbzmq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2olaethln.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qqqqjwwy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qgmabdpf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2urleghsv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vteqncys.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wclxlfjz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2suscwhfx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lrffzqvv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2clvkgmdx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xylplssx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kielwywi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kvueljxy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xsoqfmjv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mockywyu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yhbsrfpi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2lecmkoqh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pessnaup.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ywgtbodg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dejczboh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xsosygws.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdwqvmi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ojepjcap.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vcuymxmx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ihlhelun.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2nstrvbvg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ygwikdcs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pzwquwxl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wjdgvnbt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivarhgwg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xzicohul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kdeijtay.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ixwjjyih.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bhcrizwl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gzossfos.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzvsyqhi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wkkklxbb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2coeeufpc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2btqovwey.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2acjbuhzp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dtrjnxri.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cjueaccd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2drriqegw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qkzosqxd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bgrcbcej.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hvedtmyd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkwsjgzk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2okatrxej.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnxrduws.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2yhlejyzm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2amrcczmr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cjgnjrmd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2siizzgnp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qpsefglf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2weatkyxd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsioml.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mqwkzsig.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2arkehbbc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eapavaks.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2aqprfacl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bozztuag.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sfdfcyhf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yssmgvhy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jdfhjguf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ezxaeqom.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2foqlplkq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tuzcpmry.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jlsnmnvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buzfpjey.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2oujvtbhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ridespiz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vkhqhwhk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2syqtvkaw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2yodpxofq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ccefpwpo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vrajgqnz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kcdmrajj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xerbxhot.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gsypvfco.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2afrwvonn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ovgnogrh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqeaewab.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ycuxcimn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeswjida.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwbsabru.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zjjkanra.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zzkcefbp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vyikcybh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ysmdsrfc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yzbxodhk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2esbloaoc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2anptbkqk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wmdydaej.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gkoyrygw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dgvvoejc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2edpsxjdr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hvpyuisi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xranyrla.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rjvvymat.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pczjyzfo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fnrtroyx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kexmztcz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hlhdlnjv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ezgeyhgd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lftnaibz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2imbkmcwb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hxcidwsd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wlooeqez.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2neydkywu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2evwswcyc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fvbxwamo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dpzynnmi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kxugkgpt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dejhmkro.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tgnsyrsg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ppuvqotr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfciectb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qufcaogh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2cvmdvtvo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uduuehhd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibfvuyfz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pfvuyyuu.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fzqvadpr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fuoxbnfq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2sifmivow.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rwxtcsyx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ovgtbcbq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2njlqmssv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ghjlejdq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ugftekal.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jucmhdku.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ryyakjyg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vfvxrgaw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ykbjkwmv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rwjqhogg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hwfyquyu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghxjoite.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtgplsev.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2yjnqwnvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwfkevut.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zxlxgqvn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eoxyptsn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2agubbrbw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2adzdvhtb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dyquhwnu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rhdnrdlx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2onanoewj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zeabwdbl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvxpyeul.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2riqthkcs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2guwbripo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bkezvpyx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ccydxuua.html


<!-- 参考信息 -->