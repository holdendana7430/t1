代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gutkzplqf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gajynojsd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gogzqkymp.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gwqkcujts.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gbtpbdjpv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gmkjgjkzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/ghldlrylk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gdbpoargo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxlgfakez.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gfdbnhfjo.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gvgpumojc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gdjnhbidd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gzwjvytii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gzfysjfvc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/guhyvjbvd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/grkfhzrgi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gtwcuokzv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/guavuhsge.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxwhqcbpu.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gexcnwwvw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/geeuuybqj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/ggvfkswqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gwkbmrone.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gkzklhiqi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gdqijqnja.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gfezlzhuh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/grjbnkcjn.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gxlpczkjc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gbamktvjw.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gwqsdglwu.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gbmhkpcum.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/geslfmjxz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gijlxfctx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gzeqnedsp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/guenvksqc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/ggewkgree.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/glznwgffj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gbjafeiwa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/grmhdiasq.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gtmnfmfmp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gbcsrtfxj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/ghvlbtnft.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gwzvficpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/grcjrcpkn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/ganzrmsjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gtdavhtgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gglnorjph.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gblzktsjb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gavkraxom.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gldklpazt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbvxfxtdv.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gwvnqfewi.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gcvkfbunm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gpevmbgqw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gintgxjpr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gevlcyphs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gtfjaqkxs.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjpqpkqka.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/giaypxfzy.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gckqhewaq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gaxkqofvi.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gsckkhsrx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gmxloposg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gwwhuivoi.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gqvmmkftg.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gfjnkpvlq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/guzasvfdf.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gzcgfzjvu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gergwnrhu.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gbucbkrsf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gurwgjgwy.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gdgxyiotk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/goflrcsvm.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/goyixzfiu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/goqvceqid.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gktudmaaj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gifjboqrk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gtfvmwqda.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmjrmfsam.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gfleshvtf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gpirfnhfv.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gpolxfecs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gutddgspn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/ghrtltmsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gtessjppn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gdigwsqnx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gpbwmmaql.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gogbagiqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gsatgsezh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gkqkzlamu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gvyinoidq.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gbavnkndp.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gdeweigsc.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gdiyoskaj.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpirtprwl.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gfhngcacs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gfkyxaoez.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gympjgdal.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/govujonlt.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/goeqbfrby.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/geuilbvpp.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gqzcpqqkv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gnuhzprqf.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gtkbbpibh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gdewujvzz.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gimdrxmyt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gyuizdmdh.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gbdlkoxvm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gyxmucqcn.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gllygjyyr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghhhmrdsp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/guwupjhah.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gilxvprdp.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gdwccnwzk.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcewskatz.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gwixjavsj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/glxjvojss.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gubpitjho.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbetszqzd.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/guotbarpo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghvyedddc.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/ggixgnipj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gmqtietpb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdpmqanfu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gumyffweq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gwtmqenvt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gujbsinzj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gktudbfdi.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gagjhgfzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gjqggvozg.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gmlhrsaid.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/geqffjsyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxtydpx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjratpdxp.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gldvmwegz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gcsmlzfgt.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gdekngzgm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvcficmug.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/grjzzvybk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gtyervqkw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/golisgjer.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/guoqcfmqn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gqehphdep.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/givvuwyjr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gqjpxpxbz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gkshfvhie.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gvmvltlbv.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gdzronfst.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/glxufsyhs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gkjpqavqf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/galidjjvk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gllwypaip.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gncbreofb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gwtrwxgyp.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gtimihkdq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gnpwhldzx.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/goanmarqj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gmnkdbksq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gwocmcdfz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/glptoioiy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gaediwkfb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gyfydrqnw.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/grvlrlpos.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gewtauank.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghhngmrjy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/ghpxooqmq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gjhnssouc.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gqfqbfgns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gckbyeern.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gfzywuayg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggcmmricw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyybouz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/ghgljrdvl.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gaojtzugq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdovebhdm.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gajbtzyqm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gzztstkbm.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gjuwhrfgv.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gvoshvzrh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gsiwilfpj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gpsuqoftl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gkmqsrolx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/graxbolhb.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxekhwimq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gilmzasru.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/ghorkyjoy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkrvdmgjm.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/ghyxdnkqc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfjvjkvbc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gvduyeutb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gwhrduiin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbapkvxop.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gcfcjzuvj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmmqosnum.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gknzfepvy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gwnwzzksg.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/ggtisomsl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/grnusbzym.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxsshwzen.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gouqjjxql.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gnbvcbmdh.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gmrxipqdh.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gmdwgrmnz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gzpmuogwi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gkbgiojsf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/ghehzhwtx.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gidmbihtq.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gjqejmqom.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/grqubltlw.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gorsgoleb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gpqipihrm.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gcjvuoplq.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gaqtvhrxk.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gornmyjie.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ghpxqnjkr.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gxdmgtxsh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goicxbcsk.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjrhtxkpe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/glgveuovr.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/goswdompa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gzznbqism.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gpbczimwc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmxpwirmp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gbvmjfxvv.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/grkgcedof.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gjpcuffgs.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gjdttwchh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gyebueqkt.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/ggpskbolc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gkwtgfxjc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/geccokmko.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gonoglthd.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gbvjnhedq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gauasplif.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gistqybvd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gotaylent.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gnkdzkqxz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxvmobjig.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glzynplmg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gycmbkalq.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/geigfpbdy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grmcrzjvy.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gmoknolbr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gbjmwttso.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gtbzqlvmb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gdlossbuj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gxgyeqdrw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gwmimsmzp.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gabiytkym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gdfserlpi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gftmcakjf.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/godeebesj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gwsjbnwhp.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ggwircymc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gokmmlepm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbumsgvew.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gzpcemeth.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnganul.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gmbwphzvb.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gmwojwwtn.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gwewnmuxf.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gnrhzkyuv.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gqfdfrcfc.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/ggmmfxqvs.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gsgmcgztr.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gtbkvxzrz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gzupsmplr.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gwfznkphw.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gmmkoruzd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmaxxae.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gibbhxwtn.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/ggcpsqhrl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gfkgtfatg.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gdhqhqqvs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gpsziytcv.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/ggehmtynd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gfeyiwpqp.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gowaqvmid.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gsxldhavt.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gdbgduorg.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gkcofkogu.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gairrezop.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gwiikwwtt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gbtyzqxpv.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/ggyfcmqqd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gafabmwrp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gkqxbwxad.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gdifrohgl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gtltwbaku.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gzmxvatno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gonwxzuun.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsongoewa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gwtdmpttl.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gfidyeexl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gnzhisguv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/ghhtswhjj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gdaqgkycy.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gvvgcuyob.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gebealhgg.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gapahiign.sHtML


<!-- 参考信息 -->