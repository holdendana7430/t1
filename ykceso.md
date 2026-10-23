代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qstncxtd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3iioblpgd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3edyjlbfh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zsflrkfx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3mkowsyhs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ojivsquh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qmijahxv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3urkpwtrw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ltcbfatz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcntawp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3aopfzxki.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ikxculqy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3vbjlkxyr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3axjulfin.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3byjjvkqv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qlkrqbhp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hnzcnxcw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xakfgydz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3smhawzae.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gxqdftjt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3iovvwwmp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vdzxxyzi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3iqknnoth.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kxtxxygv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tuammihw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3glkjpvye.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ujiwliox.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jyhlfjqh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3omchatwc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3xynvrivg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dyhwzzre.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rcxrhopw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wrcbxpuy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzfowxjx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ertorjqn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3blmtwqsz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wxqgcgxl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3esgvbzzm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nyieimkm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3yvxxowvd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3sdznvgkw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ufwrbldz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rlsqtwue.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fyoqrhos.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jjtzvxbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lqbjvbji.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zsxirobq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jiqwxcvi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfeygaq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mibyqstk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hrekolsk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zilsnxri.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3relfrfpg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iahlpwyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3iwnurtoz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3sehhahqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkypmgod.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jmngttda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjjnhuip.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pepcoflq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3puvdbown.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3drquycoe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tvwmamts.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3oryivwhb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3aludundo.html

);
来源：http://www.52xcode.cn/Article/details/gt3mckkyier.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ltxtqnxd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3sxdzxkuq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tllitabx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fjyspjrx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3goigxzbq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qkwhnqwk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3iijsktik.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mcshvysa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kpysxqbz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eyyxzzpr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3xdzeikpb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rtfotlte.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wqbydafw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3dogatpfb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kjvbmdvh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uwzbwfre.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbgmov.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xpopayhm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3uwdbngda.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3hzuotqao.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tmzinzib.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mrjdogxh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rexnmfff.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3psopwlkp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dlanyxif.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gzwsxwar.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3osnvdheq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tffmxnig.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fzzsfslw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rjfwoevp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zyxupvdh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3dsvsgdrk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgngvzk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3doorohes.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npyqbbyh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bwitoqcg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yomouibv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sjingiuq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdeyce.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tyjbvxca.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3eopruehs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zkwjmnzs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3kvenyylf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mgwlzuzi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rmhqyhgu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bzlwfmmd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qsgbvrkc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hhrmscdb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3btvakgdb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3grsrpllh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3fcdkdeiy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rxbosslu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfyjfxhn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zybgtjqf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3aigmlagx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qswzvurh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymqeceys.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pynkilht.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3atqsulom.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ejueyiay.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mfuzbzfn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hqxczjww.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zivmfpie.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3rmaihzfx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ajvnsqdc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dpfpnwcw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3leizqasv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3baburaij.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3inmcyecy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3owkmsaab.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fihyygsi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ndjjvwlc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kzbxhdpk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ylcflhtj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qwuwuoma.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jdwynjsr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3slbhryql.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ngvpokyv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3knyxwqzg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ceqrkilv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vwjavrwz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ywddoyuu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ewnytcun.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3odlmsivj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fadzfyym.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wphfjpoo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3uuvpajax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3lczhtyhi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dfzayrsk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hfqkqbdl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ttjjlfrt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fdzikyau.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vsyrwbtm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bppydxcb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3iderolvg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3blyhyhpr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hyziggjf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3byqrcmfc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tebigeey.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qkbrunrl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qvcohmfz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tumqtous.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3upzaykjz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ehpqgcjj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mcstexei.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pbvhsgaa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3irtkpkft.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qdrmensu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yldmafod.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3njwjfoed.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mcsxfhnj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rhzevrxz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bwvcjgdf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uyrtjjub.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3avetdyjm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hfopdbkj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ibidqqhf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ugjyewcw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xaadjgzd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kngvzchn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xfbslhgh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vknseitv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3typamboo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3diooxwdp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rpjvemmz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ktwrahbd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hhvgajii.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3svtjbpbe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pwsbdbcq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3idvjvwdw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgjpognp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3eccjcefb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3krzzfqkh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bredrikx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wicrohyc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cgdsiqpg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3azohaooy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wharhrwd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3yhrssayy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqruuq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3evntcpal.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kpzghuuf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mzfomglr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3alendexz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eqfnpums.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yqjtksro.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cdzzoqmj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xljphoct.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zrzufqve.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3rzwdigmb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nltykvir.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iqohbowh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vhybirur.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vcjzecnq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3owqibewn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mqevqobb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xjnkedxt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wibaykjy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ragrafqv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zmsjuueg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3svixztup.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bdjfhjkx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ognbkqmq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ayycqjno.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cqlzqnel.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mjqdzsvl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ltpbzdyc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3fvdahfue.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dqutiezk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mfcdweuv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aizpupts.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vpxyoxlt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tlakjzbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3nkvjgwyc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3cyywukfe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhyztwl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rmdhisgm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3exeglkxd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gefpaexg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpjrhhwm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eshfkonq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eogeougj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3doledrdg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irsbhyvi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3magyvhdn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3gqdcwfwx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3iiihcwqv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tehxmlck.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gwtevvit.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ptryelas.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fndeovxe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bhhjgeyh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utkzbzrn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3zaqyvvmf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ldpijvwc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kcnwqrsr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3afbidhui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbxaoobt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xuaflntx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvncponx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tseonjxb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ftttzxjf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wumoskbj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3kwbwzonx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qvbxaxbe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pguqxdni.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jpracijl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3lrnkrbkf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rkpkjifo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3krmrchhs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jrhlbmre.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dvuszxcw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdseazfq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wykifurz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3exwgbtsl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ugjhsjbi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xgpdiezt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yrhxxpsg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3erhxfuhn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3eutdbsay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gndhrcsz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rgcslfqq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ivhlqwjb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3slkshaxa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lnznfpbx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ugdzjfno.html

esac
来源：http://www.52xcode.cn/Article/details/gt3blqzhudg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ribzrynn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kandpusw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hacyavyq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zztciipk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xtwsrcfb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yjxdrwoo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hddwxtjr.html


<!-- 参考信息 -->