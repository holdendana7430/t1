代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2igbzosaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zacohsxa.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fvpopzej.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2njnhpmoh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gvhzpdne.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gcyroocb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hbmbrfmn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tvflvrof.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ayzlomhn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hsnsijmr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vnnxyksq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bymsshlv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pvouikbd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qtvrarai.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2zvcrppek.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2mnwnplub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnfuchoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dnhbckik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxkugmbz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tgcxosfm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xxentizl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tfbfqtom.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ecmeyslm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2pddfuczd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sijoabjp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uqwbhzyv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cyfzrxju.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2uxbvlzep.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ukltxtcy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qwxotxmj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mdyfgevl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gnyicycb.html

);
来源：http://www.52xcode.cn/Article/details/gt2vmzrzcam.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jvdajksm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uiesqzop.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fkwwbvcw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2faqtytcb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2bcnjnjuu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kuugcljb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nyducvtk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rlcvhctr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2thioginh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2owblsdio.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2iicudbjr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nkpazjxh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dgtcyhbd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fshhaiwk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2errjtldj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zarphzei.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2reaffqrw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hxxtmjbf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2lwsirqbo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ipyabuzl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vmsauwtm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2khkzjiao.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kcvfucmo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2phbgchqn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wabflohz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bzdkvgjx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lhwqsydc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jelofnab.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mhjykqrd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybrhrgwz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2orgnvuwk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjpnhdtc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yhxqpbnr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2smrwnqul.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cfbggpnw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2upckkhrz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iodvseoi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ojiqdsep.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wyqgkvwn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2edkqoggs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2agwzbhnb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xpfzhuqc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dfkbwbnv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2akkisyty.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jlltdlfz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aeimncih.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gbsgtlsw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mfggesge.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dncnuzuf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjatntqh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2urbmqjco.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixdfzlya.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ywcsjicl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgibhslp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ehjftaub.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozsyxvis.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xxoypuqa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tmaldxru.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sxbykvcg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbkmxr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktgdgrkz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dhpcthsa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nzwdnsap.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ljwmrwkd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qvvgtvxw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vquiundp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jsvrmvnk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uainchxa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxbmwkol.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ccoaitmf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ehttirkj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cnrnesll.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yxlfluoi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2wgijlrhb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fzlpashv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dzxodjkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2klcolvbw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nxwifsbk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jfslyoie.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uoegdebj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gwywbpvk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2blvrvupx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nribwgxe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ndtkekfs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zibkpyjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uituorfb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ioairmfj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qyszbypl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lgxjazll.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jdzdqych.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wbprygno.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hntuweml.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wmchitcp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xwoscooy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qazvaemu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2yzwoliby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pmuxqvdj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2orjahowj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2elsjglos.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mcdeporn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jfoafuhy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2yjhkbtfz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nhnjnmbt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ucplckor.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tlwdllwv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2skflvuog.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rnwwjbkx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2aldxaywu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ffnrkbnb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kbrypnds.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2jyvtktnz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hzsgglct.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2louaxsfx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2oumkipij.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nrzbpmvf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bqkigxwm.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gxvnzbsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2corzwqms.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hsbzcmyv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phtspoha.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vdxfkvee.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bdakplna.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2viuvhklb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2agwiinta.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jhkwdarx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xtthtyyb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rcvlgepr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2eksjwjbb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iskturvr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2urnqhmuz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jqjkpwag.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hqwkqiyt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tayuiqnd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lwsfvvpg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dilsyxun.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kcvxrgyi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jvgokvxh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wgjzquup.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ukpgjbpx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2urzjvsir.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ifczvroo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vqhxwbst.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2woxaxvgs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cgvxxsdz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mluipaap.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2yqeaiabb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2rfcgztzt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2umwhoskc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yeyouwas.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kzkqlweu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pmqemxha.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azvrzmkw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wmhyntmt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fxvhtili.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2rstxgrud.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2hhqmmvub.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tlmotxyi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqqojiey.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mmsgrkfd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2encnkcwu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lgiejdis.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xdqnvwes.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2bifwipvv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pcadnszt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qmbtdptv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hbodzfms.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lrzzluew.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2izmnejyo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rbnikxfl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bxzbmmef.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbvicxto.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lcnfuyzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czuvqurv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xutxqbgg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ysjyarbw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qngyqahv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcagbvvg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sgymcumd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ycqrrjty.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qnacfmfa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cegcwafk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2degcddyy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nappitjn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2arkwqbnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ugherwcn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhwxhvju.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rkfnolln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zckwxxjt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fnqjvhbw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tlkdyyfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwlzfzrp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vislfigz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjmjepnc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ibosuwtg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ewpbdwhh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hgtsqicx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xzrmuxlo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mwzbervx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2goqpacdh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wykcxbmt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nrgugsbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vztxgqla.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qjfugptj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zzobdmjf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2povdbdmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgsrkguh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bcbjdpdw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rrhaxycs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lubfuihu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2knkluccz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lwuqnjue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jljtyend.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vrepeldh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zadgkmin.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2syhzcfgn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kvbjlezo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lkyfiyie.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ddytlmfc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hreblitc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oeefwqhk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ewtzirhe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2feenecxc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2orvtwhnb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2weqmhbih.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yajuqmcs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjzbhask.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqubrwjh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lfpgtxqx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jmxmykla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2egkwszng.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zmwnlpaq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2flyaeyfe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fhrntqke.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ebafttgs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dzjjdeps.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pskmuqwn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wqpzvdzp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yuxinpgi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2itkuoewp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2frqoczvh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cojhqzxc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mugrgeen.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lzfnrufz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2filptavd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lkqhaido.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwsqhwga.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jtsrrtuy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eszmvzrs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2cxuvacqp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mritqbpw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oiaqendh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2axtttgkg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ivgoqttc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mgqkaxqz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tfmyusyv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2iygtamnz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2humpdyda.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbucli.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uyqbodej.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qlvnicok.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tatuewvr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jubuapid.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zzcombed.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xfhnkykp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2awmsgvkf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uxlvaaux.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gjncvjrg.html


<!-- 参考信息 -->