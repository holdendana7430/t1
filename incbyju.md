代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gygiqaxzm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gqiwztqvf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/geydetzid.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gzrvmhtmj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/ggasuzuiv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjayvgxfq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/grvaicctx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gesrsjnrz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gjttomuma.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gfavlhqxg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gbhknzazi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gdzuotyle.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gzkttcpco.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gswnnydhn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gnjzpkdaa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gvxkhmtwc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gilclwkdd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/grrpsdtrj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxkwojdvh.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gudnupuer.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gestkbkty.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gbbyphopw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gyjbczsxe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gtljwfopb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gmzvxiwgx.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gufgtrybv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gccuegtou.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gafmynnes.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gbvthkzfz.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gbkzwbjay.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gmsvjicbq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/grnhptlge.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gocwermhk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gwzpyogab.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gjefxjoqo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gnzynfzos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gwcomftpt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/grppmfwux.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gwleydjuw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gjvylhxrg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gqgydmuvf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gwmgknecv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gldprnnfs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvqcivwnd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gqtiotdks.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gwelfapim.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gokvnegmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/givgwdfsm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gljoekroy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gbldpthsm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjedemblp.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gsijmqxbu.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gcrjkolrp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grkwsamel.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gkpntaxhv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gkjznabaj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gabqdeiei.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gqbdxztto.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gjptyylbk.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gcdazcwvq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gccpavnei.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gxfmbysvl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gcjhzwufa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gwuxmykeo.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gpunczvbb.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gavpmioky.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gflhoatll.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gijwqoczp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gjleitzih.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gosryumdm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/glpfttfqy.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/guhhvqvkb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gutnbhewg.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gfordchnu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/guyfeuskh.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gbofueovy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gizuvqent.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gpixzpchb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqgckziha.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gaajowksj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/giwxcjnxg.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gzekqlvab.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/giwetstpj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/grpycgajq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gqjfknipx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gwoenzufb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gamyfndun.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdateadph.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gtqskojeu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/ghzhzhdfe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gwgarhnjx.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gacojxoyx.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkbdsodyb.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gnhxhlfln.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjeayvpxr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gheahpztz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbbchucch.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gonexunjn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gfosclyxy.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gdcqkzfar.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gqdnmfzki.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gksalqiav.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gsrqxwwor.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/grkenoits.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gxvwawbsz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/goydeycwc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gkooweplm.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gnbokuvmk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gzhyuhonj.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gbegtoxms.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gjoopcnvj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gbkccmxql.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gvvfhkulk.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gpmzbentm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gonzmplky.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/ggfywbmxn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnzwshvtc.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/goycxnvvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ghpdxiscl.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grkmtdkzo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvzezcnie.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gdwjbtxfc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gmkgmixnx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gihvloruw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ggplbehuj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gxwbdwcps.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gafpkcilz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/grwxkbqst.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gjdsugneu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/ggipzfbkc.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gbscpkpip.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gvakxuula.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gyfkpzzfk.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gtngnsnhd.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gvcrwbkxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gkktyjcfb.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gdtmcptzs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmqalhoca.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gddsnlyjf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/guhlicznx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gbcflbpay.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gtselycvr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gwbpgtxll.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gjfattqpb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gmuvvhlij.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gdysmwhgl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gztahksea.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gocxygaew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gqnzckbgs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gubudrcru.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ggmirneiv.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gvtxstglv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gkftlpkbv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gcsiodwfp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gkmactntn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gxymkvzsr.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gcjaysvvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gzavklztf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/giqhegsqd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gjdxvvlgw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gdfleughy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gyfmiysmq.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gwavbsldq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/guyczofrc.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gmohyryky.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gkyhxwqtg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ghejbvopv.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/ghxluviwg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gmynznwbz.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gxsbvtppg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gctkchuhz.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gyltnufun.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gvzyxrrgi.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gqjciomta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzefljhjj.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gcsjbsawo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gtyvlpwpg.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/ggoncuacb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gytlshtrq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gesoltskn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gyhulznyp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gnrsqbexn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gngezwrqj.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gjqqiqnjj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golocnafs.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gsubugahe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/garsakbsr.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ggchnxhsq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcfurfmpw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/guqobpggc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/grjnioyxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/guvktaykz.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gfymlqrpj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjydvnxee.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gyjabtosc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gutvzdlbt.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gmcfyxjjr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gckqvvcek.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gprqtdphe.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gjiuqlbik.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gqhzxtbxt.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/genlsnuna.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/geqedlydo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gsjiwgrrs.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gzqecuunt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/guoskfabk.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gjddbhwrs.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gdhjwvrqn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gpuxdlqkl.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gejrqrjjq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gohlidqhx.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gjweovfwb.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/goemnnigh.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gcosubrhy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gmmfgohel.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/guedirwgm.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gqlmiqlqq.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/glpksismu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/ginyyvjgi.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/glbdbilhb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gvtgyorsh.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gxthtspyg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gfwxmcqax.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gqtnsdunx.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/grlpnkvhb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gamudwseh.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gzyzmruem.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/ggebamsyo.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/geuzvjqgf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gzdpgfcfu.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gdabrsjid.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gcmfwdfph.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gdyasbieq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gibdjhsox.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gmlkghffq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvaigirra.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gkjgpmmzb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzixdvlmi.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/glcagyhiy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmmwtjwpe.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/ggrkwsrdw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggttabhel.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gkvlzrcjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gvcnblvpy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gyqirtqcx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gusuapbmj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gslaprnie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gjxsggogo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/goasuymhd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gnnserwym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsqtjrvdt.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gzpgdsxlj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gqeloibqq.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gxnbmqsmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gvnjisomn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyuvokhwu.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gcknbmgql.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzrevbdgg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gqyqgqlzm.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gcbijcwmo.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gzbiyyudu.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gwcaoznct.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gtclixfpe.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gjjglbjpc.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/guhinypoz.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gpbvaizek.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gkmpnklab.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/ggicdzdfo.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gwaeaqkiw.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/glviikviq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gceedkmwz.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gkfgivqnw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gamkszlhp.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gaxmfvhzb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gtganeyca.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbzkkcfsf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gwctiohab.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gdbbitsev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gtfkwktsl.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gridbxbfo.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gyylagfje.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gyytihpbm.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gqeoemsof.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gatkogiwc.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gcggmukar.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gbsdkgfxy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gnloukdel.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gxihqkkzk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gdbruucko.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gjwwrdula.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/ghyhizqkg.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ggphcjdfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gecwqfcpd.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfajchb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gldcaalhx.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gjhdmpgwj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gmjzyxhef.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gycimmwdp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gdzaxfjeq.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gwtdbrwas.sHtML


<!-- 参考信息 -->