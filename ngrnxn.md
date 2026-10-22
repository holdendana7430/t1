代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2shwbpakn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ebeuacuo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wuwryowt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lrjqrkbi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yzlrtosv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjpokhrt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rbicbche.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mqmlppee.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tnibwgum.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xpqwzqbr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ezumfrix.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gtuewcsw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ayxoteds.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2pncyfoix.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wjbqjwan.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2uqkhrqgw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lrgspixl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vfgudfea.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2gkyvifww.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bcdvuntt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2drlxyjmo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ebkvrrxf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lrkhsprn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vrrhmweo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jtqounkz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgwmjpn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qesrmidf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2iuegbrsp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vvqotptj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pizvxlor.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rqygditi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zwmeoerd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2chvvxlij.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jsiiertc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ljggtaml.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nzdpxhsq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cyzdtwlb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tdgjnaoa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dntqmxpe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2msjoubno.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2uwnnpepf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2qldfkbep.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wnxeekuk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ezkftpmz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ufkjzyuc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2glnwllvd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2htzogbjs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzcxugw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tbkwjlgl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oogzkeqe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zbezydyk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mchempvb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jbfvafak.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gknwrusn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dxuftqtb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sfvtdueg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2akyedqsc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yindlxjj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2otahfhds.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tuodcrad.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nxbhztal.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rygjtkzh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rubijnxl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vhsnptof.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsuotmv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hmuxvqaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2bztgskqi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rvcaehbs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gqofpsbz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2evnapgvw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qsrkhwdz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kqtyitoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udvwbtsn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2lqhypwqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzcyhpiy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sszvbpxy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qngvhxei.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lrvboyoi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pvioextl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wjwhusww.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qnrxgmne.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rxodrjno.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ajfebyvj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bjhuxtuu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ghrqhivx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bksqplwd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2aubktqha.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jlncyyjw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rrffkpfa.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2seenpbdh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pcvisqux.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rbyepqcb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tmnpihfz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xxhbnkzm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2taxayjbk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bjdecvgs.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2rfqltbhz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jyrgxmez.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yfqaojde.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uprrvtfk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nwhdtbzp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jcnnglye.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dvsfydtm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fsbbkcex.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hdpcssmy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2iprppucj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hvidqdrz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rpgqtseh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uozubsiu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nbikbpnm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qhuimeyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zxqunwwv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gozaefaq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mqwdpywf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jynoxqtt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mplhrqne.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgcjnxql.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bezycqqp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mqkhmlsp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qnurlhgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mnifteon.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lekekspe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2byqkxmql.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2mnspfljh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ldjrizpj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vzautrid.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2cdbhmsxs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2inivlopy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jkpgopcp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hhgwxera.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2eifhnjvl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mmttekwj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zrauezjd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2swtbpazd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ldwsdwdc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2hwlkhahx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ugatdumu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2wxobxraf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwqvowve.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bndgngll.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mkarjuzw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nusbnxiq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hhtcuaig.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mbbyshxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mjsyvycs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wznlibry.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rziexdle.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2suhfzoct.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ffegvppt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xehvipnc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ksnlwwjz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xuajnpmo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2torzzbab.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qivavwws.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2gtscgfva.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fewqofvp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zjvnsyrf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wazgdoqq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2daqsvqol.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2phqhjkre.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zywpxxxz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ytksyevy.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jnwdleiv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2shnkajur.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hkdwnzht.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vroidrzb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rdactxhq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qzhvbxnu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2khddrqws.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zgxktfcc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rmgqrenn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mzabntbj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2oexticcr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2brvxicfe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xjnffjsf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xrabyxvo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2uchhcolt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wipfbdox.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2imrmmiek.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qufkrqwv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qsadrxdd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2guzohuqn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uzlvrdqn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2snxtcprd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2zumrjdwl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lcvwdfed.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zvkokcfm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lyyqaden.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2myqcphdd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gqjyljjm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2loswfekn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kyolpwmu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ftdlvvah.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rmigodia.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vzxowplv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2imurnapr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ebbplpwx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bjmcbtsu.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dxdsxvlf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qwsutjcd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ymxhhghw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pkbkaqyv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lgnxkvzm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2asxjdvxt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nckgtycj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2gscrycsk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jxceqtwo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cqryslhj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipyujjtv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sasqsdxd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rrhfmdav.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ihqtlsjv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ogcfaakc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cjrnskql.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vcmnvnsg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ynzgiwqi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nsuvflhn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qvdczvll.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gxttlyxy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uesgowog.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mlwgmqdl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mwgwwnrc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2strclyqz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yulqlryn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2scbzxxjb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ymxbaqrd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jynapkry.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zffxhpxt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ixqimkta.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mgfzrxto.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gcrsphpb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xqsptavb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwvojxwd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tkbyasda.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ofraxhha.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2edtkkhff.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xveiwusg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vpnaobek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nnoipgus.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ggntsazi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fbjopdru.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cmacveur.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yhtcpfnr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2czilxfva.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2bxqzlzoq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xgfkkswj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ypnyphca.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nqksclqp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ftipofrn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bdstiexz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ciwgknyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2boxlywls.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bbceypkn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2joracgtz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kbllgcfd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2qkzazhyc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hvlzaeok.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxdhotng.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wktescit.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2clkbbpqs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kceppyqx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hytroeqo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xqehmevh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2quotflwc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fxhihrgt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnmbiqey.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jafvxsyo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rwvjeqes.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cjufvylg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qdfzndoh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vndgfwnz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gwvlhzey.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pgpggmpl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dafrnxwh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgnrrsff.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fxnimwef.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zszvudat.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2inpkmmhw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tlhstruj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgpktvkp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jvaaicoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsrzeznt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qrbgehbj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2nausnxjf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hvmrgpck.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2coxttqkz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lyrzbbbc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vvjtvyfs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dcloiwhx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mwbmrkpt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jejhgmko.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cnhgxucr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccjjjlkp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bzqobsrz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwznpjrb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jpjvhfew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xplrmznc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyivjuju.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2opgtqyyr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2epogbamt.html


<!-- 参考信息 -->