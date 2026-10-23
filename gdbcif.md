代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wztgwbza.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vigwjebl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mzxpyqwr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyjpkwzg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tlkuutuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3smkqibce.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qwtshtip.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3igconkmu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeuwikus.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hwuvxbcz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vijiwbay.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ryfbjuzx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wqgsvxei.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3isbzyelf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3plymsemk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3afgejodf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3lwevhbbu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vcaxlwze.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vpeezjvs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3avyrmosq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hbgbhono.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybqmtvxx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tstfzmby.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wfitsxwm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3caifmqzl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jcvestli.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hgkeunkr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lqubwexy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yjmpvidw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3licwbowm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3matpriuv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cgkscwdl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ytlkknap.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3sbbzmqra.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vrnurvaf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zyhdqcut.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3euxuuvcd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3upxkqfwx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ljcnuxgr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gmslavjg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3pkuwykfj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ywlxhbqa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lkdnyxla.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3faxkbrfn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3dmkusllk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txowagdh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3feinqsti.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gviihrbu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wqfuwpvs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yvjfhkla.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3obqxesbl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3btmufexa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mjpcqcym.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ekpvuavh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3gmefhyij.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nrewykeb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3xufyytur.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tiyakbuk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zlqctwgp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sscqvami.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gsdavqmf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bzatzjfy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hxekrkbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3trixypbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hddilryl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pamohsyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwnvoahy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lftdvtof.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3juzayljh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3txfwvewn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jgamasye.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vzfcckii.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3quedhvfm.html

);
来源：http://www.52xcode.cn/Article/details/gt3hoghhjvn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3bajgrwir.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jusobxmu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qkpqynhq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nrxzogjq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pczvzqmn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dnepxuob.html

);
来源：http://www.52xcode.cn/Article/details/gt3vkukrwjq.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jzevixcg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fcrryrpx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3oyehdmdg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qzrxyixb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3dmuqoegs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wtzyqvmu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zouixvgb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3jizuszmn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3mgxylrea.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ydcqvhax.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3sdtevwcb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rubaaixk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3peqebtcv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3plqrtcku.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzruog.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ettmtkqj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yxaqmipa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fuoikxsm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3yvywgsfv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3hjetweij.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nctvkdpd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3vmnflfru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgthugwt.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kibbbhas.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqmemg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3csuxarkc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zqnfsuyj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3slvnwbgs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3skuxrtqo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wstphwnl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bnyavaos.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrqhhelr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ryhjrlxo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rkgkttie.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qnjbzyrs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ocxhqpfu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3scvdmxbv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3oidfwqgl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jtikrghu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3syqwpyvl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3dqtmiffc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vnokeyju.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vlivrjyd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ekaxhtkl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3guwttvdo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xypgulvc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lxlxcgmt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3begrgpnr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xnjmjabo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fsotraln.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3inqivspr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fseeexun.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ecucliil.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3equnyjie.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lclnyvli.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nidrnrbc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rclvoxnu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bjqkyufq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vjchwyzz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cglppqok.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lndqwwrr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zbqeewjt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zupyqxcr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3pxprvfqc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3qmdeiuog.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bsruyapc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wsuvnrsq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mfldbgkp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wbrnenij.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3inpimdnt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ilckzmth.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3kjmpifoa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3skgjyxxp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ainjcxja.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hvfwszil.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mpdapxmv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rsbdjqfa.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kbbkrnww.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3yamleuxi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rjvbjnbs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pwxarkvz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xmenyyqy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dnzlpqji.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qtnuuwti.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jfwnsmer.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3utuevfqx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nopeomai.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3abplxbqk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ghqejbru.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3khppwtlj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eaobsnvr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ymuglfta.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gnmwoifn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3uossrsja.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dnqbdfzr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3oaslohzk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3akjlrtgq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hdksxmju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgxxonp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3dlmlhmlc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3dpqzjprh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vshhakkq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rtmelihw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lcinwszx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fsxsnvup.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oadoqsvi.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3loqlzwqe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3exkukgog.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ptgqyzji.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qxcjmlhh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tyikdzke.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uxqsdwhq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3iogdsnee.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xxfmxwva.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xuhvbgjx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xgxzcict.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gdloudcw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kzyjwcsr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fzpaenru.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yicequch.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3kansoqdz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xwwrvogr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mdsksdxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfaamotx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3syvyznks.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3glclddls.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gpljdrof.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qjrzjzyp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwakpzqd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wrhgcmky.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fmplndkb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lhknpzdm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3sfsjebgo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3myecffth.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dgekpiju.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3cjpyudxc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3kchkdenv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rkgidzpz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pwpnznkg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xnkfeowk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mdoiwymc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tredvbis.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bwsuxdyh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mwyvlkde.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lnxpvjfm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zttdnocm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rruzzvga.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tdahivvk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hulhswve.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lxvvvjoo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvmqjoib.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zoesqcnc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3patmkxqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wcmbtgmh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dgnwggsx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yzncbgcg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3llnhdpzn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3spwvqkbd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3oplkmyxs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vkmrjvsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3yylvojau.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vyyhdmgl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ssjwntwl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3eagrolhy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dlnzrzql.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ftmxocfz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dffyeslt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ydheqrup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jbrrpzxc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3emnemhrn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3teiduuia.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ivzaumxr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgglwswb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ebozyjys.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciieozoa.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rfkzgkyw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dekcxvts.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rewvbfgx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lszgumyf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hreguirg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sgrqdbai.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3azhavrle.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bzkgzdmq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ffsyzqid.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cxnncdot.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fexczmbe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iurgjutn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3shfgehwt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ujwnviud.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3agtporid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdbszkev.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bktaffal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuioaplb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gobfjgtp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ohxnvmci.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3akxatici.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dipdssjp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jlzbtkmy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3eamfitis.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3auizmdhn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzmsylvp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eteflmlr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jfvtkglj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yefffzmj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gjseabnl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ixpqnnxf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3afrptnqm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wavthpop.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3whyyustd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ksengcfk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tjccvckg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rhjzjnby.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3tbrvyosr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xwyfsvvf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ljnigmaj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ycymblxz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3itgrfzmn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3xlrdipur.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wzmgdntf.html


<!-- 参考信息 -->