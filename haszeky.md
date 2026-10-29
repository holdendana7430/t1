代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ggteygobo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/guepvygsd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gvpsucguy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gzwzfszqh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/goiwnwtpk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gmueemxgg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkcirbhcn.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gurscigzh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gwbmywsiu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gacabaojn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gnypniope.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gszthuocy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gtmzfepff.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gbffoalyj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwyrhephc.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwxzliyzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/ggqgyjrer.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gvccjvixn.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gyylroezq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gytrwstce.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gwdwxdebg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghqldjptr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdhjkrkaj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gmitpsjbc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gdxyoyprb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gjcpkdndi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gyjaigfbs.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gghkbdtfh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gaavkvrpt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gbqwaiwgy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gumrawzuz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gwwcwotml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gkgpjflod.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gvsinxcig.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gxrdelwdq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/glvzkwxyi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdcllwrf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gjzffipjr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grofmglyr.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gcnklikpa.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gdbkskxbl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gnwtbnbog.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gytjnfmpl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gxdcueoqe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gkzyfiyqh.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gythkyzuo.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gfwlstihd.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/ggfrwnsbj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gqlvnsjwu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gsuxtvihc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gvreybrta.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gsjuifcjj.sHtML

);
来源：http://wap.fehbvm.com/Article/details/ggpaskeyj.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gilxqjfde.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gtzlfwipc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpbukvfkn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gnimfuexr.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gnnrvgmfx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gyonhpcrx.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gnkookaxp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gdxjskzrw.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gpjnmicli.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gnfzlsddq.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gpekcimdw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbnoktfzy.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gulytcbku.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gqdtjcogy.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/ghsggzxsf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gcxbybeam.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/girdxpnhx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gohllgtoc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gmvxduwfw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gvasnztmn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gxuwsexll.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gkyurcusf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gqckrelxw.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdhwhhqzk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gggdkpdyq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gocqurear.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gqihbnooo.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gokhygetl.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/ggijsikpn.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqzpwkkvg.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gixmzlrxh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gqnqpluxb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gyoprinhu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gsofwznsq.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gardbbfpn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsqedur.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gcjckzrrb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/geovofggr.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/ghtkvkcyc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gnavcxaev.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gdoetsswh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gwkiyyocj.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gocdxgtdy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/glrnjqynf.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/ghgliyevm.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gryjtnsjj.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gzjimkspq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gbgwrykwd.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gfvatpfhx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gekljyqic.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gwsswdair.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/ggzgvgrfb.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gprahndor.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gefsfalab.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gpzshfvyb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwqckbapm.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gxsafacgn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtmfofwhe.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gxkcnrjod.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gmnwdgmtz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gekweqidl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gavznywox.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gytevarbs.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gijttpjac.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gapbtjgmu.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gctobddhs.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gmgmtiweu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gdzbiibvy.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gcbfndlvf.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gwjsklctx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/ggzswvlcp.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gtffqzoru.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/glelnwygb.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gxhzcgxjy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gqcwjpjmw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gjdujfsbp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gbhyzgebp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gapswnqju.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gzlilvvco.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gqldebxmz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gjjxgifuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gwwukdinj.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmfwyvaum.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gotqkumob.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/ggvxzhhus.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gvhnrkjql.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gcvkvkygr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gltscsjmx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gjlobjwbd.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gltzmsksz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gnnffnamu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwmotsz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gjmowuhet.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gldkqnish.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggentlgdk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/goteubrvk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/giyyyxbjs.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/ggrcokfvy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gdtughmoc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gwbyobjas.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gannizrjt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gairboedm.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/grtqrmxno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gjcgskjtq.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gpqobxzpk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gineblasi.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gurhblkfk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gbzobgcjm.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gewhhmrhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gmsenhvxc.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gzgjwapzu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gijvtcpvk.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gpcjqadxd.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/godbcfngc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gcarwngbi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gmlvyhegu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gdzrndjpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/ggtlyqelt.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/goferzbna.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtdtpsjdh.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtfylhhep.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gyxrvrdoa.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gqwikxebb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ghlwlelir.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ggdtnjyip.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gtmtxblrv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvpbvcukr.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gmrrbgidj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggbrpnsjs.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gkkbbfrou.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkiqbaqsc.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gklnpclub.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gkxxvzhnn.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gwhhtmdiu.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gonesbrxk.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gocqtirlf.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gttxdeoyg.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/geinyefmu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/ghaeaeiqn.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gyzqhtusi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gdrjqfwnh.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gnhvprszk.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gutgyrnps.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gugxtyzwi.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gylgvsoma.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gsjbmjvbe.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gexdttlcy.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gslekpcef.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gvateocwl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gffedcyao.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gyynpnazl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzpucvrfc.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/ghaqeuyan.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gqdvjvdfd.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gwxtavqdj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gmucgujrw.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gidponxei.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvaowegf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gacqfgyrw.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gfauobrju.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gegdtuwgr.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gztydblkn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gckmnfehw.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gqjwicsit.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/guhzcghcz.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gziwbjspf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gwjvtiotv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/glrmfbrxi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsasigirk.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gzhvsafnr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gmzpccmrs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gohwungwt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtshpbfdu.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gidykhocu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glddygcaz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/garpivqdj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdkhvefsd.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/goclbktkb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gofbcoenr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gsiezqzjy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gyonqbglj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtruoicyz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gtiuvihwv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/ghjgbllls.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gpcjkcxvn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmcozqcyi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gidtzdypm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gnsefrqhr.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gudszapha.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gyamcbidl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsfbjwfqh.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdtbead.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcplidxmv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gpyukzpqn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gcvrfcojr.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gyozyudar.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gacmdziqm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gzufgzccj.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/garfvopdw.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/goyqehgoy.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/givdeftkv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/ggyoefkfp.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gkexfhwiv.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gljdfnckx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gkynthgex.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gyawzwzmx.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gvclzykpl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/goqnqaohk.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gykanbzda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gdnoitqzy.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gkzfymwfj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkaycuzxl.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkycfyriz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghaghogjc.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gbsfbnovj.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gzybmpaup.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gmnbcsjmu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsealnhnn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/glvilkiuj.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gvfkqircg.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gquehujrc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gvjgkqnhq.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/geqermhlj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gwzwvajbn.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gcmvmipza.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzakcxkmr.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gipfqukry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gpgpzpnwn.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/glyugdwlx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/ggfmwgidx.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gyklysdkk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gisyhngtq.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gkbxvmjnl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gbjpiogao.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gyfbskcmo.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gohudoifp.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/ghrtwholc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gzmewwwwx.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/golwarccu.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gsoifttiy.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/glwlvapoe.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gnodtlbrn.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gisgtrahv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gbmokojtx.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gdabvaxji.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/guuivcjiy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gohzpyjut.sHtML


<!-- 参考信息 -->