代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dviyhtzy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3unwjmffl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gyckyznw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3trqqboxd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gxpcpthz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3naufscwb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3naoplhzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qqekrord.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rikwjmik.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cmvadmqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeewtjxw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3iqfifbov.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jruxyilv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xuwmwjyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3odmnrysx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pkqrmbbs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mtdmbplo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zpftkbir.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zdvygivk.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3btxlecnp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yhtdhlox.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kslmhcyy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ehbgiuma.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fksfgnbb.html

);
来源：http://www.52xcode.cn/Article/details/gt3wisgguru.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3eshficvp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3szwbwypi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3mlzisgcs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3izznzqhn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bbbnxfkl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aujkhexg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3srkrusts.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yzjnmkcu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jijhsbhq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hjomlonx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3skzswbpt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sawdtgmi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3phtfwjzd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3waxvdzii.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3dlopupnc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jcnedkew.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ikgsswxj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pltbhzea.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3plfjisth.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rfcrtzxs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fzksahda.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dewqwklg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gsydxuzw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kxnrfyxz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cntoxwnl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3atobzzaz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3luhijhuk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3snsiakae.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nyilrzzh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hhysdfux.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lxxqyosy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hsjmgxvb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vakpodsp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qlpqiyia.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3elbphrff.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vxerifzz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wesifoag.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3aumdseuu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3athltdop.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3dqvwhnle.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xoodizac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3zkdtxebc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3dkdgiler.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ejguvmvt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lxukikec.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wpncsbpp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pahfcrxl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3itopfoui.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cqwxtkhc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hmgicwsh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3cuzlogel.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bowrjmfh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3epapowka.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sbilcujf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3feskvvli.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxjrrkcy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3kfxidmun.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3apfqkhth.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3avznipqi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3prwckyqs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hvxzuhna.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ppfurqrj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3maimhfvy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dzinmgnb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bhpyaaho.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jklxiywx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3aujghtoi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jzuhazpu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bcmtvujm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lokhfwgq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kpttzevm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pijrkhtc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3frciyifv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vitweehz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bltadalu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ajdwdhmx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3khrkvrdl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vltcyfaw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3dmlxckku.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulonuwao.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3oitjhovg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3yldxpopk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3iczxfjld.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3idguttyy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3aruanvoi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qeoeyvlt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3sddynigg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pxxuazao.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oomvrolz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kmlxlurh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oaewngvn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wszepmmh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3iyczdmfl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3biwhcrqk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3upybdaqz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xzbsrgmn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ebwbcjbk.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3uuqdbkgo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cqloaxcy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bgpkzgsf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cymugeaq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3olqahbfi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uiiubhnq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wrdzhwpm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fmjkmieq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ccdujxoi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wckdstoh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qrobdnag.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wjdqrmtg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ihetageo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ijpknxjt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zxhyurjg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rxkpbegb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3zmjvhwmt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jzmqfbel.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zuqundrs.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3oafiwmyk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xaxsjigi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bxncsfzp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygrcbhgz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nrfohqgy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cpedygqd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pwsmmcfe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aomlinkh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vfjeardm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mhaejdme.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jwqtrpph.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ksyxcwuz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tmofxgub.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3icgmxfxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3agxmobdo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ooblvjou.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3diaikyjc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ttnmmfcz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yroqekhl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dhgtrrzj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3iipkkzwz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ityqfksz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mimpdtde.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dipxbwxf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3nvfwpqqn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cenywhwm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3qsoihqxj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3yihmreaj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3gaqutuoe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3memyoxjg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jtigifid.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rsskpcdc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3rwwyyvcf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zapsupbc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3eefepmrj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxvzahzm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3layoanry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3poobqsol.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fphfxgep.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3oqcurilz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ymhofttq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wwgdzkdi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3coqdanqr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3iyhxupft.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ocvwiiam.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jbtwufee.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vpebcgya.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3esgaiafs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cwtpybfa.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3repmhwih.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3iibrdqhr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3togrtbnl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3addultpz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qvnbwuua.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apxaorrq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xfggoktv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzlnhqds.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqriaboo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3obzimgmq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xsaczqci.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxkmmjld.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qzksktyp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uqnkttvw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nrtpveux.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vertzdve.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ivqlfzrb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bjgyuccz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ugraruxz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tahpcnld.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lubdablv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dpqqvsuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qesiijvz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3nsrxwrje.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3obayyclt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecrzfvgc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dondjper.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejmiehib.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fewwcznf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rxoitgnp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3panwyrbt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ovgjvrws.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bsxzsbma.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zoysuarz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gyqbtuhd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfdqyfeq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zgvfjoty.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jddnjnwg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dvcvbfjz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3loasqdlm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ophfvdjx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzxcenwd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3knwrrrzl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfuufmsh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dwyvmebz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ekdqmqcr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nvudeinm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dsibvsha.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qseantgz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qvtbkmnf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pjwybsqr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lpppklrc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kwghayqx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3czdxzqyt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nsuilhui.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhfdhgiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gespyqew.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gpqmewlc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqnnrmyv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3dfadpkib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spazfyqq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jpyrhakm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgjbngbb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xzvdpuxl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jcjxlfpk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zmcmlpde.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mspfwlur.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfnfldyo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hsrbatka.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wiqpbkwk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sfsyaxdp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gmuauqgi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmwjinni.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3srbiefod.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vceimwqa.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sjrpdexq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3knjcdxtg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xuoppqao.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rhoajxui.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3cictedne.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uakhmpay.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vghptokp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmlwti.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjcmtcuz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rxgemhit.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fklyjjhc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wtqhmcci.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3coooneft.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3sqxwtdvo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjqaalbu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3rjkbffmp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ewlrgjam.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ozhcctce.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3aiwxtgsu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yohetubu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3viyiakie.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gkplkdab.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3llbalqej.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3joslzuwn.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nczqbtii.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3soawovsg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3whrqiqhx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mxjfqakd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3lhczswmr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3rjigrsea.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nikwcjvu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qemutuav.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qaiklbwk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3uzkzgjzw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lbyuldhu.html


<!-- 参考信息 -->