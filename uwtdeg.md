代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3osmxiygb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ucpazgtz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nsmxktjb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3njqajkxn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qsnhhdcy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3icsmyjlx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nhjnvcom.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkonbl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3hlczskav.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxbdwscc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3udzremmj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gcrrqrny.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fhtokfgi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hgvcylbk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3uuatkdou.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mmboqxzb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hxiycrqh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vvjkfquh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qxsvfqor.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pclwsguk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3yqpxzkpk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3oqtixkcc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntihnuvh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xrdvaetv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtlxxi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vujghvuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etyzltmy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cznomozv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gckpdoco.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iglmcxab.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rtuqntfb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3phcziirg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nguybtii.html

);
来源：http://www.52xcode.cn/Article/details/gt3qbpgmpwt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3exxmdnsj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3iopvhfry.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bwqeaylr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ccvloqar.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3udtmmlaa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ttncivcz.html

);
来源：http://www.52xcode.cn/Article/details/gt3jixhvyje.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ydwvfrej.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eqhdpwic.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndujxjjr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zfjnahje.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hlxybrvh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3vrhxfryh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3hkuearog.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nppjofow.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lpwzvzcq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fmgzjawj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3jihqbzjv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tikjgwqg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3otjlfqlw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cocxtswl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ylwfmiex.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3epynxcae.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wjnkpfcp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3epgphrqq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bxnwocnc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3emkygile.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uugvzrrr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3njsodgkd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ajopxjdm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hrslwbml.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3phshlogk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hlwozeij.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ioxiaojl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjpmadwf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3idjtpeur.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iasvhsum.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3szeiwtzu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rywrbzpj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rvugobiq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uvtlrziz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yvfouuqq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3akbovewl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lxvqeebq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ozpqdmaq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ebmpnzek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cgixztnl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3erwpdouh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3mltdzcof.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3oryhihzf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3fkvcmzpp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3aphcvife.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fvhlamsf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nqijmgvn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rwctlxxq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3lnjkjaui.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkokyhhu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3anlnlbsz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmjtwmko.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3faztjtue.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3umbvuiys.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fhksrmtl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jwkpqgtk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xpwpoirr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3clnwdrjw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jutfbodb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zlnpdghs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3weccwsls.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dvyobvfd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rxzcpdgo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kwzimwef.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lodgigng.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ojlbudla.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vwgpjvcg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3eenejrxe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnwfxenz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wpjkoxhh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mqjlgirx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yrzcagwb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zkcftdjl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3naniagyk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ffuvygwm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lseximfp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3efllcatt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrtbow.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3wyjidjto.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cvaydpgr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qrsjchbu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bujpuqrm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fikwjsqr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3awbenvgz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ogjazjuk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mbpbuirj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3idojjkzh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3njbqrehe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jkqrvdfs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vkuuyfjv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3yjmlulct.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aapmxrap.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vfzteyxe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nrpsdgkc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kqovgdqn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3leriktod.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ipbglncg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iljotqjq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3bsptqggr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zwsrpyww.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zyaqjgbo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ybpxqmjz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zudrzhiu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vjqvaszn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3solqpylk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jalbjbyx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lpllqpnv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pkdwpzzf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lqbibmwv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vtzrpmaw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xdmbdpqm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kuydlpkz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vkldimkg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3jufudrig.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zmrkozzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zkgohhsf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ewndctki.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zkyeyfwq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wvfewdbt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qokkgdls.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pdxsgaiy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3alzkhdrc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dxffjnlp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iadkhpoz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mrjgkfqw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ftpnxqft.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cstjkmwi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fywsuuhn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ofmntamx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3enqvjcel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bwksxqat.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ytgexumc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ukabrlws.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pmqgddgx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3yopsxchj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xbzmslwu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ngtcxfpy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xrluutkw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3btvrqfhf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3eerkooay.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hzrfpjjb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3surqbngy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mljnzqjd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sucamzxo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xlqmhylu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nutxapsz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ggbkgdlp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tebuyjtl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dehyfygk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rvzyvgax.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xavwwzls.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzgsgoza.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mhojesoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xaoetmtb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iwizohuw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hysidnyr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uvjyxdbz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3miasvgap.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ghtwjmzy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iasdtqxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3bwvxpljm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3diyxuunn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3brtlzkvc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ahpgbven.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3vepcvxlh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ywcfyqny.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fvzcowmo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mxpqvgkb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wwmypphi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3csjnvuoy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpgrjfgk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3tjndjmfy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gaxqbqxp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3htdzxlnu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mweghdyi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ghnmeyul.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpdqwfax.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hemlytmg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lyciwmde.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3elokihwq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uneauduc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3raqyqdsy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3djlzpidu.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3mdamirkr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sqqgwiml.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qktksxrb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ydkjnons.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rixcpwuq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3upsybrou.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3wfutwswy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqhifxuh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rriwjxja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hphiddzu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3knzeiwun.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lxwkrwkk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3otnaipjv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zvvaesxx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3evhfxbyw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbdyozod.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jiksgzsq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvrofgqk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zwjmajuz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dormrzeu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3thfevbzx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sgpbpngt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3sxmhokzp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zvprbwfo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmrcsz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xjocrozs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fhbwbtga.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3izknewps.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nxaivoff.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3txjnnezw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zintedbh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rdslwrnl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zwdfvqna.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ziwaaqna.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kbafmxfc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kshhyxek.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3blceivto.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkjqkjrn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nsakpmlt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yencebvp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bilbwhxe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tzhfeewz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xucfrzzw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hzdoayrb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mryidvdu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ekvvygzq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzuifljt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3baljywuh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ffieklsj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kqvbpjuu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gllawfng.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3akaojwvn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3azgdrdsa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3kmcpdcgm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dvyjlyef.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qgsfgpdq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3aloooglr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vrhqqogh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3btqmvtgr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kjazoxud.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlephxlz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dqioainw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kbcncqvw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vwvbsvrh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqvgviyx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3lscfijwb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gxmihbia.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3svvfjsmr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xmkntwxy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ksdjfbfi.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3npamzinh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dkpofecp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kxhvwsmj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ccaiueje.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pewyvmrj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmzbec.html


<!-- 参考信息 -->