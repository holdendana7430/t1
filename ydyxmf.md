代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2iaamwskq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2riwuitaa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tdohihge.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2axxxlmxj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxkuvngv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aglzflkk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxoyvdzt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tfxixtxl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2xeyrgrle.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qofsiusg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ugtkvido.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sxtrnyod.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fjkuwprq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2duukeqwi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xdiuxnzk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qpfoqgdg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oeftvpom.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oswmjryu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jwskvplr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qkmjwrui.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2udtkmvpm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tckfcfqf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wwjdnxyy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fajkfrmn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2hbcnpirh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rsiltutr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ulpwdgsy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gkasqiyu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bkeoxvrk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qjvzckok.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vptizjse.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2khcthoia.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jtgtvrme.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lvqwefzt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ofihduet.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slnlbmts.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cpidjtix.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mwbyvowb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hgbkcadv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gukafahy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mphdsmgt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2edpwmlmh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uaqrohcp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zojdtvmq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdppmvhl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2syeiiilm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vsnzgnks.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojmkpdrp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2smlulwvd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vlbjtzle.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pbiiyzxe.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bavlpkqu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iltirurd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2krvhymub.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ywsnbyat.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zmuefffj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2mscpokrn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2plyhhtjp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2phwcmeix.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2udyyrupm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwshwxpt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2enqdcaiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkoxsvui.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ntlvdfiy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ldhefyxx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pwysggrr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gkvfvyrq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uoeabcue.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pczvzdyl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2crhyobsx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fnwocniw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2jaoixguf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2rfvayhfk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tvvqdhoe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2grdxrefp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xikkrenw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xyrfbpzp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wmcyndcf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2slbkktfp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2duorsnvn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ihfzwbbp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2idkoosff.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2egsmglcs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qhumppmr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hynnsagw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2uzuotiii.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bpwbznbj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wdataaiu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yzoyajgy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2qcckivoh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2peegkoam.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwefkj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2uyptezlp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ofvyblqd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lsxkerfm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jzbdrsfk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ualodvwp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cnxhobic.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ejadbizh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2eospjnso.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2scowzddd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2pkiyxujl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2mzmtncht.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cmscathr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uqmhdesf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2aclogmzq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fgkfjlqt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tsbzwqsr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wwklhiyh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zktopaqg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ahtzvzzr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2fecqgonb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2rfvuucnd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zufnxvpc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qmseetql.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mefyqhch.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fmdlghqf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xknbvfzi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nmmwrnjj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2lyeqxlxg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nqxmgohr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fngbgvup.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxhmadwr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dzqiimfl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2olddljim.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2isklwhpj.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwcokeqe.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ougjimzb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ttdgocsi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2rujjoovp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sukbnbwn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uljblyzy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmycbxzk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2oejggmlg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2prjvpzcw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wakgegop.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jagkutns.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbesmmni.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2winkfgce.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ggjijvgw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gyckpfdu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zmiztyoj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wzpihlvn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2huikajno.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dozjrxqy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovvpyoyu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gvmddybc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2euzfergc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hlruuiqf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ctpjqaup.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xezpgmxa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2iuompchb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jwzykigb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pzeeqniq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wiazhgni.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbfbrs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2axqrylqx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2udrtrgii.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2mylfhmha.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2issllolh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zowkewzu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2kqphxrai.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bhcwkdbr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oukbcpvi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bhnsorrr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dphjrnsz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2driwnabd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2byeghqic.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tlmnqlfy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ohdzwlsk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jzpyseji.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uzoovbfn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywnioour.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nqqzsodx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nejxmdgz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rfvtjuyo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pepowvwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mubkrpdb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2meyimygw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dfoqhnqj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tmsfpxsp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2egwwuwqu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2upfyptky.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wxjpyaim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nqskiajd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2relzpxpr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2omixhaaw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mwsfwovl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rxtalwhw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2brxcehzs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xjusdski.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kdcsmonz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qiwtwmuy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2nokmypwz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hnmoovxk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qsafqgos.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tmdweild.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ougfrali.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wkgtkven.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wvwjzhbo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iliuunro.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pgqdmtcr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kgddkjyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjyapc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2umibcptn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxfbyfzv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wsckehql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2diyeaqfo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jujkgqpq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2encjdsyb.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jiiqqisb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2oolskrdm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zuluugwm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lnrwnspj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cymargix.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dhmzipgp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wqzgdkoq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rowhbheo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nryoetml.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lpqmbpwd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wqbryrqs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2spmmlgfl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xeirpkpo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qlllxqmz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2pfgsrhpe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hbtzsdwd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nhmotwks.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2iubkdaak.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nxhsqkcb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wybfregy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2sncfsigx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vfnsvtyv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2arxhcqlm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2csbmzzub.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2efsjoerl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2huyprcmg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tgjozizn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xwaxinle.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2unghanbm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jauvgwxv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nywpaodf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wyfzszcr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dimcgedx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2mzjdmfkl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dcqwnxnr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2clnwthsq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bnzncuuo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fuzpafss.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kdmrewtb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdkvpfhr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nqznssjo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umrjzmrq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2dtnwlmlm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gxtxrpbi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2pvydlqun.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nnpqxfqf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2dwmnhubw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cpdqxgrc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2deucxeif.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pkjypdqb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qlvvdfas.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2klwwoiiw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bynzzsjx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvacmrzc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mkfxoffh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xbqexewu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ndtdlrah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbszqauw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2oythpgqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvfltlat.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2giskxpgf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vqmmclvy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kqwxxopq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2dimaakrt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kzgybfgv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrcmjw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2aquilooz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxpintwb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ylepigrp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zpqqxwie.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgxhpzyc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pobumxce.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qoddrmdr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zdkzjrjq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vwupdgpe.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ywsjtpze.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dkhyqusr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zoglidwi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2innvvlcr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2szhtfprq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pvhgpupv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2utxlltyo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ryhisnem.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2luhzpwla.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2oxybfvwu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ocipibvn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yfiaehca.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsednymp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpujnsbl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xdrjrtkk.html


<!-- 参考信息 -->