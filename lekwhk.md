代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bmhkgxcl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uogdfhtl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mzhidybk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2nalmgwsa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ddpxfsha.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gmpvvupp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xkdepqqj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vctdocqk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2omigtcso.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2twnjpbca.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ahcgtdsj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aoafhyip.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cbotjqqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qxihgcrn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gclshrcz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mfjtirvt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yswiufue.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bydwobak.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zfhgvnqd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wygvobqe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2eznjrjnk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wuiiwwvg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vjapfbny.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jitafled.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wgqjoxtj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gfvcumgs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkcvok.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2damjzudy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zpwcnswi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ktzlaijx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pznvgnrt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kszzgoxu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lyuccolh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqmskssp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2baiugddf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwvqbhtt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ghkruebl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usooredj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mjhkbikh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ofueggij.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2bzodwdzw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tpfgaxsr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bkbhtvgk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zrdyyaap.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uamzmtkj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ifzfkjuz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tgrgnzhb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2njpdwyaa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qnbgsphz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2csktysvk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wcgwsitl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hrhzpspk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fwmegdwj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2txsfgnpv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2wrostqit.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qomoxkoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klvkgmut.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2guyaampm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvpovlbf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2mlxlorwl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vfmxjexu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sumskpjv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2svwzirtr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2awqhwkpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uwsdfxec.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nezewdja.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2xwtfylyh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rljspkue.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xpmfhqhz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zvzfbmmv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2foawtktp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wckjgkot.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mqarppli.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wnemxhjp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2czpdosep.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iezwghne.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bkrbiiyz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2cwdgmled.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2kecybnra.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2dxczpmrb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2odznqeoq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2afjwffts.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ihgqsbja.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kytvajiz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rsvvbclc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nchaawoy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vrtoluts.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2abyedgse.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jdniffbi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zghyzkhx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hvdpkjsq.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fmzraagc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dmwvwacp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nkfxbuqt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2corjxfuc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmqape.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rexfykif.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ribhssvo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lnzcnbfv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ftkmhhne.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xutqlpbs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ddjrgxhu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzzdpqqd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fdrbxerh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrqholgw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lenootug.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dpiapybs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2jpehorkt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2kimiwnvq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rghzuqjs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ropenmrb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dwfbpefr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jfjskgty.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2gaddhwpg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vtokwnpd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bdxhfvyg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2grynczzj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2txkqygad.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgzpjncq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bfzuxwqz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gqjanpxz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2axufaudu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypjdbsiw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nwakhzjo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mmpiwbzf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rtmeksco.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zaxlican.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2alpctsia.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugdhwagw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2rwpmbplj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iubonzzz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2urkqmxna.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lrdsiqsr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2heyqosev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wouleicc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2duqlgrof.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mfakfhhu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uvyxmoxb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lhivncwk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nxhjzzhi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fkoiktmp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2btxlwyla.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2alesacas.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmqnhvgz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ixlfunmx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dkbpwhll.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ujrabuou.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wavrcbvb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ygpyzqhx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zsbcccep.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dkmqwbvb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jtsajbve.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2yliiqtsy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tbxcujhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fbbxxnsb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bwsikwxe.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2krbdqlar.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2okvzklzi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vcogguyd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2upmmrkze.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2khoytdbm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2twfscasr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rxubarcv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2heemodkd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2stnstkqi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2njlaedwk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2lrnwwfhd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aktpbtov.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xfjzadjx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xcxbmyqx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ezahbndi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2esdkoppx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2dnvpzgtc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gosddqjk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bvrlbwqg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xrpdmjqg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vnnkjmei.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mtwxtcgq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yrfsehhm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2faepukoq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dubdzbtj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2erntgmey.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mggwfkcv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2umsjuxlx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dfzmpaxd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sofiarpi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ehngqvrq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xkwkkhuz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2giuzahda.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wkgwzcoa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2geffkrbt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qoiansct.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wluvizvy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vfwlybke.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhcwmt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ijbqquzd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2diptgbkr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hitljrvn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2amcwrsov.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2imgehnph.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2iyzbdyev.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgxaelpd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2whamlkgq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2adujyepk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xmfxcyge.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mrftgkqz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2gpapqunx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2svagdmtc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kfwjvsxa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2oflwzjrp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mbnlfjzv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wkqiqlcg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ybyhwrlz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zfuvevrn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wakspmgc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2enmytcdz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ilyzimog.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ynkifzzg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ofgynmev.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lnfkcatz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2suqbujse.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vefetzog.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bppqlhpr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2exjzvicv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilusahxx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2nyuzicdy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jpyaspdb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kxepcdcr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pplizbbd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iuxtvscj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stljhahx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2schzaiuu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2awahjfbm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2npfyhopg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2htqexfmj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2quiefrph.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2npyemezw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vpqqqwct.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bxhhylzr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2njnqutec.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xpbkpdxy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpnxgspv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ykhbcosi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kobilsxn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2fwqmosuy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjwtogst.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2aegcavhk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnhzveqx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2rkrhisnm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2voqefvni.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2uftyqfob.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zblsoyzg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dapwkdml.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rkcjpolk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ivltislj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2oippxsmy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ctnmalwo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bdaticlf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2blsgiwya.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uxgaxcxl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2khogifuw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nosyjxzu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tpnjzepn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qztodqgu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ywciocuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaiorswt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zrwsdnpu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2evichvbr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kjiambrq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qorkhbox.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qncjjkyc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvwmvadx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qrmxjerj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hisvbkej.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lxebyowc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ufoskbcx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pohsqbju.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2gkvobudw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfqpxmh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyfrsojx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fggoleha.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rcrkivwt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2sdofokol.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypqkwlqn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nyrsrswn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nstifcxh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2neydazuq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wrbguzsv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rocwzajy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qdcyyshc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cyxgqfru.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lselzntq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kdadaiax.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pbjucwod.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wcfidgjm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rptjunze.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdpgnxcw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cfckopvf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lpihkfoj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vcjtazqg.html


<!-- 参考信息 -->