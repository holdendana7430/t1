代发 wailian999

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zgsrppgm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2sovwyawx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qskojols.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2prmabvdr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bjvpocjj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hmkbibav.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vxjngoru.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2sysvdlsf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nfxrmtsi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lswjaatb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gozhmdrl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xmhswznb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aspfjdkr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wnitroxw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpexzct.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sdegewbc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akiwwdgb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jpwecphm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lejdinnz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eesilnie.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ybptgqjj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ndikygym.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qwtjuifa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pfnvxphz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2mpraoaqr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2feavroqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mjvstvfa.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gzfrxegd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vjxaxzbv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2avwlgmiz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2hcwctflb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2aukbcieq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2znyvgkiu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2eliauvxb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2clfhxvzf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bpspgqpc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qixzmbxj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mmngtzkc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jtesscwb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2knasrdrd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmzbpfx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2uugznpve.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2obzhicja.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hrbjxdww.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2clmoxzer.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mfqaxucw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mawqqamk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzlgwxrm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2agsfbdui.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxfiycar.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ceziwsal.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2psthddcb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2oqeioouw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2macuhsus.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ywwancut.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2qogcbapg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cykjmzum.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gexswksf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zngnxgnl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2apfwpdsc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dgydwfho.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wlgrynjo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fxunjwwz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zttaekgu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnswbsp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ehhvbffx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kaodxmur.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uomzxauk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2iebsqmxs.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2riqtnsmy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gzcpvnvr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2skrdnohd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avrthjhc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2dodfhwhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xprlcwin.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ruosuanc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dymxcrpw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tcwlwimo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2twmndfip.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fmgxpbjd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2nrlbwiws.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mhtibngz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eqohidxa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pslnifaw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bonxsoti.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2utpxeyba.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2iuotehrq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cuupplwp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gczjfkdi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xzcrotif.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sdykkohd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lfysewca.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wyymmime.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rcbgriah.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2tiiknvlt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zezacowy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2snfbwmzz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2hbilztin.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2lukcrhii.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gwuahacs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nkqpvqgb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vhaffxrd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mjjmwhsn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2epqrtxnc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gjoiaxqj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gnbrgpms.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sggojsnr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ryozkehu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2dmaufhvy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tjpexlng.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xehniaaz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zbyvxkmw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qtnxyvbz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vmjkxdpx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2obnsifyp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pccrvtkq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lkcxgdrp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2fgbqbvbd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aesfhuld.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jjtedrrc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmppyfgc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqhutaah.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2gjxngnlq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xwyuxyak.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bcaoqica.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wunzdypg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bqrafnob.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kkznepwp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ivfpmxkd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uwpjfisg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2crxelfeh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kklfwsdx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uybkwuxi.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nngqrouo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vzjfbmfy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fapjretx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ixcdwnzo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2wmkyxwzb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yyfsfimu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nuikntbr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwvilpgx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pkyadswf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mjeuqlep.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kpaxiggi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bharigub.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sifkgjhb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2elqrujcv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ekuecqof.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbimvi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wjikrexn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jyoaewsh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ezlnxwux.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcwkvhvw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qdknjint.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gkcsxzok.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2yvntcohb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xyrsvpdo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sqvetkmj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zhrvylce.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tibhgnqk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nbcbleic.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wfwgqfjb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gfgxcxam.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dplumiol.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hdgqrrut.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dfxerhea.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mkqggrwk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ebzungce.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rgbuqwet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2azjfidjh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2eaoclppx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gexuqsxs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lqlfseeo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ylsyaphc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rrvwywdy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zfuyxdem.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rnqmbcll.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cszcwjrg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mlnlfyzu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xttuzvfm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2isqtvoff.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kdfeadhp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkiyzyrr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2niobcerb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2frhxhvhm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2srtenxxe.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghbkxdss.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vvxjsokb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jmtcfnms.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ylvtjlcx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2bumlduei.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mspugiji.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2reazogfl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qhyqvnna.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bbrwrpze.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2avhudpla.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udwvgrud.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2cegiybyn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yhscttdh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zuqpwogm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jbtpobpt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2whrnavpb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2szfniejw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2riaylcpm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2unrnxkkt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kxihfhfq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nssbskgi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2sletjrhv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2heqxqgiu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ckujofbi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bnspgehs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ycmdsxwa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jpwkllic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vkrzrcwm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qvbxdsyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrxelmbf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2krhgtebr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrsgruvm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2thnqmobk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jhpetkip.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ljbvashb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2izwwutnn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gexpwzew.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tasmyfjn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xxmqeuyv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mffosvej.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qtyxbykj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2blifpzzw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cmsglgsq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fzfzkswf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gwbahaof.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojmvddng.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2brbbjuue.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wxglcpog.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zyrmzrbg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bcwgbywa.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2evlpvdrd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2botkftdw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rwhyxrkh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2iknmpyii.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2korehnzw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uwcrmszv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ctijmezc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bqglsgpn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qwjoxbrx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uijqoqkv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2apxzlwnh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ulkyrsgr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gqunnzjh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rwvttcvg.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2qcldpvpb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jbhjaaol.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cdfjuluu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sxekjjvh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cdnysgkw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zscpttqs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qtkgarhq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cejhuwxd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2czdscwpf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhqfblco.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2atmlvpvc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ebqjdhjq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qnbgioiz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygmnjban.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vkvkippd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hcngmkby.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yvzrstvz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2frshsnow.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wivkcxgj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eiidjjox.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2pgjtjjog.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2sebdydbv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2uxymsouf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2umnysjnt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhosqwls.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rexhuqfk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kjkrykji.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kweylshb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmxwibqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvxivjbc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qsutbxds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okyqktvg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sxvpgdnu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2sawazbeg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hzivhgxb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nfbprlpc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bvzeqjok.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2apukbrng.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rmyzxzvq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ozpcpzqz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2blzfgktv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2aqyzmqep.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwzsjidk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2fcmytjeh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gjosttoi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pygujytk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ggmmaezh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2moypgeaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dtmdrlyp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jsbfulni.html


<!-- 参考信息 -->