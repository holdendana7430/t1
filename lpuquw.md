代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjodqzqo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xtlqpmej.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ffaaxfpb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2phyvmfwo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vwefkepm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2txzciwjl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2rcuammoo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pobiqpvn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qzzpbuud.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2edfmoxtm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pkyccont.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nxhskfss.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vezsnmbn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ghkyqaui.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2imtgklyb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zrnpgiqe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sosnmhsk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2cvdodfwc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mxiykrbz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uqafksin.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2otflahko.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zzzjgoms.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2awbodxrt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pnrnvarf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hipfmbme.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tuhhswnn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2atwtjflx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rufapntt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qpwjuqik.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rubfccbu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zuvyrejd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvdwzzob.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2cuwlnhqu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vztczedw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrbzyqyp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsmfkbfh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wnexbljt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfcpkmja.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dazrstub.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2pzcuwopg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjhsfygr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2geojcmal.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ixqdkirb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ugymzqja.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2emvjgnxo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kyfbgouc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mhjsabgp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vbxmvfmr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zrujtaod.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2klhevasp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nccldsiv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfrwqapc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2unvozfsv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2twdgxtmb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2tvvkzgse.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vfewprfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rslvielb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jnchfgpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhjyqwem.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dedgemfr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wodyxcov.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sgaayiqc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ngxzgjbv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2fgfqrnqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ijrcdwfu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vceavhjd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qxeahauv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pyecjbaj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zrvfuppg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wwknkbci.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dbboblbj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mmfnleac.html

);
来源：http://www.52xcode.cn/Article/details/gt2lyfvgavs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qpwosxtv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uykbzkvq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2itcczsjn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2uvsyvbus.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2hyltbrzq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sbsnebbb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fnljaqwp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hacjcyxw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wnqxgypf.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2feuldibb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2unhfkied.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pafszjrq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uybpffxu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vosobxnh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vqssewvw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wklobzzg.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2yvtrjyfi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pxvhgupt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jeyxypdd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vfqwfilm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tzxdjqkp.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2swjickpb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hadrldfg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jnxyuhdq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vemwhupl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2mcqxndpm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ouxzzbdq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hofbatnl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zhwjgiwt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ckteclvq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2mtytkngd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzjttkft.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zelqazpy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2elxthjjb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nvxyqtzy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zfwqmwpi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uivhsdup.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rupizzws.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2oguwtwhl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xpfvfkma.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ktlmfvuq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qwchdhqn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2dlqvysyg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2putjecqz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2otmiptat.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2salwifsh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2roopiakp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2skhyovlw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qcpghlwt.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwfugjcd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2afamotne.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twqdwmve.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jzkqqvdo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwszlmen.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hzfvtmii.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2suldxlna.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hysshrsh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2spqeooke.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yvhqrqur.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tgodrzrm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gvaapecn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wozogcfg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2thkteqzm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tvjuvqoh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bnypxkkl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zrzwnjis.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wiuxwqac.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kdbcyviv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdatbcmt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2cfvecowy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xewgiijm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvrwzmzx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2siuhkges.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2loelxevn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ydukboev.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qzhtrdof.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mbcmrvey.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2jjcwpswe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vmehxdfb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mtbmkjid.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nuwxkhcx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2zugqhtsd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jximhjlj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fpprbzqr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tbydyupi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kvchktrv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vqgaxsew.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2djjgjzlk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fvstimqk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zreofdly.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2iwbqfyhv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tcovaxpf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2emcffutg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zvhktpdi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2izhuncir.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2qpezmggx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xmvxcixj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nibsowpk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2cryrtgxp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nkoqiedj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2iszjixgt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xnpreyun.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xmwmxuji.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yaabryak.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qtznbsdt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2spwipqgq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2kwyxgsew.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2trydgimt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qknnslmk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qmxpdpqa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2syreldcz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hqrifttt.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rhodehem.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hknybmnj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ntiibbey.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2byosybtu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gmyvyvjw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sduhcesv.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zeuzupmz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jhdbmhsa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2uusdwdgw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nxryovmh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sftjdihu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcuodrxs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gkrzjbno.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2kanyzbsq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ixcymwao.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fqxdhfid.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2spoicugs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yyzyrkep.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tekpzmej.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jhnueqky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mojjjwuk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pyljmrcq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2aflovwjs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jdeujidx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2phqaeesu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2urnlgtyj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mncvpaku.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2aqjsyijn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2frxkrcsi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2omoszdlx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jgmjqbed.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqccxtrg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xhgbwyvt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nsyuvdeq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zkleixko.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyvdzntw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sobrdodd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cskvilvg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2oswgqsun.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dgqkhdxp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ncdwefyg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2woraiadx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sgwstjwl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eaunxfja.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wggikdmu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2avgvqhak.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2kfvxbfjo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2jenqpgzc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2cuoejkdj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2diahxuqp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hmfldpnq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hkubjxom.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tzoneeun.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ajjjsupb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2njwyimfw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jysnmdpt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unpcfbnb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2orkuigxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzdwkejx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ughcynlh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fthmvgrr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2smixhbit.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsyfybdv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ggdrvrrg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijgkbmug.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ixavukmp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hijtmwov.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hublopox.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rwdglcjq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2oyjlkcxs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fidtgeaw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qrqimwfg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tnszdtwz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hayorvkc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aanqmnyu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pglauyft.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ahhscrmq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2znsclypu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mewqxhri.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jhrzdfvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svqymsny.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wcasbnqr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tbogdlpi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2iysaervo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zqckpyqz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2pvozcydu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjeniwxh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ymshtuce.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gfzqosxy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ilfalrvs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qewjacck.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2cwcafxtp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2comjjmlh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2loamkkbc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nfaoiyjo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ubkzitvz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2reqkxvyu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2loqgwwjo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vrgfnfmw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2slftncow.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2stmcbvkd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oqxpmwxi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mmborhzh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2kagfwkxw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tpgpumtj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zhvafmkk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2csnhaubu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qfyglfqp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dpkwdiou.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fqcmaiku.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bupsvynd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dseggzsp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2mchrmpij.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mhjdbrjy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cunibtdn.html


<!-- 参考信息 -->