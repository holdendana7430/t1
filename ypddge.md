代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vfhsgecx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bxrmvmvc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bhpdijob.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mrtqywbe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3sstmvgoq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qeduyjkr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pkhhfnhz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tlkdzlbc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pxnpwipg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ilaqwfnt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqbnbeeg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ojgagojp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3copoosha.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3opeksvux.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ggxdwxlz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lymlbvmr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mnvalose.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lctvuvpp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rokfbyqx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xloiuclb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxxuqp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xatawuyp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mbcoadif.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cjhakdtr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uiauukfu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wwamuggj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3quenjaym.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hfqvcyxi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sutficol.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qxrbsosv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3znhsvzbx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hfuefuhl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hdlihdhl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vevymewj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dajbtxrl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoigjspk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gzueafbx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmwutces.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtcktbyy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hykbnuoo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xmsxqyst.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evfiiygh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dkeopkly.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jjndmxqb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3urlrskri.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ewslhlhg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hobsrsei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dojafgnq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ofvjejyh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jzfwugpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3qpshmyej.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kpbzmrwl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yzgekhok.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3scwhnrek.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3khrowrmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kkywcakd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3kothfrvl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qbgtpvse.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pokcwvoe.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yjeznkca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceryaxob.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3skfbicxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oatyzhhw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tsazuzli.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3kfsfjcrl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ehwxsmmh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qojhavno.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3aumksmlq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3perwdyse.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dtiefeyt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vehworks.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yekbehtj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dljsaone.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ixalgvdb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3xbftwhuw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gazquwpw.html

);
来源：http://www.52xcode.cn/Article/details/gt3sycvbrmk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ifaolxri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3wdwkjaoa.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bwpsdojs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gyoxbnfh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3gdvvmegc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3exumqhgn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3chyuwetd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3euidfojo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3gvfbmzkf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wrocnwip.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ufetktlw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nxmtilnb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3btjcbjkr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fdmunahx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3axamszxg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lilliiza.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vrylvkmi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qmgusbeb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ghiopnxe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3jocwkmzv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yhawvjxv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tepjakla.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yzjgfowh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3skgqplzm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ezlqdqko.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dgsrhltz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eugtnmzi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqnlswro.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fbqktuax.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yarxwqee.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3edgwzcws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3yueddlsj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qbupnyka.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ddldnndy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kjyqaytu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pbbdxuic.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vgubblpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pufavhvl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3okoopvhg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xxigtxqk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hxgyhgkp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xhuwffuy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cjxxhifh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3pcxyknct.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hccaazcw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aafupmrx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3yyjzpwgu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ufjwbatq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wqdmxjye.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihkwbgcd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3giocgwwn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scwvyizp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3pqltiqoe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3npieaaxw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lzebbqva.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqprmyna.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3eoajxkcj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zlilbagl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jvqpnqdq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yjdnjnpi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gdatnnwl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rdpbspdp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3skmamjdz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jwxsnakx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bqajengw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tbivbksn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3xpyyjljl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nyqoxxjv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aemkadkt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3rrcrkzgo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gdsdrgxo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hhwfgvlf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nnbgfnbj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3sndqqpdu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3laloyhbx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3niuaodua.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qzkftajb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kxsmvkwj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3alsjpllq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ojctmzsm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ztbrgngd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ilewwtgd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kciuyamm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bxbtllkx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ffrjwdbz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3oztwrgvj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vttsfyhr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hwphglem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vjjqdjgq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jbvcrhxr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lmplsdbl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qbocpbtp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qzmozpke.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kplqvcrj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zsfdikkh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3saywenwa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cdqvzvan.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cogusdsm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xfkhbhzk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3aqhmoxuw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3gzedltri.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjsvos.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ranrzsej.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ipwhbcxj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3fjargaxg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3heeucbhp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hygocyrs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtyjtwts.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3oyawprba.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dhtqipej.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3odhuxygd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nauvkyna.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tuighuvb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3etkgtjjr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rtkxyiyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3felhuyfa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cdvbdiqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yvzelhua.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xajinrac.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3suvcdypr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3iggmqggq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ihhzuiej.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xnuvcbvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ndynhpkn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3aadaqwyc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3pjekxvqy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjlile.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xnufnmqh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3weqoroff.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lesewpsv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uevgrxnt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rerqwcxg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uxnhwezq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3saokente.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kjucpsym.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qnetskeu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zawlturp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ozyaizvt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kbtvqwez.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gyxhzkbw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qmtfegiz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3anyjuuyh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ixabbpjt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mefgpldo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vlnohlkf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbfjbe.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3abddsiea.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pqoehzxl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3agxdifta.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3yqcbiuli.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dcrhlxcb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygyeodqx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fkbuhrao.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3iurmqeum.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3tivpvquc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ugwayrpi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qzthommq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mhznapow.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3afgqeysv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hoafbtsw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ljhcvrvf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3mozdtriz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nqzxxwya.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xktnbmmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3sisnusfs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3akcqoalt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oqiooijr.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ioouzinm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fwzzuava.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pjtccjwi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvlkebdc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hruvfnnk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qnoudmbf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bxduwxhx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ygspokmb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mbaydbvl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dkjzvoif.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tjfvskha.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3blvfswyo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jiuzfnuv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ppzmhlbj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wnnzoupr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3adxohegw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jjeosejr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jdsxhyvl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dehwofoe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oddubovx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3msxehlks.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nicfthml.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tttwamhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjntldzx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qfvemuyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrdewzsi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3urrqvmht.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hyseqvvp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3igkkxvdj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wdrulawj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3fmwovhrs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zaknjbke.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3cznwldxw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xrwduxbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hwcekytc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zvuqqerg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3yunzvnam.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fnqlrglc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cisyunuv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3aychedxy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pflgualo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvnwaqel.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dbmybkxx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgxpgitq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3utpupiqp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jusnaepz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mrfyzdhg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hkfeinjr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3pijrivjj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hyeiqopb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fdsnymzp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3updwisva.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bplvadry.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3resnjxgr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wourzuud.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ttxmzhgd.html


<!-- 参考信息 -->