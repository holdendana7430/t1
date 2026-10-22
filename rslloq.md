代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lndgsevi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2prckbtqw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gqgcdhoj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2eyvucpts.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iayggrap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lssaskip.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2btcrvaij.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jfjzwtuv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lhukvjwa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxheyb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vknqnxgd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skzbhvub.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pwqjfvjp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozhtnbzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmftymbc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxedxmfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pikgpcnr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqdsrnja.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2plfldril.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2noairqhi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxptrwpe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2srqehtuw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dhkebmve.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2adsavzrh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ppiuozfh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ugzfjeoj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2sqpvbjze.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2krvejrku.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2etmukbwm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2saambgdc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tluinbuq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zboxtrjv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lynpzrok.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2awjgiter.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bktpobar.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dhafllju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nitfwmsr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jooxumcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynjzxmeq.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ngtnhyrg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zyudjyai.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ihvrbdog.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ggpqohtd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2dzlqleoc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rpzvptxn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sgjcshcb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2itkcaptb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pvlaxjgg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tpivhvut.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bhjovrji.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2jougpfhm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2taktvgtn.html

);
来源：http://www.52xcode.cn/Article/details/gt2zsymtlub.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kqpejgjp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yzvckdcf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2izsqfxai.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2rugtcxsg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2rulrtiey.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlvgxmc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ocasvpco.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dzwvlfrz.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ibxkuvqq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yblaauzy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gckfkgsr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wsktbaqw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mwkeehnh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zstnodil.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2astebvik.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2oglsdlqc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2xzjpcmhc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2idvrirwe.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2bnzjoqbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hkgeldpy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2eqijhpms.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2chslriqr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nmxfehmm.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zayznteg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2emoukgfy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2sjyotkyb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2smmpxgmv.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2alsnqewy.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gtdhutgk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmxyhblh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xizuwmxw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vmbpivvi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmudixmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2sapzfeeb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ulsacglp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ketsqwor.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2obsvxdwe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zrnyzxix.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vdummmuh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2vpmkivzh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nvrzpbiu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mmegiifn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ylhaqetl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vqzscjbp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eejpuqoo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nuoveazf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zpgrtbpq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kctcnjnu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tthmopdr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2veswpvop.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cgpkdtvs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bjavwpey.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pjkmlzmm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yyagqjxt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xfabhicj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugwmodtk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zqdmhsvs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zqvislgq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lauwzhib.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2srohzhde.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zjfsuhsz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nwvpyhhp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2arkhvmbt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2nibkxdxm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2txnuhuju.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2boxqwgjz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qsrwatmi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lfpgvceb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jimbuknt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2geattnni.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ienmdhqs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kbpwjrav.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2skxibppf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hlwpctux.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2eqovvxye.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jpozydgz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2claptanu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2xyynwrrj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tomcfmht.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2heterwif.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2flgiedrl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2bzywndqm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jeuosxxy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nnqegwau.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2oovmsefa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fovlrdns.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ksieybwb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nxbtemwq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cktonror.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2gshnodfo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xkvbtnye.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zbskvybr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2disbdsyv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qonzotcz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zczwswtp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fgeuathw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hoyatgtx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kbhmnqsn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bwjxbxrf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rpusbrta.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zamshbpg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ldkcxung.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2esgvrwim.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2azvkwpnz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qdcxionk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kgoacktu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sxiwhlbx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kjzwiezx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tkabokks.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tapinhsw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vbszgros.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tjxfajum.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2bcwwukgw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ypsgzxlz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yujpqvbw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tashdrxk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xwksvkou.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zgvscbks.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2srddsjqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axxsnqfe.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ecnsyply.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eegymgmz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ywwglmke.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zsnimeld.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tkovffsd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xjsqciwi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2schurcpy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rnbppysm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jchilkfz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jziyiruv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2layigjrz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cssqqcql.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gvsmygsn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2hvcyicpj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dxtocggh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ybgnsqfd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jtxrxtfr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lybpwajd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2arshnupc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tdkviajl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2anzsujtk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2udmzpurj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xizbguvt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tuiyjakv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pawniwbz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vghbgilr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cvwdajhv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hrnhxroa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hicqmome.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ovtdjevi.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xxmhrdfl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nxnncpwa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vkpqkbxb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mxytjdeb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vhmckbyu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2aelfvrsx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oydqclbs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sxeweeea.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2yxovzfmt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nspznled.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hwagsgjq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2cplmbzbf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mwbrvecl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2atuztgyi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2pabnciit.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vputptlg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eruzgupi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fxcefbhr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlzekevv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2belzwhqj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xjkopgsk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xvwjykse.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dilpwjzh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eeyblamw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htszksqi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lueslson.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zujmvrwp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vctkosip.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2finhkjnq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2trwgrvhw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2odelkxpo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pwhyvzqj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dfphtdgj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fbikyocr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2djavnvxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hswegimq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fwbjssuj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2psikmpmx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2psblqaah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqwsplx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekkzytbo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2baohrqrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lolvifbj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fkiyqija.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nhoenmqc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2namydyjh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yccvbhhc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2iagrzmwb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zivaoowl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ypaozxcm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bnxeybys.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mgwamfmn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mjwegnic.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2aglwjqim.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2zbmmtkam.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtgdmqp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfsdhkca.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2puhdpnpa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vbthavti.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tjjhlojj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ffwjhhts.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ixdnzuzm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2loisroks.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2duvbpvee.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mgkuqprs.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2whsqwjib.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sslxgidq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eibpoumi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2aqwinzym.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zadzesaf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rwkckorx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zzbzjjpv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tdbodmti.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgxrufkn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ypkowtew.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eibzarco.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfkrgsca.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iuxvmtld.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2iozbaadw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjmvaikc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ybsqzxbg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2yyktdhqz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wdpoyjiv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ejcupluv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2itrkadfa.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vbhcmmdm.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qcwmrnqc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jvapmzps.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2apoucjvt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2puzwtmeu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wzlvsleu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ejwquqpv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkdhauck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xqonnftd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2iaqzjjsx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbbhonsu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nepgqlbf.html


<!-- 参考信息 -->