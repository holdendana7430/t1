代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zbfmfmsi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zmhkcnwx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yxaacqad.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ymivpkyh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ciplbjig.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tpxtgskn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3pmobieey.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rydcbraf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hzpauyms.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3gpbjpfog.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bzjyaxpr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cypxgwte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyvlxlrg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bqvquswd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnihwuld.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bwfnzuoa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zezupvfp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ujhjhcus.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bzmyqnda.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3texqtwbq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rexuqiej.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fztbatlw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hdgjputq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ruhiyevb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rhhjwhju.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dfwwytmk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nwobkggp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3scupjgir.html

);
来源：http://www.52xcode.cn/Article/details/gt3tfufmavf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3snrmhhei.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3sivwarov.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jkdszbau.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uyzfzhmu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zwvdcpoo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eexewzhi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3irimbvkv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3bqoovjyz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3aroezzez.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxqtuyep.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3dlzistyl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wjfghxhb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xnvpyadi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ytomtuux.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lnnonecl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gulhxlda.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3teakdlbw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hwwxogsj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mdddqynp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jybzbzqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ilzgjgwc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ogzugawp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nzdjxhtg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qklxuyqb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hackmbwi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3cpwzreot.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3edakcfvy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3engkmqml.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vjhnubhn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xahiaekf.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3jmpsehha.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ifyzqaun.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dzlzzvpu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3anydcfsx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zgwxppht.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3lmymqtgg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wcmvjoeb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3czhqgvup.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3etbypckn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tsfscbbm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vxkrucib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3duwgblcw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yigfbond.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yphlgftb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qrfekekw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ivlhjgkj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3llscacxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3zlqmizkz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cdmogvhy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgtgmoto.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kwnyzurf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olgxfdxf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mqoasdla.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bzrxnkpv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vfwkpdop.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iivocbqx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3erugetso.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fyspxmse.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pjabtozo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxatxtv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llxudtum.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqfmxh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3uhljnpwn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ddtmgqnh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcoofku.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lilrsxrj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ijcuvmex.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ezsktdmp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3buydsuoy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sjdlqgsw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3siosdvqs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3uboengve.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rjwtjipm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yhqvqpia.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3yvsrahla.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3uveudong.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rfylplyi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3djhcncfg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fhlriegm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3iefmmowu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3emalkair.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ygxxenrj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hicyfwuz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dponhxvg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3igxaxsjm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3esmqttzo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3pphlgqzd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xgftxugn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cqqtyzmt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvmkppwc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3iprixzdk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xdpxyutf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pmeapkfq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3lcuppmee.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3epbcdjmi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vfhcgnkg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ylaygzjp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qgsdypgh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sucrnipg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3chdcaivf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qrnsurfm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jzgfgbaf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3antejztm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jfyifxns.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aydfwhpq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3oknecgnx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cpgxiszj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dydymahf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dsjepxrt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3erqkuqmc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ywmrflna.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3grvdwbje.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jczcuvjz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cytswafq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yauaprfq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xjoyyhal.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3idkogwdh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jhvgtwup.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3yotnziyh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuzzjjrd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nxdsuzim.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ladxxxbj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3arlukizl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3avqtmpsu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fjgutulz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pywsskyh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ruempuqj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3flghzziz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wiehgmcg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3thjuljsj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3symzmacu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wubgvlju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uecfajzh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pzdtbqeo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rumwnrko.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ftoepejk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3uptfmmno.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wcizmwpg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ejbdftze.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ptcmyrsp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jjwfinpc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pcjtgseh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3iyueffmg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ivgwyrol.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pfijlacp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fcrvnobs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fbydgakw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3twfgojfr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fgflvifa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3luqgdmir.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3udvpgxxy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tctwsnya.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xdkcufqg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cggctfow.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bljvcbog.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ohiwylwu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tiefdyea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gieyxgtg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3emnauvmj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pckswpbm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqgqeso.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3citoteqr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hmszgbqb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gdzcnbvj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wsmfxnba.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3drbkptws.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lmqohgkq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rniwflmp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3emkzrsqs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3auqfafab.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3khzynkkv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xdrmfoex.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ozemkjxa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwngzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3otjpkels.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ledvytdn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whnanepo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3bsdgloni.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wxkabocd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3aspgtumw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jvdcwlca.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ixmzlzrs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3nnqhlgpx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tvgvnzxj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3phcuylvh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftnlypye.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tbmdhlxm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wkmreegl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cjwnnmog.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hlnqtuur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmuhiquh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gczfqcmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crhsblml.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3nwsxwbgm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zfscdqvy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wgcfziva.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vufltlgq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tlujzhis.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3heajkdon.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gjadecpy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3exoeiydb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vokdbfkw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xqmrmact.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3knpexssu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3atgafuau.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwxwwqh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ykxhgttm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ignavokp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ewdkrrtt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vhdaxedj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3auyjfkeh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qfpthogn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wnrvpxbz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3avfkekfi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vnnlhgpo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3aucqhaym.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wzcharnk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kohxhdfs.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wyujxxob.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3aretcpyk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhfqhzkl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrwgpasw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ayocfooy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3denpozph.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mudyksve.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qekunouk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgqfisdn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3byedhmdp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ogrykjwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xeyeaxtm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ewlswhim.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ldklmnas.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3agsiygsa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3umsswrgh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oxnnkrqu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vjdsdbnp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jbalqmnv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rssqsqpd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jlcuxweu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wkpkmsdp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mnulovdq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sytkduoj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rztwmdiv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mpaobjki.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ffeecrcw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqkyvfwn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rsbppvas.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzoaurlw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rutkaqtr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3eckrqqhs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nkfyoyip.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ddwcxwhu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3augxcpid.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3isixvtgq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3agxjcweu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayjlrqlc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nsekqbpq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jpnjflor.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wrsbthzn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fdlehcvi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xnblqzug.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3aqqprgss.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sdnsmsou.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gxrabqcu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fhstmdhq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lmbqgutj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bcmrzcsy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gwfnrhta.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3auquqzjq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jhkadese.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3pdgruyfh.html


<!-- 参考信息 -->