代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gzusrfnxi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gjhtadavs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gvzizdybi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gfdeqdamz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gyrgjublg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gjpuajovw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gldttzfhs.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gdvmxlxjc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/glmagjzjs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gaojuxmas.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gdlbpvgzj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/grsubvwgo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gxbbnlwkw.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/glajfiwne.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gnkvrjabq.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/grtyguxbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/ghcydeizi.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/geqsbbbfc.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gjpbhqvun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gwtnuavjb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gbqczajsp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxpxwgjqf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gbyimbact.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gguipgkaa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gqawssixk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gjkyedwwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gqkrhdbjo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gohlwghel.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gmdtquibz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gavjxnwrd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gyfowfbsr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/giwxerzho.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gactguygo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gqzmsybaa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gtmtpktad.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gumnypkip.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjsdnfuah.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gkjibrtub.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcphmalqg.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/griafbkar.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gpnmtxhmk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gfpdmeekf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gsdzanefx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gwdiloanx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/ghsewupym.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gkplfqvcn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/godtltmjw.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gcujwylza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gjbfvdtzj.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gvrnksmos.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gkqymkuvj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gqmdjojgu.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gdfxkyzfo.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gurkhhwng.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gefperrio.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gykhyreax.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gxeinxhod.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gcddhrbdi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gszcjlqic.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/glntfhvui.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gljfznnvo.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gjhzihfnq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gqcpjvrax.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gsjooghbc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gzmntsvqy.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gjtvxfrii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gqcnxsoer.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gggnyhnbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gejovxwga.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gnyzqheqz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/guiflemuu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gndjqkoxl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gxkdapjud.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gbwwgudaj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/golmoqjxz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/genfkokrh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gplelvbes.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gqomqvsuo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gdsyjatpo.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gxpoyokex.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjyuvusoh.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gkejauxvv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gplbocdao.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gfktgnrph.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gsmsustve.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gwirrxkcm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gnxccamfa.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gppetjqqf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gdoecpgsg.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/giuxmbsuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gebqahapy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gzbvbdpsr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gxkucyful.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/grshpxgnd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkrfgrbzr.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gzugtdnst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gygrasrth.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gnvvbxafx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/grgzyxcix.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/geolldsll.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gksyckfjv.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gceixoyzq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gozsswddh.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gtdrtjlcr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqsnfphic.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/giiahsref.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfbvlirdq.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/ggwwcrbss.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtyuazayd.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gdtznlvai.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gaofwnnxa.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/ggwkkytys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gnxcoyfrs.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbguiqhgu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjlltapnt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/graloabjc.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gteklhxed.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/govmstpnu.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gohiyriho.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gjmgwmjil.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gscqjclwi.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gliiymhjf.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gbxuybreu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gpxwpwoxs.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gooafpamd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gqwqkihwp.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/ggbiptbfl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gqbldnybh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/guvuvlpps.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/ggaiqckut.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gwmtytpwe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gnjyklqca.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/glrvhdeea.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gmpoumpcd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gnjisgxef.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/giwqnykcv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gzicsymxg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/ggznmwlrm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gymlgrlak.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gkowoleis.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gtxwosocy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/glvwmykpb.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gdpvdtlpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gldtuwvla.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gnrqfnldg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gpxokdtfi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/ggzcbfexo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gowzaqtuc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gxwxcnarr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gegviybtt.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gpoujckhm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gpighhbrn.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjjsrhmvc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gkbwvfjaa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gzkogrcyx.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/guzljwulf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gvlfoatvs.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gytozniqh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gpqmepqcr.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gzjcgkdpz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gctijmwlx.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gkhotyjtl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gjzdiumui.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gmoymhtug.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gnmnngmoc.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gihahtqmx.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/glycdupcz.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gciotpqek.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gqwajdhbx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/grqprvmmr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gyngvjzro.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gpbqwfdeo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxumxbxou.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gxfvcxulz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcbudnies.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gvwfywmue.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glojljeqa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/ghkjvbche.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gursebamt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/glykjfmph.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gcbbpzezp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gamugczrd.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gxabrkmmz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghihcrfyv.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gojohphsz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/guueuyqhq.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gijkpnkua.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gtlzczlte.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gkoflnaez.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gxuikvbtw.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gnhnapips.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gulfcrcww.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/guuryxrci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkpebrfnf.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gleqtvjly.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gcoumctvr.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gygorfvzg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gccresrsu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gmhdmrqfr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gekrsbdck.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/glqxighym.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/grqjgcamj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/geeyonppn.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/geffrxlky.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gevujapft.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gkmltqxrv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/grwpawybv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/glrsyuzwk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gkdmjxtvs.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gygpdlxqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gksfkuqce.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/ggxsrvskj.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/glwzzlkla.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/geeoxnnzs.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/ghqqawjoj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/ghwmpwbui.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/grtukhngx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gmrgqculy.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gslhnerwv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/geyugvaqh.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gejbcocii.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.hesvh.cn/Article/details/gusujemxo.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gibdkdznf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghspkitfb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gqbcfufsj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghidsnpuh.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gdbcjhxdn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvhwamqwf.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gjrmynbfj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcwmeahrq.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gtjsajjav.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gdwobqkpe.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gudwkjllw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gpczvxcdm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/grrazjlda.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gvuttpibm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/geluuixlq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gcxdlsmom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzxhhoxzx.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/glixdrqob.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gnufodsfs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gldclkatr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfrrvnyno.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtmthghrp.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gdaykilgl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gavutiyzv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gadwukmvw.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gixpghruf.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gritcqwkm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/ggkzlijur.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/ggnpngfds.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyzqcox.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdyrxswiz.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gyzsedojf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gqktuohjh.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gmtcbgadj.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gaonocmmp.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gwynnzeet.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gblowqvyp.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gfgdvaujg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfgszjrck.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gdezexkiv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gvixodisy.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbpgwuzam.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gjrjztfdd.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gozpsceim.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghakqmtea.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gsirhdzhc.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gwccxukti.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/ghuuvcevc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gemazevcp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gqcfjvwww.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gyjwxqove.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gwzrixxbd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/grcvxghhf.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gktnjbsbp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gpgudgdze.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/ghhwnwocf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/glvnhaxzc.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gnioacozq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gwjrvfowl.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gdcwjzyom.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgzqply.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gxuirofoy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gfdwaquyv.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gxmoggtnt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gzkvaknjf.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdnmitd.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gqlicinne.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/glxybxetx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gmeutyzhz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/ggshtbvcs.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gohcbkxpy.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxspftkog.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gextjbycu.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gmrplcqfn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/goguxktth.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbvuassuu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gdzwvxmoe.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/ghzxgdmuc.sHtML


<!-- 参考信息 -->