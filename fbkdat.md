代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kzhlnukk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pffdadmx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wetjkhwh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gfdbxtip.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qbshescv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tinbxhgw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mokllfcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wabttnab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wmuocvtf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ouetqygq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gzjdjkle.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lgbedpzd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jpcbknzu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gnykpmrm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xatslzps.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3hpusvbvz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3lmbxkmhp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zoylbvef.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jjeiqtxw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dglxzfvc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lnbxankt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrbvgzo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3znprtznj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gyguditk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vkvhahsn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xlbqjwnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qayrmydg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ltdxyeik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ffqaqwjb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fxhaxpwk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqepwb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tunukwgz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ohdhxunt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3enagnkhp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dwtxdgdj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3khofrxzh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hpebelts.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpayxpzt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3txxhzuhz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlfwevon.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tukxupan.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqlgismg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3yhmlnbfb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3gvwykewj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mmhiccga.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3egvilwcf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lcxzgrhz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3uascbrif.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3roaeiwsf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3anbxrysg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3dyejwxju.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3mxykywis.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gflfpeio.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uugmzzaw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cjziyqts.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3omwfimfc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jglelkfv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3khtdgryu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kmrawvgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yqzorjiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoymistl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3xbekexph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmdswtnp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3sukxzkur.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3yporaorl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zmrgftyu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pxbsdmmm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3payhwhup.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zozrddyf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kcqofpyh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yrjqqksx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jfysgpjd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3gnsywsqf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uxvhhrvc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wzdvvpts.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3decssgps.html

);
来源：http://www.52xcode.cn/Article/details/gt3kohxhsza.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pkfgrrmx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3aydspxtt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ougdegsr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gseskcta.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3frimhgvk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qmydcdpm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fnpygnof.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ewsrscwg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3rixszstn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pseepbcl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ttmkcbbt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jtzkxezj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3orockszj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3emuyxbgx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ecplrmza.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ubihqwjf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3vsikzetw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jtatdfwe.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gtxlkrby.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gnsophyb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3twkafbqr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zdwylklc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yaawkyor.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wekeajby.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3slgruadl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3medddjkj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hbquaycd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytpacrnu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bucjgxmv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vcofwjdb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zbakzwrz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ibnakttr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3klskqoke.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3wkhotfik.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mnnzxqai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mevgjwxr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ncigftav.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3yadubpau.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tcifbzie.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nvnnnclf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oeduhoeu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hgpxsxie.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uzbptgtt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ubkwhkdx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bescxyal.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jckonibu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gbiwaypd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3uvcpebzl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cqbvxajp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vychtecp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kaouurxa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vvkpqbny.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jquaofpf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fflhcpdo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3arkcspvc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imreolpf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iurjgxux.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qvumdqok.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3paeotgag.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jzarsvtq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kqdstexq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dgbgbduy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gnblyogu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3kvwbhpde.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cteqzyqm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pysolkel.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qxanzemu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nnipazet.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmadkgyq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nizqlwat.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3symvvrof.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3yqlvfjcl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qkaydzsm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ivjkiglk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eoabzywm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3yzkokgdk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lqzuaqaw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lovehuis.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rqxiexdy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jbwkospq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3sqrthgoa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oirjixrv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vpamurez.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zqorolln.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3rxwagfbi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mgavkqjz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tbdpczju.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yutjyheb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qkjkerwp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ftsgrnnk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3ecfydvbo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rzwpknlw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xhibenng.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3tecceypq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qimonapx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ijuwsrfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rywgiwxr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zsiiuxlk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3qulonupn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zpxhlxzc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ezboiydu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fcvwvwnq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fqscvrwt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zccgbdts.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3wkhchplh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ketptxdf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3liteowki.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tlhegilw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3aozjnfvw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjlymq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3xahguwpr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mezvwkbp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vljulctb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fukmllab.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gxpxhubh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zeenraeu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ntrthocp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3krsrgmgv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3xwloblce.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nrdzlwxw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xonqdgus.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3stbzvhzr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3upktjuct.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xjcvmbwi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tmaakoky.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3whpkygeo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3prugxsmz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hdzokyvq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ggawhoeq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rnluekvw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vogpszjq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3znvnrdej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tzjwwrgs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kabxgfno.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3fyoocmgk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhvqyw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nyjrbiqk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ufdbchza.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qfgvxbxr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3flseowxa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ycbccgbn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ddkiudyw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wiwsxtxr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kusajyny.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3snmzrhrv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sfzohtpz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dltnhtob.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3bkdwyqru.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mapoiori.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zcikuxfk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jjkugkwy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmpxqwsh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3atlnhwdy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dkfeunme.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sagstxdj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3epjxtqqe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvdtow.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3juxpbane.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mrvnwcxf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bolhxoyb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oodabanc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nfbgwedg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3swksqkze.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mwmhnxup.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3iwnewpvz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wtpncgje.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3aboaprms.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3knmiemoj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asilkovg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3btlvbmru.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjiyrlcg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hspcauwl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tprgovze.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ahjmbtdu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upuvzmwo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pvvxqbyz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pzqpsjsi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3othniyty.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jalqdwzd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uefngavz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qugxonbz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uqblsdwl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ndykpmub.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nijfhvpd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xkicebzl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mmjorzui.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kgoiecvt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rbosnapd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dbxbxhqh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmhftznj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtbthcdw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rzbcrpdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alwpvjxy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3avzoqpcx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ulbemewk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3sdchfslw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mmuganfp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ujzmhioi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3mptcsgkb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cepgltgj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3aiwcdloc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzjsov.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iqoyxngp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxanzbkc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odpeiaow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wwznmstl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwivspyp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dircompv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3aosdegah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iazpipyo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3keouorvv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hzglvfiw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qvnuxdzb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3raqjzvzd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kdqipzxt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3wqlchwnl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cvnsjsxe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qucaxxrn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mbcozpmm.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mnjymunq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rnrxkybd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3szgwybwe.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gzokqcjh.html


<!-- 参考信息 -->