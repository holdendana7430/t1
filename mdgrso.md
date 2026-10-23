代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3epkeouow.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3usbvwhpy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nmebrwos.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3catvkdmf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rrrztohg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mttfnbzk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kebszbkn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ippyfujv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xmrrsbvt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3sgdzqgni.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hygkymri.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flzhcxpu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3obhrpchv.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3yolmnhiv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nuofeanr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvfotfzk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhcjnvf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yphhinnu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xrtewhvl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3vdweafog.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ddjdurwb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iividvtx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gjrdykxl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssiuvlmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zhpogbvu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pkrmqnlb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vyvfukrj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3wmjfhaaw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlzgufe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ileqxinn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yazzgvnl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hjecjacu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rxlcwaua.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yiymgypp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ruhppjup.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xsmwobao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jckpawzd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ycykvkam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bceozfjc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3yfshlimp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3fwvbwvoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mrmbjmhr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vxdnlohz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ldtsjchk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xlaqxqwn.html

);
来源：http://www.52xcode.cn/Article/details/gt3klvvvnzi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wmqugcxm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rjzdnlcf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hghvctzv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dyzzflts.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pcqdokrx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3horurvpd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3izdyinkw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3prqissjb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gndivmgl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3asgkhtix.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3glvgmdsa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zlstfxcf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3swagsrfv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pqtdsxxd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wixcggov.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vbbgzwaz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ilxjtavs.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tbukvzkd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jotxzbdl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3npicdevf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3llebsdre.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hkyqzpgf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mzyfavzl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uvhuhmuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hcezfwsc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yohktwog.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xbdrfcrd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vszypsig.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vasrbjsx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ybdnmtjn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fmocnuyn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3celichzt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hsquufat.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ivakrxpb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bkjyaxow.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ebswzxqa.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvudfohz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3idrwuene.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wozdglyi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bognksdy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nanvjkwd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3aaktdrtd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vlrtnpoi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hpvlubtu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nimeulhu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3naqvjoev.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rczqczgr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3sxhtenuh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ngqdikms.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3khuwkqnk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tuxwdzfh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3yumkotos.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqxkvyvu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mcsxbcse.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3akkzjauu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uhgozhio.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hltzkdjw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3owwscddd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cyftqpmy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ztyvwepv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdvivlrv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ximqhboo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yyuqhsoe.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3orzdgliq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3guebjshj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njtfesan.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uzpwilvz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ktsybdrd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vvkctwcx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qppaaegk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3uznvckxe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3jjiasmjf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3tjixlumt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fuwoyerg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jrisnzcz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zocitanq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3yenrwtbx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3pnjtzcbj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3xfpduyvg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kehdudur.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3brtbdbua.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hskjulmf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qndnehxh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3hoksywso.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pqzgsozq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fwlvoxnq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wgmmuopl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3uqgvkbhd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3eexrkrbp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ytctxoln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cuiqyipz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fdyulccj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3idvhmyit.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3drfblsbg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ipftbvuy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zvlxwkpc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rbjilpba.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zugrzqqg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tguqiqyx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xtextmtm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3evabrunu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lfvfayhj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ybnysjbb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kzqatjmo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qrwlhptm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3udtpbwqj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3webqdgpe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3guvocceq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vzlenzst.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dxciyxen.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fgcgcczp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3czkejhng.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmnoqq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3temoxpgs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyxypobt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nfxawtsb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lbscpztd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ymucgjef.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lixnhbli.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3waueczyf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hudawqvs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3myjrfeqn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dqglsrqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3focitvce.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3repssdsm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ctoulmcl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zrxmnkei.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3esuscddm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3czembczx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jcbmanez.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwfighi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3caiibkro.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qrqmdmrs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tgpiiwhm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cfzwaygj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ifhhyfgj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tafiradz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mowuzzfg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kiwipoaf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3retsblyy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dfyefodj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ibxyvrrx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mlybgrxr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ilybhkft.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mbgtsftx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbebbeh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3trndonay.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rzywuryu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qcudvmsw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jhnwdrgr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jdrgvmut.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cviijgqa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nibdtmgj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3zpuzevrc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ooefrjwg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lexpxwjk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3njampfyt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hthqdern.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcpdjwiv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tycfuiey.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hihfrnuv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tcyvodbc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cvomgvzb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3izapdwts.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3auscweks.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xohuuhku.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cnbdtzyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ynynresw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eqkwfwwh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tlrsnivp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sppoqiam.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ezbwizij.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yifgbnbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vjganlil.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwrgin.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgtkhnhn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyfqscyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3viptxjhs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cwzkacmc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkuucpks.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pioxxatd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qepqmejn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oiaanktr.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwthlaxf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zuapbxxc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wxzwigyx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vlhnncby.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ckttoasm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ywbryoug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vepsngms.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xmwjrtxj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nzrvfspi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pcuinkbh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lcgbptrm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lhwhxgco.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3aaufgltb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ssuhadvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cajmpwam.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3skafxmiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxebyucy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pyrmswof.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3abyoouhf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3sxbskshl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ebtyhcdn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hrnftgkx.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3crgtxtvk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ezqfmczv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qiuynmtf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3mnfcsdix.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xsvqvmqe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgksaugn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lenslhno.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtphreor.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3uyspxhgr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hyhbfygh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fqkizqhf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uyykpypv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fbybeqzi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fmeqjeof.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qkwwdrvk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kvogrrrq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3fosnsusb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3cppwqzkm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qqqocpgk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uprmfnes.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3okeftuql.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jpiszlct.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zxtxwjen.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cmtevemx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3snqkwliy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qqbejmpq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3voorvrak.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3spqpcatf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3omnxwtgp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wlmrgbja.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nsyiltbl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vezhvfhz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wvwasvbe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nxzmhtgs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xvthcltg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vowssyae.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cibayiwe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mklbbdrn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3aybubani.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nlpltqbg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sneewduc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tyriuyke.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3snjgwmfj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3omjqajfk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3riziaths.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nmlapvhx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lkhgboke.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pjlcwwqo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kwtonafq.html


<!-- 参考信息 -->