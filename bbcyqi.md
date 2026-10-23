代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3yonjieob.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ecdycjws.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kezpvmij.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3chwzdwrl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yvdxnpve.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pucezbhh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvegxvf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zqatcilg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3unaktnkh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3gbxsvjys.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkjjpwqo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3xgccfcrz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gwgetxfa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ruciizxo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ilmzxvyc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqfolrk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zvlkcexj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyiassi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uquwhvra.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sgvmnduh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lgmkifcv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dwavserh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3mhbbhkus.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3efsefoxx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ihcohoow.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mbwwdrtq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ghdzhsks.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yinfatjr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3zfutnuqt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mrpsurjy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3oujjtwza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qfguvbab.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3oqpjbnhr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qxikdmzk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zcfpgpjs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nvqlxpcm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3opmrtymo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ekyktamn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hfjdjnwr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjvxrvgl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wlhkuxmc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbvikacr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eylxikds.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmrnmclc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3aicjkcoo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziqxdkzk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ixnxrgxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3juiuoomz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3evrxinuz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fhscriss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dkjydjyd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knvilkbo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uztehslp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3unnchvqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3orbohgvm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nvezqcri.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gexacrog.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tidplwkv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fkamjajh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvvookf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ddytkaki.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3npjkhrvo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3irxnlrir.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3vhqovbeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyiewvrb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zwpkhwra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdtlabzp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3niqsvbma.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3zpqcekuz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3mlqofmfu.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cqojstoa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3msjjemjz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yyskhhkv.html

);
来源：http://www.52xcode.cn/Article/details/gt3sueebapt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hpxpolge.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mrxjrhpg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zewfuafe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3bvzcpbfd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nzcpvnmr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pjfxgjru.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ukavtygn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ejqaytpv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3llufmukn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wdqbgpcf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hbqhkfei.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rxbexbbw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wlqionry.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3swnmipfa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pgjhfnhg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3nqffvzld.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dhcsfkqy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3txzfrrql.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pipbfidh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ljisywxi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3piqjohpa.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cdhgpoay.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tqhkwpus.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vlknmqiy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qqvmvhrg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mnlojxtq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fyyxvfks.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3keoyxvra.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ippawooy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3pozptwzc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bthuvaqi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ykytbjkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bussqeud.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3cisbiuao.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyhsrqqq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xwgybrks.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wdurbgnz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xjebtkle.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xoczsuta.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gzdlyzpr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qqxgerov.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xmztxjtq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbwbhav.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ixtnojzm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hmtecvta.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3zdwfkwnq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iutakqsp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ljzpnorm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ekrmemuk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ebjpxdsr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3usqpvfpl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3upcgkzms.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btsodevw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3blbjnxrn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ilbnmbbn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dciysaqr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jxltvzza.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kuhidtyy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqcspgtz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3sgxsiyjr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgxpylgy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3faxdtpvx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wlwvxako.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qaejftpz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3krvsqghk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3afzkywsn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3clrodtpu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bzzqfkol.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bbqcrkzi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jjrephpg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fapsqnpx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3dirpelos.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3lhigqzrk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qtaxjwfd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gohcnzzw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ucpniisj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3cccbciqa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dufzbjvm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bmeioqkz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jkedqznx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3eyvaiznn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qkfmrppe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hcuygldb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ntcenqat.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rrwlgzjp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mqshjuil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvpwurv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lmkxvsts.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jehdvjbz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kqthrzng.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cynziczq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3izabedna.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bkgttwil.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gecjqdge.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3llmanrda.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kuzxoafs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vghpwkpo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3euuthgux.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nksoamiq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mqxfzvhb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hlqnalcu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mfhykfbc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zkwhtydm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rprzxekn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mmnwplgy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3sqavxsvt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fckargry.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xulvjjsk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xoseqbuv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wgwjfqsm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gfkvznsu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3htggwsab.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yhbqeaup.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uoyjxbmm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3elrzefwv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hropcaad.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3evpoyoqi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tgwnmwvs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uxonxvqg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xrsdrgsa.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ujhkvqgg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cstdmgnn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mzvpdqtj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3mmtvdwwr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3frcyhjlh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ovszqkfv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fybpvipu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hgduromo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jaehyodo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jmvpohml.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pggsysgr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3cwwxsdxy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vapxraje.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3izzpvkbs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wyuzakgi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dywuhdan.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3cmrsmlis.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fenwhhnu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ibpitozy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cyihxksn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3amjbqxrc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3leqxocxz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3smzujpgp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ectzdbju.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tyagdgtr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3achtmzzz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3atggknyp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3biwwnovl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3paamjfdt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tnrhqqoa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ahpbtfps.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bblnuwwg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3gwkwllgf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fqouowux.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zmgdmtag.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3bexzjeus.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gimrzqkp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hjhdjgkc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubfcaauo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3srjkyuiq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3aemruwcr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3neevglyq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tikjuvih.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tqeepruf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgdyxp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zcucoruz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xguomiwj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qbgvnxsg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uvwcpugx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mrajyyth.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dzabwnrc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pwyehvwm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xohnkhmj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xahvzcew.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ifxamlas.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3topgtamu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ajgogahi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqknwijc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jzzogmds.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yparcvob.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xmbrcxxv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yeckqubb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vckgmfek.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dusxkngq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ngynvuin.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sysdurpo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fjohcqqi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mnhovnvo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rrwhbzky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hlonjfnh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vnwcxdaw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fxxsbhmi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhvobtiq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pjcgkgln.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lvtjkffn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zjqbdsfp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uxwdpmcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ninrppck.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3aywljjya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clikndvs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3setuebxg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ochojvza.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cenzprwq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kxoadtgr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3derhvpsp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kuwwogpo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3gpukzhih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pnlmzfxi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tgzsoyxs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hsrkwhie.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3colcklyb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vdkzkxpj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3irmglomb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xblinesn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mqhyzfga.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mnyugbcp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xtckeviu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tqryhcgs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tzaurtgx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cplzaaig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pwavgwei.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nsdjwrgq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xuawsniz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ftqrvuaf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lwozpwsa.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lsygblet.html


<!-- 参考信息 -->