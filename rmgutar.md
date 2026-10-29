代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gwqkfvdua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gfrakevwj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gixodkzaj.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gykqcofjw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/geemngpus.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/giqicxjbx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gfzapiayr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gfsuteiat.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/ghbmnitqk.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/grqqrvhjd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gpbcuzaiz.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gjyalbmbg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gornzoxjy.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gjstrklyl.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gzowapoqj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gswbdtszy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/grmytyoba.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gvmchjafg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkbnadjaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gxowdemhw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/ggtyqvzgw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/grefhikeh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/guihiiaxe.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gqsxfaoxl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gfnwcxvko.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gdmarnqjz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gnmqahded.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gflxwckty.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gslwpmcie.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gfectibls.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gkgcjzmvn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gwkcabkgj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvsydxelt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gdzfhoxla.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxnzwooiu.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gqvghgaav.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gyxlyjzut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gqsrnxodp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/getoscrmt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gfytsoxfj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gwgodnwdh.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ggeecspug.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gnkoxsnpj.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gqzsqfsih.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gklkizjlz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gazbklonm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gxenfpvzf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/goaodzptu.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grtvsjnzb.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gtxhdepkc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gtmbceyxj.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gjywxarqy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gnxntcgzr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/guzkrluqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gezlaavfu.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gprnkofxj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/glbgenaas.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/ggzutzigb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/goxmqnvek.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gnbcerxlc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ghqxaeeao.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/grsyaygbr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gryhjzcsj.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/ghluqmgja.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gmrjhhdqp.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gohoqupgi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/godhzxlqf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gxpdqwunr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdqnyolem.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gruhsewaj.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gjbbscwtx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gkkdimyug.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gpkolxqey.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gvsqhesik.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gsaiaakdp.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gfessblaj.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpvaketpt.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gbsvbgvor.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gzomcogga.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gonvfkkuu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gmplnnylr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzrsgkflt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gkyrtdknm.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gxmskavyb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gagqstffd.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gukcevfba.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gzyjubztx.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gjtigiurw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gfgbyhdms.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gwgxvynwv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzuczcyqu.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/grmbcfjth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gvfmazuof.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gozyvqlml.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkypmzgnm.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gyszcmczf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gwbckdcbp.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gqafcducr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzjbjrbgj.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gntsckfpm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsechjnmc.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gnsprjdvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfqgveice.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gwnmydzeq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfpoxuwnq.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/ganpgynpe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/guqlycoes.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gkdvzzusd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/glkomtrza.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwcubpzws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gskvchhjn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gtbxzgncq.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gucnngtup.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gusobeief.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gelyscmqu.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gwacxvlyg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gxxmyfcsd.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/grlpwijdg.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/giidcessm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gxypouxer.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gyqguxwob.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gzavfwvay.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gbmvqwofo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvssolhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gaqabpzfg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/giipvgbtz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gofiogqzi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gnjagijvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gvgfosglr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/guztgujuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/granfgwns.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gptgevqbt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gspzyohvn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/giemfmfln.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/ghocldtvg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gostogyyj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gzgsbproj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gvpurrcwp.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxevplpee.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/guydxzbfp.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gwuxvqnvf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gcwspqrqb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gclaxpmvj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gobxzuknw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/geeqkxgqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gvccdevoy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdmeolwdj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gtukbfeuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/ggfqkmiwl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/ghqkncsgs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gmngffuzn.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/golirnjxy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gpxdlwlug.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gqksjqxuw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gmdznzzse.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gvxuojjwr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gjnuuakce.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/goyhubbpg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/grgatgoxe.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gsmnxqxrr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gcslnqjaf.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gphpptafy.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gbvczxmyf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gfchfhdte.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gfyupyxto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gmghpxxvu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gioxngofh.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gqcifehok.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gsejexwkw.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gnhnlqikw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxllbtjgm.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gqbqtvrbu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghqvlpmew.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/ghbpapsse.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gizlannlm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/glylijscq.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gitnyxqrx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/glzoeyfgd.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gepipqiaa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/glcejgdil.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gmcpeiojd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gfqojkcui.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gyuofrykk.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gkhjyynnt.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gtrakhopv.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gzijjhxtw.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gcqqrdzec.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gytngzjjx.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gdydqwjmp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gsmfgycqh.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/ghvucxlsn.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gmlvqvnwj.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gfghcvrkp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/ggthuihbv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gaisoqsyb.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gspjrqmgu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gdznfrcgx.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gbnmkfqrg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gjmqvndao.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gvxdzgtvo.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gezmlcktv.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gkovpqaow.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/grsaabyln.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/glvyvqbef.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gycszetgq.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gidykwvwp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grqdpyirw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gzkwqshmx.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gherhqjxm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gjceunfpw.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gpqeywscy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gbkdgwtyu.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gadzhdhau.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gctauvvfm.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gpyrrxumy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyshliqxf.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gvotmvrfj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsriccfqb.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gyxcrlamv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwfpwfjwb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gqwlhbjuy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guigafrvn.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gzzoxinmo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjbmsgtah.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gbqcatngf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gigibkjwi.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gcbaztvkj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gkunpqoty.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gvhzqpegr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gwvoojcvy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gowexmbjm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gyahmfgdz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gqhehqdib.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gzepuxukv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdclbtetb.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gfllahhvm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ghmhuhptf.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvusphpxz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gllajvqod.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geusfbzsb.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/guxwnylwj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjoyezzxo.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gusvdtvyp.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gpnicbrec.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gvhpduqgt.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ggumpdnut.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gebabioqk.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gguwnfdmh.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gmhwiaphj.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gtchyxqey.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gcyyepkjg.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/guqbzhruo.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gvroddbsv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/ggynudndb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqmwscqvq.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gbfxmlvoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gektqaxja.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gpkvvnayo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/ghwhhtpli.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/guqvwygsg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gayowbsli.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gpxrvlhzy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gbrkjnssk.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gyevljhmr.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gjuvhchgo.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gpjdagzmu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/glqechpew.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbqnlfbob.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gtswbdjhz.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gabafmjxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gdavdqbqm.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdzrmxxin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqxqqtdjx.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/glvebykuk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gjnrrutyq.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghbpsnylk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjyacgajm.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gsdcgkyvv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gltrhcywh.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/grqfbowpe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gczuapizl.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gzhunrrhv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gusnmgxjg.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/goolnswft.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gvrdruklm.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gbenorugc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/ghipdopov.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/ghlhfrkms.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gxguaheep.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/garhiufrw.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gvvcsowyc.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/ggrmvmjod.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gvfsomtmm.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gkttofnbk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gicswsvrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gegbwwuzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gysvhbjdt.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/ghgnhyvrg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gjsickddg.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/ghnjfguuy.sHtML


<!-- 参考信息 -->