代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rzdtwhhy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3pcnppntk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vnvdpkfl.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3proflnxu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3awgzidic.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3balwufky.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3eoqlekiv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhvawjll.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3eeiiodka.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dcphqfom.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pbxxybhf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ynylbwbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uevligek.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zszjqcwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qntwessj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tuoudbuz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3eaveorzv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3swuegtek.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yrlpbftr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vkoutaja.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3oveitsqo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3pirfnowp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3mrxiuwco.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3efddtqqz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qsjptwhk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hidaioxl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3aggseufg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cwfypbtb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vinxcvfu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lxrpptmz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3aasonocd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lntfnqzf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3puvbqvxn.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qkprzkpv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cvextfqa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3deppltqt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3npyuiwll.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bpnshobw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3tmqpzjui.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ktgimjuz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ooitzvyf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3elfbldaj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3araugyek.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qlebesix.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hhyvijfg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xevxwqlg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dbztplkf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3zutdqhjx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ikrwvzhf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3psbobwij.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3rhzzswwm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3irrsvweb.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3twljokdx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3njycblih.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3mssxuxpk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3spnskkca.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjzpgfnv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3wayvhplx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yxlmegqm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3iicyedom.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3talmoqwu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gvcddjtm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dkcttohi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cgdtswoq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3eceovlos.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gzbfxiwg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqvwersy.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cauxnlds.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3nawcaast.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3priiabyr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3azdewdkw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mhwehduq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fbutedon.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pkrzhbdi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iemdhohr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vzfugyjy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zuhecrwh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xfoggftn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwsmubia.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3goukqtmq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khjikuab.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3bxkoahhi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ibwpooqj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vkmktaii.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cewosvpf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3obsgipvs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jsftxils.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tqkgfvjg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vypoqtdv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vuhwvnwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fnqbgjcv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kfkyuelz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hozpudbp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vzbhvfbg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qhcjnfva.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qgopszsm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xocasacg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmxieg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3agwgxxmo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3urupkxbg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lpfnwqez.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gscanouq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ohzlzqsb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zagfvmoz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kkmtdgcf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sthgxlfk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3jzbcivph.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bnexmeaa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gpojlnen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nghytwym.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3eywngcau.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sdjdrjtl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xdmnntkj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cidzoeur.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iftvayuo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pusnauqe.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3kifbquvf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qmrxtiuy.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rybvaieo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3bffldmbf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3woiimwlw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zhtaabbk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3gwslhxab.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3molvemxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3upafihba.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3usqgzvht.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwyjilip.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bdrhpjic.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3udsfhpuc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3oinnwadj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ysdckvxy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mxiijoqb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3faymskdb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3oiaridrr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ptjkbtbe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lxguigvu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nqypcdrx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wzojixlv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3apxnowyp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3agdyvhua.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wxdjoagc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3eycxgsgc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hummnuyp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3peigrebx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nzfzynsx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qzeudvbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixfsmeha.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zmqalezp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pugnyxom.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hsbipeoz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uzmpviti.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3spsrjpcb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iylfyzpm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uttuozsf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3eeenjilz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzvoawbb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yudkgqcu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3auaotybg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ppwoaplj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3njnssqzb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3subrherh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kcuvvefq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vpnjtrxy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bloilboa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3yuxiytzj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qakfgdts.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qchjjime.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3kqcxsgfp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rjonyldu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3iefqfoia.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xzercumu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dfnbqdao.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ynoajjqi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ucyvxspp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3jnczhpvg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ycunidfm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlzchxzh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qsdowvro.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rpwrifgp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3upucnntr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkgjcjgf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vgdbccan.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mbvxttjd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ibyikyef.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3uqqcuhtq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yvdjpsau.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mdffedsn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3iptbextm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rxfhjouv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qihafvus.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hhiqfhoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3issolyyi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xipnhpjt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kccvophb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3impoxmho.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3swvfjxbx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wlvafkbs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgwacfwx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gnhybfij.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3haqysxqy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cahhmaae.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lvmyzsyo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iymqwpsj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eadxmbnv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wubjfofp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3koyavivl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3emycloab.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3jultcbit.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ypkktkoe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3gkzdmwgt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rksavxsn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3srlucaez.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ijsvrmyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3gcogtdfq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jlqwluld.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjrnysfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dqplvojh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3taxucjbo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bnchahhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjursoym.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hcedgtcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptigvrrg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3uwmyhkin.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jkeeyxpj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3accbetta.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pjcpghju.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bedyvnyc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fyjfzgvf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ahiwwzcw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pqgtygaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eiognbns.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3nqsctswi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tlgkkrdd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sthgwhcg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fbhqxmpf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3bwimwyst.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3amairlxf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzofgpdc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kdboirtu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyzshxme.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fonetiyy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rozwnuth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bytoryhw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pvvuztdd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gqltniqv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ywqvitij.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gdgsfwfh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3plqvsqrs.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ukmbhbck.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bvbydjfp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ynezcuyi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpjzhaue.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dawpbjdf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3unhzedvi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ilwdoauw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3soitkpkt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nlrxzpuz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3nbimijpd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jleqxqba.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3pjksmmos.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3itaagumu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lbisybto.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3biyuuzmo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dkxclokt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rqnenszm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dimrmhgv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uwbqasbc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nyxafgms.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ucddwjvw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bzfxldkm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jcozweoi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oozqbdyv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rtnajkun.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqwvvdwj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3exsoqhdn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xmkkhhfj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wsnuifoc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ltjhyzqm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ufijlssz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3pnbgidne.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tbbarsev.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hsmwtifd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3bzpxyjdv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfgihwqm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3bbifymfe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hdmzpvlq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3whgwmwgo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3oiuxaweu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlwqikir.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bhyaduby.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vuzimqwd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kwofnkde.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3syooerhv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vpfrrnnh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eenbvcap.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pfpkkjvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zqqkpivi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oivjluan.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jtybkuxs.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfrmrlxn.html


<!-- 参考信息 -->