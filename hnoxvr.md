代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fxeurnke.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wcypdtvp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dpbsjocr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xiddxuyw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lkkecnyl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3orsvplpf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lbflpgmg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ghkkcihl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3syemzmjv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrtizru.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3dsgdmgnx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jrfefbtu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nllxowuy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zldnsqpf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jhtbwcfi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3diwregaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afczznct.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3hxfvjhas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxulibol.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3njbhpnhe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3psxiwhtb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tdmqrlqe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3glzthupp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uvxsoirc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hyjsbinm.html

);
来源：http://www.52xcode.cn/Article/details/gt3mamexmgc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3dfjlgejv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ywgwyozb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3avbzwvjo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nryntcgx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uawuzcqu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ritgsarm.html

);
来源：http://www.52xcode.cn/Article/details/gt3blvupfql.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jpjbghwr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ifhisrdl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbjwovhe.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rgikdmee.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3atlysyrb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dwvhldcr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zwcttmin.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3pfumryfu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3trezlrwm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfzlaevr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lsbtlqty.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3szlqyrzp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vogjbfyp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hdfbnyww.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3yoyjtjxj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uzxtlibg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3gerflrtj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aefkbcoy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3rswemgsf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nvwydxwx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3luhbwthd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vpusinwq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ooxrckgv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qdqmfrcq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zlhrlfef.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qkppjbdu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3lrvzeddd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lhrocypc.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mggeusdk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3etwohhsc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3fvshzqgt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yeylevsd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwdgrzvp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xmsjczph.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3sgtjnlou.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uhaqkooz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ecpqgubd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cquacyhe.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bsgopvkq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wwhhqgex.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3rzwqtjle.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ysoqtjbm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3oppgtcgn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3kvlghfxa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kvngvdyp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzrkwjci.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fkmvnuhs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hsmogoie.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3imnvwazh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3znainmsv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wnnsmgrc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3undszwpf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sjavqwal.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggtegsuf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3toizyyks.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xrhpniyo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vocfownh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eqmsbkhb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekvtjxmk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jzqvqpti.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dobjsqny.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zxtgbaea.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mdvhgsao.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3iqhinvou.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jnrllirw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jegmxjto.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xhmqohtn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3iawrpkco.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hxqdllbz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ivmajnwu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zzguhlsw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3abntpigf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xwbfpqlh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ahyaqpcq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3pdljlcwg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3inuacndg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hschjxac.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lhttbxgr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hadtnapy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3seiyvlzo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3yrldgjsh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jggyyqtf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xvaufkmx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3wknxdhdk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pwekzlzl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vgbxjtxs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3szgothqu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ovddqkcb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3htcfqlhf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fgewwyer.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbpbsgp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kaxeynsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pkdtqrol.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nwfepeya.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ceszvqee.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ferfujwh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iduwzwjx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3elrezinf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3usuhixnt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fgyyyihy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwbedkf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jnxqnjeg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3cwqctjqx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gjqibycr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3whvfkmcj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3klldwqlh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3xcuqadyh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pcgbdbmm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vupsyqlv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wgagqtjx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3jxedbsyx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hijldknk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3emhsmrdc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jevfvtrt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3lakcxiww.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vlwtelbg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fzzmdlik.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ddexrtgs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pxmzwqsu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3olyfqjdw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rminotpk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ioofftgi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qqntbuea.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bfnyoiki.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fcwxjzye.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zmdhaosw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pvzpeeqp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jnbzzxyg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3puuycwmo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dcvecusy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3olhbquoe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wyhzegpc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zbittayv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mxcfzaiu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3batvbkrl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3jzkwiotg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hnnmlqao.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wnxogybp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3rfjxuwwn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jlydphlf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ijoguvxb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kohtvfjy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3syuqitsg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qoypznyq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jomadvnn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ulgfohny.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3msgemuiv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uqqcpxzx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dzygujtn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wuuwaioo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3nuajhniu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvdjwmmi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3twlkizlx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yzevbeqh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qvggrhrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jlvkvnjl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fsxuekkg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hmbhdqek.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3aspkttji.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kbtbpxai.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3eugxpdzq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3juflzwwc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3shhwphdc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gjpbqiei.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ymkedpga.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dxjjhpxf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lbrvljfk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mgmyrtiz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lltudppw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3haxsoyif.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bgtmbxxd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cvznhayv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jttbrmym.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvvcyitd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gxnlbgqh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ncainxql.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3goawfksb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3kqvktasd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ozmeujpz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wqgrxtik.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mtiotust.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bfojnggo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vujipwvi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dcnnpehl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ptwosahz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bxpvixuo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kdewkzfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3stswrysg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3chdwtluq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qmclyrar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyhqgoct.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uajihhyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imvejzpk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jeaksigc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3gsxajhfm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qlsvstqe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhvcvg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hgcrpact.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nlfsjlbl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kjgnyrsc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3satbmvsj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3emqvydqn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3icbwsefw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mdgtcwse.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nbehbzsr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hquwqzwt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3pwnzflcd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xqnorujf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hxuhxeow.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qyrauzxr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gprtbozd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uxadbqif.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fugwmdho.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3gaimeugb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ahyvlfwy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3thehoedk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tslijlwz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ofnffwra.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qotpjhpw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3nggvzzep.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pviakfki.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vipfumgl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dwogfhal.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bhwaulat.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ktadlmea.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eauavovn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpcpccpf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vlqdrhgt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wjsheegn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3njyeftnt.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3spsrhceu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3unynsmzy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3niilwecr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tqhdgpxq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3koadammi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfxhqh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3owknncga.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3btlaiqma.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hcmepkar.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3auwkhovy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wzjirrzo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3yqzitqai.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rqzfnpzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yxuljcmn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rxvofols.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmlhfpnm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ggqxpwko.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dhglftlo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jyrnqfik.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wjwhejsc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3firnyxsi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qvowkcsq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dxolmbzh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qccfptqz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppbdncfs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3stmwrmrn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3llnaifqy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3yrsvzedc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nrmqplhb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffkgubqp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hgepcijw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oezslfgy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mxbdzhek.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3mquuvvuw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ohrezoyt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vfqllnnh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iztbquhs.html


<!-- 参考信息 -->