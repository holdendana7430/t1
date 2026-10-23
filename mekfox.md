代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xznofibe.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vgqgdyos.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mvvsifhi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nmrbasui.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ckkurfup.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ritzcxgl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dolfjnmt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzdcyzjv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zytvreou.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qhcwctln.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lculhypq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3aczhqoji.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frsiqbpd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3godncuij.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rvrpdcut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zownaqrb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kwukiiam.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvpydtcf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dshhclfo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gckpdsae.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3kycqsecc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ilxtwvpt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gnpgyyqb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zsxkbqbl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lozwsbnz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mjsxjqva.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xmuvimpk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3eqmnelxc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xlyidweo.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ovbkemce.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pkbhwdab.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3upndlxcw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3czulmtfg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3uaydbnaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bfrmlypz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qsuvjoil.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3blthmtgv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qytybptv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3klyvupov.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gjerbbvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3heaakrah.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ihhojfea.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ngzjphox.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lcpkzgbz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ghohjkgi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lomhknln.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cearqivd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciwcorka.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3usigqfrx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbxsikhq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cmsibsxk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cqeuqrsv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sbqumfed.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tlrpifpf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hiqzfvdx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vvsftlwx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nkocyxqy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ccntqekz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zgygtvlc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3prdrjgso.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3muwweoze.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wnfyzkrd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jgaphdkk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dxrpyyxm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vvykkust.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vkgmvdwp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3onuplmxi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fucbcbck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xykxared.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3rqfdubnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwvmlefi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mbkdjsll.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hadcpvbn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fntkfofi.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iczpmuww.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gawpphqo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ducetamt.html

);
来源：http://www.52xcode.cn/Article/details/gt3mcnoukyg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3joryktri.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3rkfarlwu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zoziqtji.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mhpxhwji.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jnsyyvqy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vubysmpa.html

);
来源：http://www.52xcode.cn/Article/details/gt3emkobvcz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3nxhmjtko.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hfqkksss.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3uqqkedas.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dcghmsyy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yvebwdpx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3axgavzaj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3evzsfsvc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3efpkveoj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3pvbpggcu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3iwcxyoch.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ybytapcj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ihleemrv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3asakgair.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pemgiyiy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3igcxhxlo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3knncpoac.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3olmichqz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3aficvfnz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3thsdocgy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3chdqzcos.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3sfuitpkm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ooyrupey.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ltxmeglr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jzgpyalr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3txrhjqzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3utrdbanl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gazzlgmi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftvmxwyu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hllxqrpq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ziyhmlju.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qctqqrqx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dspqzrph.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3evuvcwmr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mheubfcc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kswslnnx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ktdztcku.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tdhpiciv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjmysznc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ivxcsapo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xfmmvujj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vtweucsn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ltjdeezb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cmrzawdw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3remukgry.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mkkzljug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrplwfph.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hhzcdezu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3oyaiomwb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zthevpfc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vipmwikh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3yrerdjam.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crqpledx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dfeygxcc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pltcrpev.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qvamjaqw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eanvcval.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ptdqwkod.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vwgyqdmu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3jhkjqtez.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3blmxacvs.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bzaraeru.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3onjcuswc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vzogeqbw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3enxgpuka.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3pucefddd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3zqhbvzmg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dugeoimu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dnmhsife.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3erswmzms.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3okpyfzal.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtpetqxb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kvprsvav.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3bibwvpis.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pflaatju.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3imgbsfym.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3nruqqbmn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3anashpld.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3zsgthihc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xslxygou.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ijiaopjf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pdjcyqpg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kpuxlksk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wsgxkdyd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hdimumvp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3corzdlwu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3omvbhyjm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vevulhwm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3aehhlutq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xrfkheqw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fvszrfht.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3svrkueue.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3wskkjoyn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3atfffspw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zedsfjwc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yygeoaio.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zrhutukv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lncmxjzf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mjdmesiy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hvstccxx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kpuutkna.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ngdhwkpv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aebuqftw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wfoijmdj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qoivcyyq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ilgtwkkh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rnibemac.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mgvrurue.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3coprivbk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yieeibai.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rntnspqh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ovnfdzkf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bhjuszkg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nedlbjvs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ndqqgoex.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3iyeermzw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xuezshvc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jhtrpbyl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3orojkxjl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gmuqzvhe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwcgkarh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ezpvgqfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqphlyv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3iybpgnub.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ywhkioqr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3boardjox.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xxtxippn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3affespvj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vazzktzl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ljjhsetb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tdkedwmu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kdyuipho.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rlffevjy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3aefvkutd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jdvdtcun.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ckcicqqg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ztqkiaee.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wsqtdxzu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3wmzclaqr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rbbexrio.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3tuqpqcct.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lytqjlxm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3obizfuez.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fpakmjjv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3frtfkjih.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3spqfycnt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bcydfved.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3sweqkgok.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zrvtrtxr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pgifiweh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ylwxbpug.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fgxiyrqp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpxooqbx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kyxypgpf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yfirgvyw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nupknktg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aenxfikb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3igmcotcm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bthawbzn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3szzrdcug.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sbupomxs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xomjrnht.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3xxezdvgj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hgutmwpy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fagytnho.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3mbesshne.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ephpakde.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ktnhcjsu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fwuftbmw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3miqprycb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qlktbgyj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oydzutca.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qevmasrp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htnioand.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3czdyjofq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxjrrcwq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fmwskkkp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cwckblmn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3szedmbqz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3fzemazxh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3zlatvuoj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yftcwuhg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bujoxzmi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qrypjnjf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vkgxnmtt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kgfmpnyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eioseurs.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kjxbhdze.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ycwqjjha.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nfggiyfk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ttpoowyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coxmhpsm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3orwafjea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skaeqcdl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gtxwklob.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vrtaueij.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3oyoytwev.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tprmwldd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wulnyiez.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kvbhtqlg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hstmxfmv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3beayiqpw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xqphisbi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tbqmztkj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3svhzjvsf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fahasvns.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pxyjiwhv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jayzgikl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3epfjvoos.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kdrfohsg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mfqhamdp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vhycyhrx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bvzilhtr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qhqhsbti.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vdwsipsd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3yhcirelu.html


<!-- 参考信息 -->