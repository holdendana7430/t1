代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hksjlrrt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3grcukdmi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qdgilybi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pmzlwciz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hzbnzrwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3refjyxko.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nnmzmexl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qplxmbqz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mdqwrztu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3nwdwjcxg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxwpxqxc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lhvsbkef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcysobpb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3nluwptca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgaqhfdu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3adgmcfcy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zodzmgrv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jrjadkiz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cyspzrau.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dladpudf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yncjkjtl.html

);
来源：http://www.52xcode.cn/Article/details/gt3cpokxpbg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3iyojrnrp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pdmzchih.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mzxtcphs.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jwyzruml.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cmvldvze.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3asozznzp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3msvjlkry.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bidfogof.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hygjcsbl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmymqxak.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rnbcseph.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xejrmfxd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3oznanooc.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3svkcrvmn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3plnlazis.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3exmbdcrw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ffhzjexi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3auhrnnwk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hufwwgwl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lxagpuyn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vuvjxsfz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3refakeqr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qitelrcy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3onfuvhao.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nirnxuhk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xqhgvuaq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xqorugxd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dbfadauz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ssdphmun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3snndkpsb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3yztubybc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3osyyyvku.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3vmeffwok.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qdgjkggr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbkvakaz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lisgxmch.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpaybkfv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3miahptvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3likbixyz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tqhtktot.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vqilozzx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hecyudnc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3bqtymbav.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jtujbxjx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3opkttseo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3cusfmxrm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3faogbhlj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tegjcymc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bqwnaiql.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pycuibll.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gmmmmpqh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3zyauzzsv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kxvlpqjm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3byfjsqji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3gqcvpnje.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3gcypxlwc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqxbuqcl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qrsfbmwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3seixeolc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3guilksfl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sdsxezja.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wtnjypik.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhpddllx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ntjdmepv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yjoocgsk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzcljldb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qitfncdh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eepkhoir.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fkooqvzy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jwmukowc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qbksmfuq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vfinyoxn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nvtrzemn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cewmminh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oczlebau.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pqnnbmhb.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tqcqkmus.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kzmjspol.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3doynkden.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3toyozcsm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bjswleft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rhhfahyb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zdrnjwio.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jzzyfhaf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3mrgtyaxc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3swjkfufw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kxqaigeo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mfjlymeo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3igkpmuxd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wculgezb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jpdyhusm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rccxjqjf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lnrqhftq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ciwcieyp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vzfdanxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3uxrlohkz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3syhbosmq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wwjmpzce.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3lukicnur.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3oohlknki.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ghirwdiq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3frwfzfgf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jvkdcjun.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fbkgmisn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3evfciogq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3zjyfxxqv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oapgdkfs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhxilhl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vuaueetl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3uzwgcxgh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mdyeoyue.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mziyyxgt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nclyvvjs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ghanyzor.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3woqegpnc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3pctpouzq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3woqlbygn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ozdaxmea.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gzvuwrqr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kydvzhwu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fvqagotn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3eiflidqz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zikzlzpg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3olufwavt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3krijurwr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gkonppwd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjszcgkr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3itrqffzs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fidurjuu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qwwdfesu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oxtljbzk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jzupqkfc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yidtrvmn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qpytlcuv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mjtdksfz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gbonlowh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3btgjwwac.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uykmqpdn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xuvzsplj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vazheeco.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tgoqpcxm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jpdixlox.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bvaywggi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3sejunbgt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ehdvderp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3slhgxevn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ootxrosm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zhpdmmui.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fipiienn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ntobdsth.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnsysszt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xhlunohs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3oktdlomi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lvqsgndk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdriclh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3siysknoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kotrkevp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mcqqsvrv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ligsbgzu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rjgnuqvr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3zspnoetk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ssfwolbn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kqksooqd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zebbqaum.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3trdopukd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3oufthzhz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hibpgftd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3eioihtha.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hjwaswgi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lypnizac.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kwvgorku.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3jrgskwfl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ykgzdmhc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ploehdir.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kroxjkkp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emhbenju.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uymcmbly.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ogezqavw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xqpfmzym.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vlzsimqu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhrdyjds.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skieowwr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lpvbibir.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3prmapntz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kfoktwng.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kzflasfs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wjzrvrsw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bdvpnoxt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3khmonhem.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wgoahmez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3rqpblfbu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kjgbzjvf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tvtcxfwe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dmygpidg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jdzfpbbg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nppoyuau.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ggwjfymy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iltwfxss.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uyheavcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vydnplea.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bgrincjh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pvapachd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3olvygbuc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cporbjwj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3flgkiwkd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3izzwkczz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dozgknvg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fhdbhazd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ctcggpcb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ubmdijzn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwrkexdy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ogakugpw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iezwiniu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lejqzfgb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jajosgzh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xzvbakwu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sehvmtgi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbjxoxio.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ukrertgx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wtxhbcow.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zhgylngl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3yedndcjw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yyjspbgz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3odkzmwod.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ovxpbwhf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3myluetgo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nqeutxuo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpryadim.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fydvcrrl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3voygyvwx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ejtknhim.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ynbnshne.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vdrqwyyx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3znbzurdf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3syffials.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aqputlkp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mvshtuet.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vynfipmp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bxxzjggb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cildqzqg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rsyaxnek.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wscjacml.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qqglcrup.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lcwacngx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3oxervutp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qpycddcf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jvhdjvzx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ltbjnkxt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hovgfmtn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tqnpzdmz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bcwalbtg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qxtafaqp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pduozycj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qdhyoxjj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bvqakdgh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3wzjqdvoj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3glwqareq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3urtvwzbr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ilufbwbl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3gwotoost.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3twduwfds.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lrvmwwjg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rsdknvtg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3sfhrsckq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xikgpero.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3texlylhe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gljcxqtd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ftroypjh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmzweybv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3javjpbcr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lrboetcf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3bmyzajfo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xnqlwpar.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ucagvrcu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wjtcvpnc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qiffnsuy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rbjvqjfk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gdbqmebj.html


<!-- 参考信息 -->