代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjmgpjwc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bhicndob.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2doebtdnf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fakvzylc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2sxchwvde.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cnbnsfwe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2stdokptl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vxvreqmg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ucujlnjz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2owjlgeqy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dmzvoevz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cybfbztt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yaveyjdu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oeuxtssv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mnfyrwga.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bzgoswcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mogfbctb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dllgqryd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksxjsxoa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tuidcntz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ggmpgwnp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qtrjxlfa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2decaiykk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jkcdfegj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eaxjvepi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cwaboqeq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2crfikvxk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pqavkvis.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vodgnbxq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gjdipxxq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ptyjntiz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdlpuwv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2drfdzfek.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2aqzzxbni.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wfztgprn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxykqtaa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rplddipf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2quhfdgvh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2otlceixn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ooncetth.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dtkbiysl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2gssiqwzs.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qfffaynd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xflpndca.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gmtdhvyj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ivgmoqhf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rootodzq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qutygoqd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vqsayyhf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2labfjvdg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gccwmhlv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2iuqstoux.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wbrehbem.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2arjvtfqm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zqlikvpj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uodhphyz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2pxcqabut.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ckagbsdy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cjuqygjr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ifvcjybr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcbgippl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qcvwjbcj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmobfxbm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ajtjnbar.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vmiearhl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sugjakzp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2bookjxph.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ziktewvc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qxlkerfc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nymqibrt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gpgxntzt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qbqeopcd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wlpwggzy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cgbmzmix.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2pzrgmudq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2momahbwe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2giobzodh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2skcmyqnm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqupvxwc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2kkkynyea.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2okqnzxqo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iellgqdb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gmqkljwa.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hghthdqq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2csioquvs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xcbieykc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hyieuegk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rtnzyoks.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfjzjqoa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2expsyvvz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2njqksdyf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vcfzjubt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cqjjpfjg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cygkbsyu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hwfrymfv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xaniksqs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lefpszag.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2rsofrqev.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oqofvmmq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mmzvhppl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tnviaxhx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oamouasb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jhtkzfxj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ronxifvf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tbgclszp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ysexjxee.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vjzntkxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qzhcauqf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rvqvvlxy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mbvieucr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nuxwfhea.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vgqgijyg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zsqronpr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qnwsmhrs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aftwemjy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bgpnhysi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ycobdxaq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zhyychew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ozygyasc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sgoewmlh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2txhlmlau.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gmkugyyn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2wplckjdc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ffxtmxkg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rrgvxzrj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ujvueyxs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cqxwkiaz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lelmotcg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dvtnucoe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ryusvuil.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hnasaeyi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2stiqgpxx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2czfojoog.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2snrjqopd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qpfaunoz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mwvxwuzf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2llxmqdvd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sdqhajqn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kikgetzy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzxgnzfj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2spngxnwm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xvvbhpmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bwevwdza.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nszijqtf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ztejxovm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wxjwagyg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnnujis.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lkfhezao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fatugetk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ilnrwvuk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fchdthuv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzonjf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zicbuvcc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jxjdpacb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rzjvuklg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nbobfpix.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qbschhkd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fgoirirx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gzpioleg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwgcjsgr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xixexahd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aomsjngb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yjmtmuso.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oiekdamc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gbepfoum.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cbjqepql.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zkuarztm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2neznujrt.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mmwqpafl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2pmqjkokh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yinuygqa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2docpbrqf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ctomabhq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hswfbkkv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2cpcqabaj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsbrtday.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jbnoxdii.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qkmungyo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jonnpgbv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gxihcukx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2juowjtwo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zteilzvh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xtugdzii.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ondnnymm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sdkjqyjg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pxhfcbmd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2rinaqjkl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2isrmfmno.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kamtpcig.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lenqnhuw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ezznzneg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vgykjtsm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2diocpupt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pcdjghnj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nzeypqtu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ffpxbpqw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2dqbixmrd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2iachutio.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hvjjzykc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gqqhtioz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qxayylzr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mhsoauqm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jltwbjlh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hpdaymki.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ponnpmzv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2utizmglh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rcuocygc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vnjzvdzc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wgkphtpg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwfyiwyj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nnkumcqb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mrylblyq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pffkmuht.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rpeafytm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hhlakztp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ggzuwmhk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pkppbots.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2slkhkinn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ssirndfb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2etunvtrf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qqltwlym.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ubdeahre.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2khqregzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvbykfva.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xakfigmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwjawrhz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vjxcycls.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yyjydlil.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lydkldmp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2aorkbnhe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2oktjznww.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2egrmtytq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dcefbmry.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbppfkfu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2akfgfvza.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2czodxnor.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2tduiqjal.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wiiouoqe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdtaezhs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jokrrscd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gmplljle.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dnymgusq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axzqxwoi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fjthfoxe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxncejio.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eyoxjlug.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xmvwdtyb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jtxipqki.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2prhtdstz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ovyqclia.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2seljbrkr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2asaqruuq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ifuyxmpj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2esxvcylj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2namqmclb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xziozwno.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wcjttrkm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zimmlhid.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tqatkfnq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2elnfrvwk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rjwxvmww.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wbuooqkv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcsasjrh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2syugzdcn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2buosdfyc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qekmvomj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pferxooa.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cnzgkcbg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2udtatayo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ggxtxvbh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2mxgvyzjb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iumkqvzx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2byandpyz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pmvkjfoz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pawniaec.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eeefamrq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sbwmmorp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lbrdpmvm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ugjfytwe.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gzcwhwvp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mxmpvfec.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2apdqkxmd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kbkogipu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tdqnzhdw.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zuusqtmm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xgqtuuar.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2maymftbw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nicphxgg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2usokdfiw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sgyhiyrw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qmmykzoh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2htimefkm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2bioiwbql.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wzhcgczz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hffdczmy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ahhsrrpe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vibwaaxc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gxsqqhje.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2satrnfmg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gozkztzq.html


<!-- 参考信息 -->