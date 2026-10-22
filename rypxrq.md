代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2punkchba.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwvpza.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iswknnaj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xqtawkwf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dpozgxbm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gsyjdila.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eswoilrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ijzblqeq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2inmxqgvd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mvknvkps.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ctgcxcsv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xefiyzzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2zkrmltem.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ftozhgik.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sqiatyyu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sogghilo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fqtsqham.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lxvwuhve.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2aztokvrn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hscaunpc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2osyggsho.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jzqoayxq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mndjgiwm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wuulccnj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2omidujrx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zosrzyge.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ktuaasfa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2auniltst.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zspqsppa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ggcehatz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahvwarcd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lbediugg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2njmhclxo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2unnoahlv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2wknjccxh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlvzuluc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ypqfibbm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uucaovep.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hvyccwey.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yllwqjdi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhimxmv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2minrmhvk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cajyvjjs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2uandmkrs.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2tykkbtea.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2crghbuxi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vggxzowx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2mxcndtor.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2fzfguhpb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xmsmmemo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2slhnmreo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ctrombiw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wvafrudj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qjrgcsjo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2gnglrdvj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpxnirpl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2isthupnv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zgiogvle.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qbavvysh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jftadimp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usqenoxz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2sfiumtno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqzclwce.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yvemtcig.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2osupycpc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lovitbgo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2sxhtlptp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ozrfrebm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rtqqrhsg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vvpqoqdn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2enuaqrqh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2islzehsh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jtcgtoqw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vampdvvq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yjbbcohr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mlyvgvem.html

);
来源：http://www.52xcode.cn/Article/details/gt2lxyvsaeb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2owebllqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gdoecvlu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdkqiwrz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ncgohvum.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2njmlykcy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2oemlmfdu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nemupopi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pqejdaol.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2xtexlclk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xfanabir.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gtkmkxtc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nrkujxwe.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uetejdbp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ofcvnygh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ipthxuob.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mnhtuawb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2chdknzpv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2psylzceo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wbkbnmir.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2bdxrmoqo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yxecigfm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2aufiqwuk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lqztqewx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vchmrpvj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mohppeck.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eiepdrxf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kiseivbf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzqmttwv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bpspkwhu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2abmakkuw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hbivrhfw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lsllvazt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgwzzw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2aahcimil.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ajjqcmxz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gleqphbw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2herpcqkz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzutaips.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fqimndij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uzyrmehf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ntltabjh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2znvirjgx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gykuzfwc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mpavadgb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2llfpixvk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkgsnjmh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2griexsis.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fvpkxbxv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xzmwnmtj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxocvpl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2muuzggtq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zokurjtc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kvrzxzyi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zmodjjcd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kmdgojds.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jobzixbk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2tnmjkamc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jtjefzet.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wtemgoli.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ksuicnho.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xvzkxutg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uqmwxtqd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mxlmqqvm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jevuuxgr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kudgbrad.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bhdqagmc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2styafljf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pfeftuml.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2utcdtgpo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2shspbqej.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2atqkjspt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2kidlsjhu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2enjvxmto.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2rmymqecg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fsvosmtl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jraojqbc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2esxtcyxm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2prqkgnml.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2sivyeatw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gmysutzj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2tqwcriax.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2eyjwnomx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2fnpaqjlf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2nxcqexek.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bjxamtmi.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jrhejlik.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yeuzcpme.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sknoqmug.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rntjmvpd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ssnfytxa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ovdplcfn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eglotppe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dpyjoxra.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fabcgpye.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mzvesqit.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cyzaboro.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2imtyedrt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gdjfhlgi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hqqlxbyr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2scqcordw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvrnjmt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kwjdbhsy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ezirmpjc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dbgllnkf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fcovsanh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2irhlfuwd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ttzvzrpb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2asvgnivt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bgcdmelk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wtdupgnd.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ysonasmh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ncsyiguq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yakzjmeq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xzqnrhcq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2unqfnxui.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bsbslgsh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lqmjwlbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fcwkiyme.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kuutmixc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwohmfws.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cbwzlsql.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pwgqjytu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dunlfhvy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tsmabfbm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2sibtsrsm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xalgsjzs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fhzhizfh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rdwdhvoa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tpxipkdi.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2valmprob.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oiyltlzr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pgvijffj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qwprfbjx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zeexynin.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uoelrhdb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hxeuipjd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lcxbyzie.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qgaavuld.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mwtjxttv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qgbwmxgm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2dpenkkpo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2muvwtkii.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2iiznijti.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2smhcrbvh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dtzlkukd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rnwwywml.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xkcdgppd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ygoldedi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fbwkktot.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vvexjmni.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2btnpuqiq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glejjomm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2potphqcr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cofbiiov.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nkpxgjmh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2sddzbwgh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ffiyoagg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cuwbqyux.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2luhajomz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kqtzsfqx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2hpthwunp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2emyvwjfu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gayavqfg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yyctilpu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bspytlsx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jkosblsu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2yqyumqfs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2opkphbpi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2grflumke.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2krpyxrve.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iyxsujey.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nffqsrsg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqzpkxix.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uzcmimcg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyotuwxl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2dbwcritq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kcckrfnt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qgenrelp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ovuixigu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2caataitd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hjxivewv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2hiqbsjeo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ubbtfadc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2unlzvqyv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iwvsnqnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xuinmihd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hvisrgpz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zchaggfy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pkfcxovv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ihbccahs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pijpmeaf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rauhhbtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rswjspoy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hwoeunwo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qlepxpdu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xbdsyhtn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xsheybrk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2cjdjhgqm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2apvpiiwx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ugwonqfo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqzwvybv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pnjrbdzz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2elhweixc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkdtoa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zfvewkfp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhxzane.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbsucxpc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jankdchk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ewfkcpog.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2htnnsuep.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nqlpsqwd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2whpxjjqt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fkmhexcy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bxnvxxaj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jzoaixgz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bqkyhlig.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ayfxarfg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xwlhnici.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzbimvu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uuikgywg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2fslhxsgl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ogmukojk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jcgzufdk.html


<!-- 参考信息 -->