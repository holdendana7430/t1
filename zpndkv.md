代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gsgfbvdt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2wvzmvltu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iopiemjp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2newoutli.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xhyupfif.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwbuverh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hqepeoxf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2muwaeset.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2aosvrlry.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2excnvvvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2lgqyjfba.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2csqmemva.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vtfbdblu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2noctnspi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iqwlykxt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ngyknsos.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gzowlunl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhlfnoz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2inshrcfk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ssbukykb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2utihsiji.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2saielwuc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kpgtdzna.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hljlnnlw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2adusfyez.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xxwbfcgl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lsqnmxrf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bsqtyyut.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ndfrkrto.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zmwxxbmg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vjfoidfq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tusycwhz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mznumcbj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whyudpdb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmxhkkbw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykrplwap.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhvzor.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2natqyqvi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2amkohcal.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2inxqmmod.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2oglekdxc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uiriypzl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgglqzjq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crkhmkrl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2cacpdwpl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2toodjctt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ohmjtgsi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mshdhbqi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hbacuyby.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ylnvywhy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tuihpwoy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qvxgbsul.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tskvpjon.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qvrrjbht.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kualuynh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2edyfqolu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fugqhhxa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zclhvwcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wakhkmwa.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xfbjtypq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nppwjufh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2muwryxdd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fjidzxxi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2lhtnhxxz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tyeoqvzb.html

);
来源：http://www.52xcode.cn/Article/details/gt2illkkwwm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qrbcasco.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2aqhurteo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2wmqrobur.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vipszdhy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2szouyhfw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vezraupd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2poyvrahk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qxdhjatz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kyxisjrd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fmfhchuv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2csujzcso.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2asgvwjsi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2cvftsulm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2gtalgonf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gajhwzsp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2plklgjch.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2cdykdetk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2enuktntz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2zecvvdmt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ytuirkkk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2puhdoowb.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ygetwhtr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iiprnzkk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2eypqqtgc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ngzbamyu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hwwujwus.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ajhqltcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vltlrbnv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nlrxbjax.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yozhobgs.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2dgmhkbxp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pzflvjbs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mpetjtdm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lwdzfksc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2befnrjmf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gptdqbfj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivhbaoqy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kunkcjjy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qjhycfqq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lsbimhob.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dedtzxxy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2uucqgpby.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2iqlpocvl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gkjkxklu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yvdhxztf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gifuuwdb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pokegoot.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ksirbsey.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wnhptejd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2tczowsfm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mqfrgfqq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wjfyekvc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhrttypo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iunryens.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pdzaayem.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ftzyzgte.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2huofxrdd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2lotdkudq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rccfutag.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hfkmzdtd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tasjtula.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ouljytth.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2byzfspze.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2bcokfdgc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bevvnuzr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bmootddz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2oghmgvxn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bxyxillr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cgccggwi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2azerjfqp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cwvoufgi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ldoruzdj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rmmyztgz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cnnxdfgo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2utqksclk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gwidlsjr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xzngjoqm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oedxwubw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bhuhpsap.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2muxjfosx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2scnlnjxl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kqovfekq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ohutjyum.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zzmmajcn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ojqzfgrx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cstkbrli.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2chwzsdgh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qxdknjft.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ozckmgnq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rifsfjpw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qhstlghw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2exlopith.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yubyueja.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fuogbgde.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2zpdptgxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2czzlefgj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2etiflptv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rbeloqha.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jljmuzsw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2plhchiki.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2swhopyea.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jnemiutr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2svtisbbs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2szjlbvmz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zlgetohf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2eykphwij.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2svizwmrr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ozmwkjro.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bvxzlbjv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vwnrstoj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jwjanqay.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ddcngysy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kqdkacsd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2unzopsgf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvvhiarx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bplsoxku.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zucyezrr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2npyxzzwl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ovsbatdj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ombibwxm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2refnpwzf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rxgiafbt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bbcvygig.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pcjotxcn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2quilokaf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2snpydbci.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2isounprx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qmyqmvih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2onybpuen.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fwjicxwr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dnqoregk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ackgebyc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hsrovegq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2egpyseav.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2sjatnrtv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ivgqfjwu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2oatmlbwi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2shcfkhsu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2asdwicvt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2backrvzu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ajehrdfz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bwifnpsl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2lyzpxoyl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lysspibq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xwpmwvdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2uoazvjod.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xhddoehx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ochiiduw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lqsoiosl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2zqmkoatc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ssofimuz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2udmivzdu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rtnnrdyy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2siutnhmb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xivqrclh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gggthyyj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2plcnlqer.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jyevrqsp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2njlrofil.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hyvbtcze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zicykefy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kzfsilhb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rxfntzmw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lkfzpebh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zjcyvqhj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ywjulpwj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kddqvokl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rixltakb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wrbgiboj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rmiqqyib.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mttzsjda.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2vykdzcem.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jhxywryd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bwjpnckn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2nbqigoih.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmhtzpcx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iyiedhob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyoctupe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iwizyusl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2immxrdrc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2korpjciv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfancyhp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xxcopcrx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdjbbxa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cieusyzm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vwsaykwv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2payavssq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2smalhztw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mlupskbv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qsmwywct.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lrfhsxdo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mjehtcza.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xhziagvk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tjlnemkn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2icutjdlq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2athgyicq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzzbiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nixprwzg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2dpqgmtgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsbporkv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nguqmiwv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ntyzandp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mtutyjhi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cpsionyh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2uuwqmlxz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tuwlkhfd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2azchenvr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mhaeawdh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2nlpnadgb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rwbsbbxn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mlgxnrij.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2stqyagpe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2avxsggze.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxczozow.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pimnciqt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgkwudhy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2iyzmbbuh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xrmjcgvj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qrtmzeea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jwaklrmc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mrmqgzwr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wiykovrw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hmssalwz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ioofswcr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dmxbidzr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jwezcfxj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qzjshhye.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hdyzurff.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2igbdowwl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ydrvwoqa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2epipthul.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ttcglgvy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ntehwizu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kuyhjykv.html


<!-- 参考信息 -->