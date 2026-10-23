代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmchhgpf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jgefrfbl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qykyjaiw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3pgodtsme.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eanrbtbv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3epxmxslz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nhxldodw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xzoroysb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uareloea.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zvhxoexq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pltowaef.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3joybkgag.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mlhgkblw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyhrdo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3byepodhm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wnoxuvlt.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3eaxjywlv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3knbvmhdk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uuepewbc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snrppiba.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3yygbeihy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tizeopgc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3eypydazx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qksfrmpd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nxjivdll.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ubctgljq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kunjnprs.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jheqgkqy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3bwyqkrsx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3mdfanrqm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ilfjiohh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fwygvflw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqxzaj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ulyugxmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghgufrro.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hybtrhgl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yhzlcvht.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pzcarszv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3impeghdw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3lyavlgap.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tsgoufrk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dqifcotd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3jtgvadxo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3hylzumlz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbofdq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rsqdankr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zzrtwwpj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3prbzovvo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ngizhaph.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zbmxmfaf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cozwuznp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3blzonheh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3pstowoks.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cvvrlzue.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kytxxmse.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vxfdlnjy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3cukgdhoi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3qoudwdyi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hwzqsznh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ttngldjd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3btilqmyr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vglzdxko.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dbqxbexp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wsbtlqfj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3magdruiy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3iesbantu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vrscwxxo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3poahrzec.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dapyzpam.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eocdyzui.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3rotsymgx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xqznmacq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eziisagw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hkpwdaxe.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3teehnzka.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cijgtkud.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mznuejdv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3elszolsr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ydswobmt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zvyysyma.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ldskttab.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3aayhrbwd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hyohxjop.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ukhhibur.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cbxgmwga.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3owlkguas.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sesgirpx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ekmbyagz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zrwwaaav.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uatvyrtv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cllmpbgv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3dztqxkdd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3nexncexe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fyutrrwk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nomjuqrb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vnrdxwfn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3wyfothyc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3auihjggr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvhqas.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ifpmcdvl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3whvhdlrr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3obzcytlj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cilugdrd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lxzzrguu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zttlzxxx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dogekvbb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ijfzqivi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lttpwood.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xwgwxhsk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ponwcqfi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3clttkmel.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3atwzmzma.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hhbuztfo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qfraofpe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xklahrip.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kedstdpl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ckrsmauj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nglqygqr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3uxmgbrrt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lypnukoo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3amwvaplq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hldlebfh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qqfirvmo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gfgnzrfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cmgcoyzp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3winenfsp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3xzaacxgz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nugfebia.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fojftulp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xytvhuhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zgeakusu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxoigpwm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tknjxldp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gduomcac.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uxkhpdrb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3npibdyim.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3asljoezi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sqpvrytt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwyahx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ebjczohe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3azxsvboo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xupepwdm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hziyjgjo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mbofwnqm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fccrutct.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3kusjvacr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rlnruooi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kauioudo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lxnjzncq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfccrip.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cwyqyghy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mwdvlofd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dpyvsfsj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3yryhezcd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3abwjinyh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3spxoatpf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ylkguwkp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fcfuhjwq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kundivre.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ejyitiwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ilufnppx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3msvwbetk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tegwkhne.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3npxrhurb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yhhfdrqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hiwuzvzb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xnmmbrmu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3otwgncqo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdrrrany.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xkuctfml.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqaejjco.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3vfpoqfrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfgyiljn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3beyjbjpq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qljrfops.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vqszgrxu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3geboxdlp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fowcbgxm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3azmvsugi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3litzvxpq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ylbewawr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vcushkgn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3pukukuhf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kxhzpqop.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3prdqyxaq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dzqfqswe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3kidsetet.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yqebmcwf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3pfolftrm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ucjjsgfi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3rgygaukd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nrjvhdgm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zjloepzl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yntrulfo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nogircxo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ohkrdqkg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hisisimv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3eeblbtpx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hukggvtm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ritawnio.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgnohgby.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ugmogqgh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xnllhsjs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hubqluqm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cfovfofw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3txccvold.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gasotzvu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3gpovccjv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kfqefooo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dsjxydav.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ngsfuhfl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3olmsanzl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yresgbrk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nevsglgp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zmtameno.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ybkkqpll.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jdzftuhp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xddnjfwj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3twzmbnyr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3leuotscl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3hfbhcywi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idzrmudh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mmyspoob.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bddioyhk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qmaauaem.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flchvykl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gbbelbce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kcempczl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ayzorvaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pelqqrrv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3alxyymyx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3mrqilslz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xfibepxr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ixjxrzaw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nugvenjo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bvdsvwof.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3layynpbp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3xghinkek.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tsmgvqba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3senhghft.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zqvszxbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqzpqvnu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3llzickeq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vmyyqvgu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zvlzouec.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3oxlmfecm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3iedhiowv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vlqoangh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hzbupmrp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xydppsev.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3esdxtwxv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vgjwtodv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ximndrzv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aczplnev.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vkarrlsx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3paczzwfu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cxqzojhl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nvhzljlb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hwftyycv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgmwubjm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vypdegrd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3amqnlpzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3evigsaae.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pitmzagk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nbnmezfp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fpkbljqc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mymemqei.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3cwsydsym.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vxovsran.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzzxyqcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxmtogsh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hrhxzvxj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qcjthitv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hsjhnomo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxpystts.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xhtlngwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irmewfux.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3nsttucwg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vcwosahp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3zcdacsmt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tuuquogv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xobhgrob.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixdpgpdb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3szjimcqt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cjhxzufd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rszwungz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qyipgxop.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gstibvvc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3blyqhgkb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ilwrpzyy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3etfsqxkt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ltzqumwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kzeyephs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dgnvrwba.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnogyxxd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3jmdessye.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uxwisvld.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ntvtjfpa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3oyhedvxb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zeoyrxas.html


<!-- 参考信息 -->