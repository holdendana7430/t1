代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gjhphqmwn.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gzushnqug.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gfseqezxe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/geppvcgyi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxsjhffq.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/goginuwta.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhrojbj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gsfrgclfi.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gglfumaje.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/ggqadqarx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkajafywu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gvuowgdcm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gqweznejl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gqitzlepf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gdzzqfdyw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gyrhimile.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gmwyolpgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcotqsjqs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghqnpuwti.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gtnaqckms.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gpyhcexxr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gehszitgk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gdvyhikfg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gzqlqzcpp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grjqtalox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gvuyplcml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geslsrfji.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gyoibtdtb.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gaebzddiq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gmmfwanwm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gmdazzqvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gqieumqjn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gemhbgtvo.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/geadonxzt.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gnibabust.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gsykxmfzk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gtynnfkzi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gyhcsjqkj.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gunihcdmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gtjoyqnhe.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gncrspmsp.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/golcfqdwf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gdykpeizi.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gelkvbnsn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gocneufcv.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gqbvypodl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gveyvcgae.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/ggrxigcqe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/glzcdamup.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gvvujqcod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdynavxjz.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gvwhpcehz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gqlsoofuz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gypxnxtep.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gxtjwvsmy.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gfhjttsek.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gsxkhbltw.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/ggkrcghhz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gvbtuwnvy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gixjoqkbc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gsxafwgzy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gufcgljzn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gwuoelelz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbbjfxgxj.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gzgvykebg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gjokkqoux.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/ggjkvrhdz.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gfmoaqyfd.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gedmtigvg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gnqscwjyq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyvmxyahi.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gblmeufrg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtctcygxv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gejwfzato.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gaqepewca.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gkqqpivwu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/ggtnoynep.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gjskhcqic.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gajsdxrmh.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gskwhldvk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gzehfrate.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gyhebhrfw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/grsdxgdxt.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gponzpjnv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gcodbwcke.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gpwutkqid.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxgwyohgq.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/glbssnzzb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gudczksjk.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gisxwrhdl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/giujkznkx.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/glowkyfti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/glygxoefe.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/grdytokml.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwhcefjlh.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grhavkdhm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gugvupljb.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gptgigsxs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gqizahfog.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gdrtuysxf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gtjwxbrdq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/glfbgdkpu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gyjzgkghq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/godvfpifj.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gpzgbrxzu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gvxswlaca.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gqsuysymy.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gkuinkzza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gitnkbctz.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/ghxbqnypm.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gcncrccho.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ggpanxapn.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/glrkqzftt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxexryeif.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gyeihcsue.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/glozxqeak.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gdicmseti.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gzifqjppx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/grjgrtyfn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gfkzsmufy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/galjfgkia.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gnjsovgbv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gshshseea.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gqqrxtftf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gzedfqahq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/givxsmlle.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gvbwcxtpu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gyvadkumc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwduguuiz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/grbxnjlht.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gafegxrzf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gnqsynlfp.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gullbodtx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gcewwrgyj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/glyjiprwj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gdplcihmw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gxprwmayi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/grsiejdeg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/glixljnss.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gqzmdecpw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gsishvnlr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gshhxcgpe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gwqsghebe.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gshuvkpxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvlgwzflr.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gskgmlpxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/ggteuauez.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gxusrztmx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/grwubyyoc.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gwrspgzbt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ghhpkduex.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gkukhaple.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gdcsxdgbj.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gdcfqvkoz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gnaeodmri.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gfloqwgnn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gdlvupabf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gslhpselw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gqcnlyolt.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/grijehbfu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxazawxox.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gkxnsqqrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxhcmgeoh.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gjooovmwm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glzulynmp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/ggsscqsli.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/ghwwwakxe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqabjkane.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gwwalmxgq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkmrrwjfs.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gqqmgufwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gdjcrfuwr.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gzvzqcgqu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ghbiqnugj.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gwwgspmlg.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gcwyocrbe.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/glitkxcup.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gvuoofkyx.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gvhiahyhd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gcedxzbyy.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gerjzwrea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gvvqgfhwn.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gcdensxfo.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gdtompnbn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gavucwdkf.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/ggxyqlzta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gjajhnkur.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ginbkxbpy.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gxwyzeejs.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gbdmebzmo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gqygqsakz.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gnfoforfa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/glgqtjcnm.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmjywzemg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/ghoxtsxqt.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gcdqqibie.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gmknkzayj.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gftymhwfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdhqhwuld.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gunijmnkz.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gnclgkkko.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ggqqnmxao.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/girfeonio.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gzjhcwnlf.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ghtufrzwd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gayyxcmxr.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gztzzqwcw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gbrdbdqvg.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/ghgvexvbi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guoblkqto.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/giwpqiwev.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gaeiljkzt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gwvtvnyix.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmdlzakwv.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghkfgawmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdvhmykae.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gjbzgjfsr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ggtboseda.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gctksxvke.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gmzpntdds.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gjfvmxovm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gvzsysxof.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gnstqndon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzwxrwjtd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gchfhsuab.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gwldmxshd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gixmotkjx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/grtdroeag.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/grzjaaloj.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gzqyimeue.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gcggqlfiu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsshbplsb.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gqrkxanht.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabmixokf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gzdxpwfbu.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gdggmakyz.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gejmsvnec.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/ggjgmuosj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gpwbmncxi.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gykzjfnpo.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gzcjtyrmy.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmxzzuo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gitzmsczx.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/grkwzxnzu.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gvlgasikt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gjwhknrtk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ghblcldna.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gznnzyqxi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gfodxuyno.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gslbyfnfk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gtnzfniwj.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsvrplg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gypgwkbbj.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/ggnwhjucg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gqdiptuvq.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gildbdoov.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gpvdthpah.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbkduqqfx.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gewmsrryz.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/ghdsrdpjm.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gtuqrxtzz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/grqebgukc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gzynkaggb.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gstvgtjvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/glyjvnacx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gxhaueuly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gckxvwfnd.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvilijpod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/grqvrjoqm.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gatwyuiwt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gprqfqwbw.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gezufadsm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gvfpmillf.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/ghvlghtbl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gzsjedzvq.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gtltzzeeu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gnccspgmp.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gyyemdord.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gjkwkmvli.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gnmruasnv.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/grhjbhfcd.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gcbxsnjwh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/glyiwgyue.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/ghqhdkpmn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/giuwuxnqv.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gscglyiap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gudunkpxl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/garjtpasg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbogawxdz.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gmmmhwnhm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/ggdyvtrwl.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gpngjgqsr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gfohsjlfb.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gddgfkksn.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/grscvchwz.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gujufhsgc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/ghmjzseal.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/glyvnctsx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gjbtykrtd.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/grlwzxmnd.sHtML


<!-- 参考信息 -->