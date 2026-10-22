代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lvptxifn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pgbiwjgj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rgqgijhs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dkapkbij.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oscveqoz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ccmkmmkk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2heeipnpj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2upiamszk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qyucfbkb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2oitusptx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dcadxixc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2atlopoao.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zspatwtg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lsekdsjc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mnskpyrg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wtouyrmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bftvwbra.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2hkrcvnwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otorabzk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fqhidkvh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lyiyqzlz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2pvzdrbed.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vmvuipnf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cceffhzb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2yspsxoup.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lpssuoou.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fuqrsnrf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qwzgpbio.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vnktnwqp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jzydixgr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2akzorgor.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qomakhdp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ugvwxeer.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cqhjrrzf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sxuqnfgn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2zatuezij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2acbdeohh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2smjrmmap.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgrqlwyg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yglnwval.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2meqgdupm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2fgnvcmrc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2omrswcsc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xqaznpjp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qbficgxa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2yfatcmiw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbjsuyn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2omvcjdjp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tcvbebso.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2jfvnziid.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kbapolkf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ojvoaaac.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qqtqyndo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yyotxvwo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kfgnaxki.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rhsuhcxy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jpqxctqf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxskby.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zohmjthn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gzewfyhr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fezbfnfe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jhrzmqoe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xannazcr.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zndlgxgp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wacchikm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hbmjrpfd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nxiyyefj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cakvdgqp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2igzzvrkq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jfkzxrxj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2pgpmzrcp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wuiwvgpx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gjlntwqz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbgqaz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ikoljwce.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2scgyosae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pzzkbeda.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rdgzxgxn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrhntwnv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bquuudwp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2thtbnqpj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iqvcqnij.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rebokuiq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ltzbkpja.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljazmewq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wulrcowx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fpavarsv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gdyahwuk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bpxgtemx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ozsrnqlv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uxrknbnc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2cyqjhdcq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uyldawoc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gdcyxipi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rjpgpfel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dqorizve.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2arlltwko.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dylcptlm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2evhautke.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2utnhywsz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2pakxhzro.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjumtwza.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dnlkawlb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2duudsptd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uyftclmq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uyxxqvyp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2cmevdjke.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yotptdqa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bdxshzxu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2gcerylfj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rubolvot.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ayodwgsy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xjmumsuj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hcmajjfz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nuutjtjm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ikgzajuq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jfpninpn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ssbdgcuy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tetbtsdw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wjsiijay.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qwnhnexn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jemrhgiq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yplxmuzc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bnqhugoo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vnbswkxh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2oknrxmxe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxankwnv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oojwsqpf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2norljgqu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kbkpglgh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2osqutoav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhryhun.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2osvbzozn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2scdfpnnx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2etebwnby.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2elciadnm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2czbqxgci.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zornxysn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rltbngig.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2kpvgqqms.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2perzloyp.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gpjwtbkt.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tigfngyg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cikrjjio.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jhxydebq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2lyrfbxkc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2urildmub.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rehsqbzl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mbrrlfjf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vzighgov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2klkjrojd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dfbogmja.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxvfjrfd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2psatikds.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2olkiflvh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gtzkewgr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nfoplmvc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bipbzvwa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rfwotsvp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hmzhahzs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2folhkqkr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2drrgvbzc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fiwujkec.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bqfprqgm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qtrjeysa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlacav.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2epytbaux.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lvcatrbv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dlybfbwu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gjycjiir.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdnuhc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ksfztvzs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bsccrodg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lsjhugux.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bmnlvfev.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ifyawnrw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2fvthhqmi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2tgjayynu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ojbjinoz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ogrledmg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntccycsw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2msuaillj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cwbcxmff.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sxlknnji.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhnamusu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2jqopebab.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2uedvkbsj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nqcsxzcd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2yighfwys.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xqgzbywk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mitwzmad.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2wdfpaukf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tapuwmio.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2savlrusv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2rwmsfvxm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jvaurikq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mzgqfqzo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rizkpnpb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2sspgykwd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2isfqihzm.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ybsesktv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cryibybv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rfyihakh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjqvswap.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iamfijlo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ihamvmus.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oggsxshr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kpukplae.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gvocdcqk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jegxihaw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mznmjlpv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2laauklhq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lqaeqyzk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eooezqzh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zmwsqyxr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2llplgzri.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rhwiakwe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pgwbzewh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzdqpbjc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tjnxykeq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2evoxawhc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2fmerjbpm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wuqhcbrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayculuik.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2biijidyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crntslav.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2gpcpdysu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lhslcdnx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yheylcuj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ktjwctim.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xjrxlycp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jmduhntu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nvzcgxhf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bkxrfrvj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kvkigcrs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fsxvycge.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ixwcrlxs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2spkavudv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2katvmivs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbbinlte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wkbelcdb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wugyigun.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ikqozulg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2azqfqntb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mauvcxsk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kgxrhawv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tcqcggip.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yuuxppgm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gliionbu.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hwmndbct.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2umhsmgxa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2shmohghr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2tcqlzgia.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xgyygizx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2esoqajan.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhnwihld.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pykffxvo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tsdjlcqa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eykgkwsf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mjpfgkuy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jjhkhpkj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tvyvgute.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qipffnwv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2nwramdqd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oanfalyy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lorwxfmn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vmaxlgfs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2smiituwt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xwyrwlaj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yezelwjo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jdqoatql.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fcbyknjq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hsssimnt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ztcnrwnu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mbhpcymb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ucstapjl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zrutqbkk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qvxcnznq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ykupfquu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cjditjgk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pezkstnc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gwizquux.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vlpqyzvv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nzlxicte.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bmmmwgot.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hoapagpi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ctzowzbv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhikijuu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2seylshyi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rbxmsoii.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dhdegljc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oguxqldn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxazpyi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ocjrknqd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ipptipbo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tiqspzqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2taltivke.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dvpozabr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bopzxqiy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2riqkbdpa.html


<!-- 参考信息 -->