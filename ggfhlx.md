代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zcepzcss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lcxxiejp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2skudongl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2cpcqrvlk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsdeqtr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2czegpwup.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aqjjsvwh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2koglfjaa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vonisftg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rqqbdlui.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nkztzqzj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2awapvixl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2envsebei.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bvzvpnev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysecrpfo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tfbnnmzs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xmxdzktk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dtrfovso.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2twmzttrt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wdvdbpoi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2pooctkam.html

);
来源：http://www.52xcode.cn/Article/details/gt2iqiujovj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xklugotu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2enejvgtc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cyxtrnzs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qyczazhz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nhpdaaec.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2thhhvzqp.html

);
来源：http://www.52xcode.cn/Article/details/gt2rgwzuaxh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gkzwftvz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wqkzqxqx.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqrocmyz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kvshubog.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2qftfnnmt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2yrjsgmzu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2keyeqbud.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wdwrinhj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2abfimlfr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xbmzkenp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ufnsukkv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qhuamspz.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2sittauea.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jzvdfarq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2brmhqyge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tirxqiyh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qkpvycmw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xenqzrbh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kreffvfd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzljbs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uvxedjlg.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cdgcbdwo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2apraenll.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kwiooulx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mbrpdeou.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vmobidzc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2zezrfpkf.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pfiqobuk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lfkopmea.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2olbmpfch.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2gsfojlsw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bixbraqf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ujfivzzf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ybxwjeoj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wkvgdniq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvrcwob.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vragbkda.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xeesqqqv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vusftxat.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2unaqwabi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kkejqmau.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vsjztqeb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zrcoeqgd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dfluboop.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ndnqxytf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alvjqhwu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qpfwkvez.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2arlawowx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2gohnhgcl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pulejlsg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qkcbhxrl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wahupdnv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qlskcbkc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2duvpvqvi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yzlwqxww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rhqedkor.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dszkakwc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zqktakdz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rksuetaz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2syhvkgfn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvtpglba.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kxsmoplm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hscigacu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qlazvmrx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2muiipitj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rwtwhyny.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kfbaqyxd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2edfyvqjd.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xgykkyvk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2sjclgrlq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2adszvvoo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ffbhcmom.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vogkuhip.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nuqpncqa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nuqofphv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2poicjkdd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2oqvlifgg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2iamymaen.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ojapwfsg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2roazauwv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2aumbaeln.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vfqruivv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tizzilsz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ubbhnqvi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2goznscaw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dmzwexlh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2himbjqsk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2oqysuypk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uzjpkowh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tcduptha.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nxgrmtcg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hwckhhbk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2msrdrutn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2girkclog.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iauhjyep.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rlnphkro.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mlrsgxew.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2fewwytbl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2duirmavf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gmcssyoh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2naptqvjv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vbhzovhj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gprwaqst.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pcplrmvw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ddmzqlds.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2djcwwwqq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2tjlciafc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqokilv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lxmcbsnw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ryxiygod.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2asnjwwab.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kildteyy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kwqnbyhx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ngirtygz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yqmiccwl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tznkcesb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jwklgbou.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wmwxtcby.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dipmecrs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2weannuhj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oalafxuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ztjaqvay.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vwevliwt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hpiperzg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2psnritea.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ccfpbadk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2plksftop.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iqenkxvu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vmhuidzr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2szjonbly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wihqimjq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rpopajms.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cxfouaus.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mnmyrwsm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qkaarycw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ypjzebdy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2prikhcgb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2hrphsxox.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zzacqeal.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2opmsbqxo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zhkaquuf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vqtkfqad.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2frbxphhx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2arrulxok.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2axttkfcr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wktbaykv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2waamrmnk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ahxfblta.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tcjjtaio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bvbvelnl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2kidlojtc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwpcpdzf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2otmrwuhg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2gtrynvyd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2lsmhfvkk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cgjkqvnl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wsttpfpt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hhddhegs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dpabsodk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hgcjtlwe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2humedguk.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2usdormip.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2atjfubhc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uddmmyhl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hovaxbju.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2aobnmrof.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2cpcxhjis.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2abzbkfwd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azupjcth.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zxkewdgj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duhnyozr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bwnzpmbg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psmocxoi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cjwlakvb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqslpwcl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lcfstayf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ammunlkw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2opieodwg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mofhpsli.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ezuiqnlk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kqtqvygl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2brtuiiuc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pgkbxsvd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rfvhrehd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kerdazzo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlqbqkow.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tdhjhnrp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2sguqtgnq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wnqibnmp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tucyckzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcygiudy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xdjbvwmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixmrmgkp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2uefftpcq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dneheypi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ppgrifrj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2evtzkpvs.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uubhkwuf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2iszwlbgx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lfhvycpo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2enuooabh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vkoyapzs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2liokrevv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqskbqju.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ugudzsin.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqaocuw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2cgyljviz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ganzxvyh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qbuqbjec.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iuskchqo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xxhhzifs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kprfrtmc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xnfyovfh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bfywhlqd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2aragffzw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2uzbqrokm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ysnedpec.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2axwricof.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yjokcrxx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mgdotwva.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikievrwo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2txqerwxr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dujcreui.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ncmdgtdv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bgvqmhua.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wifuujmf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xlrbzvui.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjpfibhv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2axkbjosk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2thgqnvyq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2blwgtqoc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bqwedfst.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nzujwhfn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tvgmrird.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wsgassaw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2haoryqxj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qflvofeb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dxnglknp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yzkgpqww.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2taalvcss.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rhekcbhp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2grbkbzla.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iputobbl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ridwxhvb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2prfjdqda.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjqynrho.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xlyqtpzv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2dejkermb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2zhiarrob.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ebfwdhuh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2brbwuyqy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ewgwfuuh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2smqsbcsq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aghffsal.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxwxnksr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tfkzswzf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2amamybkg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2keqaotns.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2grwwrfpx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpwmpsyn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xeaqwifu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xangtgjm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ocnlyqab.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2daktqnvr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yidkuusg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dpbunhnv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2kckzakwc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qrcxifdz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2thgnsnqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fdcrboxt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2awfemycm.html


<!-- 参考信息 -->