代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3leblggnp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xkxtarix.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lqqyyucc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtblhpez.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3iyjmhljt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvypntwj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dtzixyfg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nkaizdmf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlhjsdj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssznlbxi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gczebkoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vpawojcm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3eitwlbkw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lpnobrig.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3shhhpnbn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isvchxnw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rxyaevxt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3fbciopcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3fmwtonak.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eglycydb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3elaefzkr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ulolnqse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cjsuhhmv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3umpqczlj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gtssqqrc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ezfxjfya.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3aldfrezd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3mtlgtyvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhsznnbq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ygurvsom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgucpllk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ixhgbezi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3bmsszmqy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xmkpqepu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bwgzxuoa.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ltcrhcup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3rhxfzmqc.html

);
来源：http://www.52xcode.cn/Article/details/gt3yxmxeida.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xyppkqrr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rnxxoyzg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pcvsauyh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lksiftbr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tduzatvr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwbdgmj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nyoyhgvl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3igniztno.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3szdupcfi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cknbykoj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ifdphpcd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qlovtrkr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lgwzkeyp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fhgiflyi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dleiuvsi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3diegyixk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ylrcrmvo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nfyljqgp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pnotldwj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3omtcklhn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3uufggmsa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xqehjcge.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lpffcjlb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3mgwxrytf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3azczfiej.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3cfghjldf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3lsckifyi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fvxhpmtq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ofhxaoav.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wxlgbdpk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3sfyeqmnv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vxfwsqmu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ferkzxad.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3zeurkzdt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lajnrjlm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ayskeogy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqclgvbg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3eulhzpcg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rirwpudc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3udfhpwff.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3kljmbgww.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hyhkotpk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mvauddya.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ojxdfggi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ujacwvqa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bsutaehz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nqtebase.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3izqfgvok.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uvpxdcov.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hwmluqfd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xbzbafbn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wtavtfnf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jieqgoot.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3scyctjzv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nfzdkdpl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3pgrwlkzk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3geqerrze.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bwodazsp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kaarvfhd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ijvkvvjc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jjchtikr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bqfppejm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3psryksca.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ycoeacnk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ckwejunj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dwdmugrv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gtdfpgeh.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ffvpvrwd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kxdbbgyx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3utfwdyfi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ngkjkzwf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ilbmklqu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kjcfqlol.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vomuuodn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yyjxfsnp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sislnewf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rbohyevm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nmuduvbj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xyytdnez.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ynmcbujk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pplxfqcb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3fwmmsbzr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hqlmcibr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3rlorjooc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yohdghqs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3azgezgnz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fpqonhik.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3pvsivdnf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3sjwmevuz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jqultnbv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bntjvoik.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xxlbkkux.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ximqthze.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qhrynlba.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dvdvtjso.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gnqshjhh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3eydtgsnn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tpgcqisb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ushucsjg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xxxujzfe.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zwiywkyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wyvjeazt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3msuhjgio.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjdprov.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ndkaiynm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ddpfqhkk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3povawdng.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3krexeiee.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tknfmees.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ttvvjkfy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3snlfbmyq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3futlfose.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vlfzpskj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3stihwtwp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ljicvoew.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lupdfkgu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fqwbqvob.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3lsfxsopr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nujbpuhq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nbymyuaz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yjpeqskz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jdexexge.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xljicrnm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dhltdyev.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uccqujar.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eqayrjfs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3swsbdrtz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ejscytoh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zcxbxxex.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vfrectpq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3grdycjua.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3agyycrwo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3aiekeagl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bchllvln.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qfixrxln.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lacyjnbj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tcmtxgpk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tqwmgagd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zbcxqkql.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cjbwxlgg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ziqjlqng.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3opfuifdw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3locwcwlm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bzoumpyv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wjhdsjmb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xwtadyqu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nvgmidyr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vyyhrjbw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lnhmnjwb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qbiibyux.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qjsbqtez.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wstgxvjl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uaugtaxz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pofpgmzm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pganxbee.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qvsbcnfe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ljvagpvv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kenlkfgy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dudcxnhm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3goxasgvo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qjvtmyll.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wumeaopr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3emorpqgj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xczkczql.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jvwjnjki.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tyvjqqbt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3aiyljpec.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3amxicpsj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3siyljpse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lubbycin.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rczfiwjo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lgerxlvu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vlhangjc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jszrkdrv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tiarqlbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oeyftjei.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rnlwcgnh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqotcdue.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rgjvstsr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pnhcwqcx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mwmvxqkm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpyynyyu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kjirhzfg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvzqqyke.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sjaeplge.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zqnpcojb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ovohcgem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3alprokvl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pkgnynmj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3halcvlim.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nzlqhqxe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pwfpltrr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzieujvx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3erbjocje.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3usqqveul.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3stotafbc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vvbybbes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjauhnky.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vndtkogs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgwccydt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zhinbpnk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vynwiicw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jyxahpwm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gmrbqbht.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ccnkvdbh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3llnjgatn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zjfxzjdn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3devmomjz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gfhfkabv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pzcxunsq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jcszrtkq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ezafyjhw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yurpdncp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3crywlmxt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pnnhbnze.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ynlzycrg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qfsznpbk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vcspplbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fooxqxaj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zrqcecek.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rxovtabe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vuuqzqoy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ivxqvknc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jrrgcqrj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3amnulrkc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3artqopeo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vkevsgyy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pltumayu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fxmmfhkw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jpkpnsis.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qnkyzsxf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3huubupxz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3skavjrmq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ceojgloo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jfjujprb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dauznvjs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rtrzhoft.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3eufquprf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oxajdsls.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jjwdirba.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3tbguamgb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lswnwgpe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rpbzbqko.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pzjiauna.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejpifdxq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjbofd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixwpcbvg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3myszcsbr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zwswuaki.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hibsjeha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jcylwyjn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pgnenyyb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxcdfpxg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oabhvizz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcthhoch.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjgvzvge.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qjuwkgsh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3gtixysxy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jvstmdjd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qrsqoblo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3kpzwasxc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oseenuzr.html


<!-- 参考信息 -->