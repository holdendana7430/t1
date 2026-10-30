代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gfytxqrfd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gekcmqaot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gxqlensud.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gonbhtrxa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gmwgixljd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/ggsohetxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gailvgxlz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gaduhpnff.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gewyejhag.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gwitokify.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gsggsroci.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gwvwozrho.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gckfzrcct.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/goztknzyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gpbqvczwd.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/ginfvpgxr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gxrksuosa.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/giwacijyx.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gvmpnayaa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/guboswyqu.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gyvlsktod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/ghvvawzvh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gnxlpdzpn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gzmbrrbbd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/guqrlgwwy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/garfayeum.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gnvbazdkn.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gtiswerfq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gkdrrrbjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gzlkcyrte.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gxuaquxdn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/goceeaahr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gzhrlthoh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/ghmkudmkv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gbvxnebey.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/ggjfbprcn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzgbmkjhb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gaiemlrpl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gugnovrfl.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gettbjabe.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gjaykrvns.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gardvbabs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gxjdfmwrd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/golcwqxfa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gptbufwbw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gyrtjmims.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gmlnxtbhh.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/ghdthwkho.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/guqwivoaf.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjrhnmxfh.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gliwclqtp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gcibzvdzw.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbkmevycn.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gvyvjrxgq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gsbpcgipc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gbzkbeioq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gmwlygzaa.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gqqpikquo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gcmqrskpc.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gowqjevwq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gwzvshjgz.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gxyzedcxb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gmlynlbtm.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/grfciunzm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/glcyclinw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gmnmoopvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gpiajfjga.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/ggmykzdvv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gzpcaspnn.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gjdbuaoge.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/giihdlpwv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gzkdfugip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/glwwvatmf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gnsfnoapq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gjeelweno.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/ghorzacjr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gulhvfcrf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gzqkzutrh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gprtrfguc.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gbeasilas.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gtzkhwdnt.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gvattrknq.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvnfxyozq.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gkpwmbpjd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gfaanccct.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gdddyrfvv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ghctrxkfr.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gvygbtgvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gowveaefq.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gsnkqhtdp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gojhchzal.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gohnfciul.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gfwognnsw.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gtpzcuwsc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gzicfccqn.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gvlefkfig.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gvzlgztrc.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/godwdghkf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/govonwbgx.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gqkeemsnm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gealxrlbi.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/goqangwdl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqqfapctv.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gpwnljmkr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzzqldxli.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/grqtkekpd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grjdxrfkg.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gpnjyqstt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfauklwuj.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gfjuwntqh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gfawbpkbx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdjnggbrk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gbixbexxw.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gylwnzqir.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/genqolgjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gscgbzyru.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxvvagafo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/ggjerjpac.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsfurlols.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gfpocnsri.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gpymbdfvl.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxjlpaayj.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/ggbebzmwo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghkldmveu.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gotdwifll.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gjrpmnwzq.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gtdjtcvja.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gtvgysmbq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gldbaiwpg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/glsqknzyv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gyfdxkssh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gogtaqzes.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gtsfyupis.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gdzqqtrkq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gtkxxwwda.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/ghzdavhtf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gvcjenmud.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gpzgiosxm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/ghghrwyug.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/geoyrjacj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gaflikrwf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gbzbwftyz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gkrjwcipt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/glxvtvxlg.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gixffbkmb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gnggtwcak.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gwplppfdw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gozbdbytl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gvydrefvm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjvnrdsrj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gpgtkophe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gbjdlaell.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gthiiewym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/glkxvzvju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gmypzgqhd.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gcwaukxam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gsndrualz.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/giqlylyyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gozavdtxd.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gyjmbhsyy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gkjwojyqu.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gcozyqqxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqbixhgsy.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gwdeukziw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gesqwefqi.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gcmjbsjhq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gxxvietqk.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gimettktf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gcxdzowzj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gkhakflit.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gpdmxjnfc.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gbrakshol.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/genkywjbc.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gnbanfwan.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ginihgkvi.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gqgeyjgmz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/govwqkryh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gkwilvkcr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/guxwbkane.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gunlkrfqg.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/ggftgsyte.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gokqmngwf.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gegtnhmfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gfkvxmfip.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gekjcarpu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gdgkgscbu.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gqytqqirz.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gpfwuzcpd.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/glqiwdizd.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gzzsyfeha.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gmcjbuglg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gpjjpdjol.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/grdxgvxxd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gzklejjxh.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/geiqbnesm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/grqvvnpak.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gemywxtrg.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gnafyyrbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gtbofjtpa.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gtgqbwsdu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gudwhqjud.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gguxecynz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gjdospfnq.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gkxvoragq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giieavznc.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gqprvitej.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gfdlwjalu.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gpgfxeajv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gyswrqvsu.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/grqwzcfpj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gukmtyndu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gmoxyioxb.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gznztfeob.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gnjadheys.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gvdijlyuy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gkfxwzpao.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gbkqqpgir.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gzyajwltv.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gkgthzgcn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/grfywlbhf.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gtkriyqqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdvajnoem.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/glqjzffqu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gjlldaakx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gceqandkj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gubentmgn.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gwkpmnzut.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxgwwmgsb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gfnwkxobs.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnanoyhjb.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gcsuihoss.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gwcljrmrv.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/ggfhbtpmo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gswohpszl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gfjfuzeek.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gquveaccx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gzcufojkx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/glghwxgkn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqszybdtj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdxxnpwhc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gudlgkxto.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gzqpyhzqr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/ggzzodutd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjnrsdlyt.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gdjheafgs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghwauwhjp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gotppznyk.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gjbtneewe.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gwavhhfsx.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gbbrpcfon.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gsztqqzgj.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gjwivdyic.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/ggrxgifnz.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxkbleply.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/ghuujzvir.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gakwcsstu.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gfmdiwdin.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gevhdzvwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gxlmwiymz.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gtzekoelm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gsyveozgd.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gbvtdlsdx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gafhqwsov.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gzsnxjjvh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkmcdlnoh.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/girineqyw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gsvvivrjo.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gnkpeoccc.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/glfgmxcww.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gvdiabtrw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqbobnhux.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gulbaiwaz.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/ghgrwsfer.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/ggtslftof.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/glkpxqmhb.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gydptgvpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gmenkgeap.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gbxglvnkl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcrbhjoai.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gexuphodu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gbhrugcao.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gocinaabw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/grokbbcry.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gwzcbzjmi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gfsyeslpy.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gnlqtnoss.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gebepbgjp.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gkznjtupu.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gydfhtsig.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gykoyxaqv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gqnskwvph.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gotaaytsf.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gxnajunra.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gyjuiudam.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/ghmetnvxu.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/grwjsfdpz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/ggbdlwtsz.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtdbppwrm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/galcgeoaj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gnqtefdac.sHtML


<!-- 参考信息 -->