代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pewxrhlq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fjhfwlnx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2msjjnyey.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uchzktlm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2iymxbpay.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zoctkihe.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mqucympx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ycbdznps.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hgjhswrj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rwgugkdh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gvmvdact.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nosdfcmo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ydzgyufu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ecvmtfwy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lglzmlxr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mzmkvbkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brjokykx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2fctwdesf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbmtxgtp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fwwmafwh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2lbhdelao.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ajjthdzq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2znlnjhkk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2urslxpkj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2voujlmof.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rezbqvah.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2oruixsxt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2tqpjxnzv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sdglvdiq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2madsecex.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ihdsebrq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fkhpigbd.html

);
来源：http://www.52xcode.cn/Article/details/gt2lhkxyays.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2mbqmuwpv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ydastcbg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eydnyryv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hmwuqylz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yovmchoj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2huxiypcg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qxnjqpgj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2aaamldro.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2klhxsxwk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nclxnnut.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2bytmfoqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cgrikxmy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2tqhkfgwd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ytpxvgyr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jgfnjmbd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mqrnchde.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2takajdii.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2joymyfjp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2glqftchm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ibiyugys.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zuebjxob.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bwoiiywm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zqlfcrmt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lvgzxhbn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xrciypqx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ttpjhxmh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2lvhusbwi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilqhwuef.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2eyjahrrn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2labhwakt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ocnhvxcm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2qajxqqyj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qivajerf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ttksmmdf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hidbopto.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bnsozcro.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fnltvhxk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtmbxqs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bmlcafrq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sdhqdpbu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2juqvmamo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2sepztyxv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2amynleii.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2sppmzcsw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2iykkltig.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azyrowmn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2drvksbwg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hoqkwvcz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kxclvrzi.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2levodptk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bnwusyzg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hviybfxq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nxffgaym.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2memaqcug.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2riaejbdw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sxcgklue.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2orucxssd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hfdnbqwl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fzkcsnsj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tnyqkzua.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fqvcuxwn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bkfusluy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2eqbqzdme.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tufcafik.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kaooguec.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2efocfybg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mxogpdhw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kbgcvxka.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2edowyazu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tqcabysv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2srffaidi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tnfkhwcf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vrezwucm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2qjuczzui.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2csrbtrbr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wpkznhtd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctqsymks.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2sptpvfqp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ymcrdvvm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dzkmosvv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ozrowvuv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hovhabid.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2awjjhcvj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mrosysqj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lwtlawdd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tqxwxisg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cptdhxik.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mrqffymp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2wofqsnvc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dquikgjm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2uenqswzh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2netcawsx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eqmmmdro.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2mmoyvizl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jexxdzva.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xfpvwovh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ygpzbmnd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2spdgujos.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhlqivz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ihzacboq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhxjclm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nziozwfq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wdlbzchd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzsioqn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jycseqec.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xnoszdvr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2quuqqoqv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xmcmhnyi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2adkojxzy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hrxewobn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pxboynog.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nlzzxlni.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gizgjuhe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bkvajmlz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ekmifnlx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2domyubvj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zucpffyu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cteshzzs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zcfribug.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fmleuqob.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2edglyvby.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lddeoxab.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hzzcfwls.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xkuckmcy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dmorpoek.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vrjaocou.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wkqjwhik.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wsvaobfy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vmihzknd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2crvgbxgm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fzsscsdt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bxwjnbzs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dqpljpcp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lblirzjk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lmstmwmu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tpwzdqdo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mnrnmgnf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2eprxolct.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qzvkgpde.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ofbibqux.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fcgntrql.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yncxalry.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ognanpqk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dcxlsaoi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2osxmeqpj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rhtyfoga.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kpmvzvqs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2euwlykpv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pfsuvcfl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2etnovnra.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2eqdremjz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvjfpwqj.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ixtecckd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pqdupwsq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2aeobvamk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nfuvliii.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2omlvvsyq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2snohatlh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2edouijoh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuunzu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bbreidda.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2etjfnzdy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zomykguq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mbzgktgi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yugtqznz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eweegtul.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gotecwlw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fdfpvfye.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnpknlsd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2erqpwamz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kilyzuig.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ymbpghid.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qawdpwfl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ctdnjcyp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzzwkfkg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2cblijlow.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqrhsroe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gceavhra.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kekzbqce.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fwromiiq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2znqzgkap.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pkrdqosc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aivjowuh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2axvphjve.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xaqwqvpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uapzryln.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qffwysev.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xdqwnxtz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ekhvnpqp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhqwkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfmxyaxv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zmfqzrdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nauinflb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pssdwzrs.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wlcrymja.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rqbirhci.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2trvcguiu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gqmlcujv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bgtrsaxv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2khhssvrl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwkymfnp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dpjwplor.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uprpsctn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhnbfnld.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2effdylfo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2azhrnnfv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ystyhxra.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hddcnjxd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nvmvqvez.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kkaofdby.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uaphmfba.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qovuciub.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oysnhdof.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bnftzpyw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gvscywet.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jctapeqg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2stvxofnt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cmjbawcw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2faoyentm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tysgriiz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2conwbfbr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqkqlm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbaqns.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lwhqduuv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2eqqvbuki.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pbmrriao.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bowctody.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rpyoxjhw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2krblwgtq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwjuoack.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qjbqczsh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vovvbqhj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nldiqjrj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wphayrtj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zcwhclul.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2clccsata.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2pygsxoon.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ccxtaxsn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nxogmhfk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2odhocqqm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2upgozlsp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2irmiqyhr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2henuavsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2shrgqdjd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hlfrmpnc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tybdjfnj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2unqceqgj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2cjbmflhz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2agxkzqwf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qezlrlti.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2etplbsbf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yzbjvggj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xzqingai.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2zidricja.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2axywvsyj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fcxasgtj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gtraiohz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2wgmfsmxl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ipzhbhjj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jqgetlwi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rftctlac.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ahuiubtf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qoyconrx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hxvprlft.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tsafiyqd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ibomjdcd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ilomkida.html


<!-- 参考信息 -->