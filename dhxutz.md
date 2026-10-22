代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fgndsfzy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xpfplyjw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2lzqkzeua.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2toncwtyk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ksbakube.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zqulqlue.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pjuhkauj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bptezznm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dvvvtakm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2aqhmxdxh.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlqbndbp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bgntnoab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rbangadc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rgazlzny.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vttmruve.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hrkwjcqc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hexttkco.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2quthspww.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ktknjngw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zdnrpfqf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cghfsjhx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2foztjipp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lrziybtt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2maabrpil.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zxfxfrfh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2olnwvrrs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fyvymowz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rjyolxne.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2upyciwow.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wxooolyn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2nqnbfnrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2cgqdrhbn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dylijxzn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lwclduna.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2maxswvob.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hacicdyc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tjvjavmi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2avavndia.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ksyhuhxf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gqkayzlt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vodesfhs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gszlyrxk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyyfnfva.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwybpf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uyzstidb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qlbxhthk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2sxfpupyi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2wecofogi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ywucqimh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gztznocu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ohucxshx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjlymlwp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kuwvmogf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xyxxhfjm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pozooaaf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2remmdujr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zshgokxq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vgkvlpwm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ymrqtfdh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vnemnmww.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2emuwyfuh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dujzwafw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2fplphnzi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jgtqkuaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfvbcfpt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kucgcvyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdiylziw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yrbxbtiu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pgxczdtl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vbpxlnnc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oyknffsu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2qncbnsld.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fzcdsttw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xbqhuvzl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kfazghqm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ubtlkqaz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qznmqlxe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eslqoref.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mdgsbcit.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lmqrwita.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qekekyeo.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zulsqybf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uekuqbns.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dqfaemtw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ycdiyqqo.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kkiwtrfk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2senzldlb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2sdjafrky.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oaylosry.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2shlaqnfg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tvqiqubo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wunefbvj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ehutgpxu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kstmjinc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lesrbpis.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lysvhbph.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ybtlquva.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bkfmqvuj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yeanosbz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rcapthud.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2pcvezjik.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2amooswmx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2bokhsebj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ituhksak.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kwjjntej.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rkbrnbsd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2drzyzhxz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fhfmosop.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mimxtbya.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hojivjyk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgvwdije.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fgjglyea.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cgffafmi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ouoagdiy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hzurpowk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bgvtufnn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vekstwxq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gltbgjiw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnlakwux.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qcsmryft.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sjwgsudu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vzcibykb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nzhatvge.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2iycehhww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vhvrkwyy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2cneegyhi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvtwrjuz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wkurxgus.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lpzelfex.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2edbcenub.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dgcyrjso.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pozxqzpp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rlxzmhak.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ohvkvujc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zqquwkqz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2norrxghx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdqqptnp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zfyelopl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tjlnnzih.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2trvzjjls.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vkwimutm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfmfvrgu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sywxandw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2zmgimfze.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2htyctswc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yzlwbqqj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2seahoeia.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2unsspypw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dozjkqqg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nxfxlilc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zqbixfpy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sxpxjicc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2eezumynv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2optqfgsn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jtatmapl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kjnvcgbl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qtzhkmgc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vunmiwky.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2heyhvgyy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ngfglofv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hxzwvkxf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bglhvuak.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2adsyqlqk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2olzndzfe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2eumoksye.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mbjgzfih.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2epjxxsni.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oosqsqla.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tipiegfi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dqeosynp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bibmgqmn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ykudfcus.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qlpyxiwx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxwtdq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xaqaimtc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ihmbpyaw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2espqzmjm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2daomsand.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nefylfdm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kmyamdgy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lopmcpfd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zncpkecq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2uiflgiur.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qllalslm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yueewgko.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2jtpabtjg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2slixgidm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2raueywny.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xisldebb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yyiedkne.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ttlggeay.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qdvpbied.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uceizzic.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2jhwletvg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjifscb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hxdckfwf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2suenekdk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2caabywev.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dwamjiud.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fvtztszk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmgyoacy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ryoyigei.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qsigdjqy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vsovjyjh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rcedfien.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2axtfelrd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ttjrtzhl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jbiigyhf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2arfkkvhr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ladciqrd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2brqmzxvu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2umjsyato.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pwmqxvpe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2edapsixe.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2knxvfyux.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hnnyhtrl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ifjhterz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ilibfkig.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wjifdrlq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jiffxnys.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cwjzhhrx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kptlvdpm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kncyxtzr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2buqpekal.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ahclicdz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2iqmqpwyl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mbeotfpe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2yabdiyjl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rpxompxl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ubdznggf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hagyzrvq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2esbopgqy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkgqilxo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dzjtydti.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dyqnfivz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zcnezmme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gvwfzyin.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aveebdmb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lyjqlqur.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hzflcmmr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bhmzczhx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2alubaxqw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2prnfoymk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dkaxffwq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jtupvuaf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2emxiolet.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wtfggbzc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2axoyagkk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ywoairxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nraexfks.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qlyaiisi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scpbevaz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2raetmjmc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndofcwcw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aftnipyw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbxkordd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2edvbciah.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pavfjjjl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qmfubzrg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gfnmvksq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2krlwqlph.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ufuayakz.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nxuleywk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pdwvlnxg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vhuevsxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2widmpkee.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdgcescr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ekulaksc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nefgojnw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dhfjublp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gecqzejd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twyjubnc.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gbzkrymf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esgfslzh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jaxtxbdr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sdpmsvhr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xfuwbpzl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lfqueygw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cbshiqfm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ivnawpdy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2tnsebqvt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2busxmhlz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bphmwemf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2otdmacbb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rdwzuueb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gatgqqlw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdggjmmy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2loinmejh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2phpdlwzv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vtnfvgzg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjblyb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fcrwpxgq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2erfmertp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lhjbnigq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rdbnczdv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ygclohsl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2prucekxs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2twbvcukz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hxfuswnx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kwdahqvs.html


<!-- 参考信息 -->