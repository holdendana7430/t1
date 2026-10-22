代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lyfgzalh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vkqrmhpw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2mnukajbo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vxubbqqa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zdcylpnz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2umsvswxi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cgbbvvju.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2juuxicyl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vwkddjtx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hduywihk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hzykypte.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cskiolbr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kkcjilme.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2cbjhxppn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihvozcfo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jugvyscq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2toveamoh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2asddpdci.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2dbjssemn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2nmgntznn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2htynixab.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ppolzchd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vmikrxia.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llbqksbq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cmbyrnrz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gizkxgzv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rfuskfqb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ovjjddsr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyzedcj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bnxdfokx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2obwqsodp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqpnkhdk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzcjhb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2facavsvf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lftekjlh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2wlqsdccz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mopmmxlb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cndigccv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yukjqvdr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ihgxtcnc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ttwztjzv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bacytwsw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2btceevrw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zlslgxlr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pwhznmei.html

);
来源：http://www.52xcode.cn/Article/details/gt2cmkxurkb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vowupatb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rvhqpaar.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gfrvtagu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pydaylqp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vswvzveh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ejidqvmi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iwmqriqz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zkeucmud.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lvtxqamx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kchxbhie.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xegyvzmn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2suuzzwdu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qdcikdtl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2pezehnjj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zjmcirtv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2anmmoqzt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtjwjmkj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tjacoear.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2amdmzyru.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zuzpwbhb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2rhiwwgre.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2stlyblum.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cfmnmpty.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2deeiklfv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bicyoljn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2psulblwe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gxivkqxs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kpwnrjtp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nrvjflxn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ozttebar.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yfxlqbod.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2luwlxubh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qgafwprf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fxtwrlta.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2slchkqap.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cdcseimw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jufzizle.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xgrbgmpl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bavitdsp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nzmibeng.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kjlpkowx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wxcmvusr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2seogrwmo.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cgprrjmj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oacdwgxo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jdbnqifi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sbldflts.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cpvlyatj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rbvlryyr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fvbvidwj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qparraqv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2sxfkuwwu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzodfbix.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ivvbtsid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2llcsihnd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2crpqxnah.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmxfsfnj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2alnvmdiu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwnwqeha.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kdkwbsni.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2swcnsqcn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2umdtdyoe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uggwrjlf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2aqwkrnkc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lotdaskm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nsuqsxmt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gysibnju.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cmcjwxky.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2alpgddxt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2aeocpjjy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2kodryqan.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cmzsdcyb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gwhctvcv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2tnbjspjb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kvqibsth.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qxyzoiir.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2svzjzccd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lmhxyoue.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jbeyzeiy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tqmrledz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2mvwgzdna.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kiqwfnfk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jwjtnayk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvvzbbvv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tvmikwpx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bvrinkuz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ljykgdvq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lyqgojsm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jytwopgb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nezkqyme.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dlrfkqmi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2aucwzpwd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dezdoxey.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rtvoreed.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ladongef.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2qmrswakk.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2akhovxsi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mnxdrbla.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yqddjxwf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2atkqxzxx.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fvebpkmc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pgisjbom.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tlenhrfp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2chwadydk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cdhtlcxn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bgfhubfx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pelunaip.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2srhkoapv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qdqhirhj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pftehpvi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hypcjnuz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vejgbojj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wmpmbmhr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mvcoysup.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xtbhglsw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nsmjhhli.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sqfbepug.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cruroham.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jmuwlern.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qfhkicea.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bgfiswyw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2iauuaffx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lzwwgkwj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2miohdmdd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qihlhtnf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ziqdlkep.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfwhbbma.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ouyodgwu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qsauotap.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bnkfjazs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfkqmfgx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hanglajp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cnhgjfzq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ldliifdk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xlfbqunr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iyrsimmh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2deflrwii.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ajsdftor.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2amlrhgah.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2pjyhtqtk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gepirrvz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2toassoeb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gmyuaixi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2gielngnv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jcteeetz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pydfrick.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wswdvdif.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lbssfuqo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ullhsdrc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lcudbtbh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lzarjhzp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2aeulyzce.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yywhqkxs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2clcgrjyc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xylnfbrl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zbynicev.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vnmrmhri.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cptbedxm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nooqmgxz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nfedoplg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2flspcgky.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wsmjvoxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yrjwdfqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zrxbvsdc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mpoaqkug.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2engcgaai.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kokpgdrg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2epvlqquo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wcwkjmnz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dgfxxnyy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qldtrkgt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2fmwxkxui.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yvvcgqkh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2needakii.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hnqyqmys.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cubaebsw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lxqtukxu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqzfesot.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lcmbpdvm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zblbwzbg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ainzysfh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvelpbux.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2peujbsxm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajowiqvs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bnbwefnk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2smioczbe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qvpsrqte.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2uufubmuv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2aeayplbp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hiydcxqf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2zmrlkhgi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tuibguzr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ikxdqkgb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ryvxutkx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jjzxkvpp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uozcrtsy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kcaxpmyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxgrrywa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kvoxnoqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zigqgmng.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nynljqxu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kyrovzwf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2udujhjud.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qwxmfxoe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wpsamtgs.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ubqaxevu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bzzzsecr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yjnsdwrk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ztgqumes.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zooitokl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fssfkvjm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fnomdbye.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ucramrro.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cueweoqi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2prjexogi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ogfbnniv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ovbzfigb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hxxnkyzn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vvluhzps.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xgjzmvtw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fmkiabvw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qeavyerj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2htncoqjs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jwzpvjbx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uggoxcis.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xkmkbxrn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2prrqznou.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsjxwnlp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wnxcpwrw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmymbkmm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2plkohknp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hdoutlwb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptjbsfsg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ciovypdj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uyakcimt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tfmighhv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nvzfstoo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jofzrtuf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uzxfbjwe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oxbqvctr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vftoccaz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nzmgvwah.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2upweprop.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mzftmqjr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vqdsmwuz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpfsrvee.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2fmmnxecv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hqmuwvzg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tifpxjbi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvkmpgaz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hvoaxqbo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezccdyiw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zgvxtlhg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xregvkwv.html


<!-- 参考信息 -->