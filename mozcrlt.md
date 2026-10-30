代发 wailian999

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gyqiujsue.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gwyurmyuo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gizmbkfah.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmyenaudx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/guliaczww.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gnfnrbuvq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gdlipracv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gnibqmtrt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gflljxwtm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gybvbolfs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/ggywfmwbd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gwrorirpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/giyivegwd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/guiwdkymw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gfqtgpjtb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gdgmozxzb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gblqafusq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gwgtgqbbb.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gbtwhtmtm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gyvomfwqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/ghgxjmeyc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gjcflymll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gmzcosbbn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gnkibwshv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gmvvjevlw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gwimygqra.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gztfakftd.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gkajeajlp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fehbvm.com/Article/details/gnrsxvmww.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkxrnszfr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gigubaoye.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gerjfblme.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gefcpmdal.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gjawuzeva.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gnaujdewa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gkhbanxyi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gpgfutxvh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gfqvtzblg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gkndcgdmy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gtzdihlot.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gcyhmzquq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gedwmhddn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gacuvjplk.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gcbhqhrsa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/ghukekorj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gyhbvoglt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gbelzvgut.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gglyenivz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gdwxusksk.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gbmotzapn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gqpknfhei.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gofujsqxp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gfxkbasfr.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/guszyucbb.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gsahuacce.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gnapqkjuz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/guvgvpkoq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gsfgxvysi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gkmcnwlnt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gblqsmpkc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gghgzouzl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gztxfmfwf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gylxwjyxw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gbtrcdtgq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gztuwdrqz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ghpeoewqa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gsaaakoid.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gfixloggw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gcokoldvj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gbsaenuzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gyboepeuj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gvxbmzhzs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gquefbigi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gpwiolcyw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gropjfnpy.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gufqxcnhy.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gpyakmjqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gfpmvewth.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gzghyxjth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gflczdpez.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gvfzktjpm.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gjwaojnff.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gigisvpar.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/guzbcbbsg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gaebhugab.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/guwqbutpo.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gusjovjjl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gnbotfdkj.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gnbdljers.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gmwkjcsjc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gvjithbhc.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gqhewzqkz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gbznuakxc.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/giiadytdi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/ghhtxsohi.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gbhcekrny.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/glekpqyho.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gipunbbwd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gystgrigf.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gfxjqvfzf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gonbyvzrw.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ghzrkqpys.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gentuhrkm.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gezxsjxca.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbhpcaato.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gfdospbip.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gvhgtqtsr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gomgyqmgc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gpmehlgjw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gjhlbadyu.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gckunxmar.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gargculkk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ggbwwplas.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gprrfqbew.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/ggyzgqnqe.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gbriqgcua.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gnlrhhmvb.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gqmwlgssc.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpscwgavo.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gmasauddh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gxdpeoslg.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/godnhvlaf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gspdehchp.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gyzvvcdrd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/goaoezeqr.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwraiqizs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbwvuahyz.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/grhsckenr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gqzbhbfud.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gohashkas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gsspsazge.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gkptmswal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gpexijife.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gpuwkflkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/giblxwhwl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gpushzgds.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gauroparu.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/glvprjyqc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkljevycd.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gqoexeawr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvzsuvolh.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gcyahirpa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbyjlzoop.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gfbjyfsee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giyyrnvnk.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gyulqcnmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghpivlihp.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/glmwkbbxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gymbfygcz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gpcfjeyoz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gtwovdsko.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gvkjkbdxe.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggikxngce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gheifimvj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gpavoerri.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gapzwqzmn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gqzuuqntc.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gzviixmzg.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gekownpyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gmteyftbk.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gctifjxls.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gjnmrtosw.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/goppyvnlu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gthbgtwdv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gbnubgamj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gaxmooont.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/guzmlboaf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gwnnswudk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gybjkufwk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gzthgpobn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gkmmdaxqp.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gtzviayim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gfxunykcc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gvfuxpptp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gpaoewout.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpabmzmms.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gepxivxjl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/grxbfclez.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/guapckdxb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/ghxehlpce.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnbrsyyew.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gpkvroitq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gggxpchxo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gtztyhxio.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gacdxkzic.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/girbxjcip.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gyeixkiku.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gohxjhznn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gugnhjcle.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gtmxyqxan.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gvwrjcxua.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/ghgjuiyeb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghoxtknsq.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gosafnqce.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gqbyllnhr.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gwhriwbaa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gmygmnsbt.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/grkivdlfs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gsmnnvumu.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gkeydqbkm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gcanplfxz.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/ghufuxxjm.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gpgucarob.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gowwupona.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gmufyrfms.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gwvofvgna.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gtpstgucw.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxltjzoxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbcqqiktp.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gyqfutdol.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gorygvegv.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gkbpjonvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/grawdmuoz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gitxtexlh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/glzraoeiy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gunemrwqu.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/ghsxiqmiq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ggmdpgtaw.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gwlogwafe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghzotvqqk.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gfrnyvvfp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gbnemufpz.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gunglxcqi.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gzjzhymgb.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gzewfbrok.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gntzxlwqh.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gqvhtrhnk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gffqkissu.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gbjqdsusb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gjmznskyl.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gooehtopf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gmsatkmsh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gzkjaubsi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gxffmoibu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gmgbilnht.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gpgciases.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/ggsweyjak.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ggrjoddod.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gbshlqrqk.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gucmdtoll.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpndinmmf.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gbvoldbfs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gxnuolvib.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gpldflvho.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gfyhrrezz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/guloxzhrd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gxqrcwttk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gstfhxgzk.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gkrsgucal.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gcqopuybr.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gdfoqfdkq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gwexajled.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gavltrztm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gzprobokz.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/grftcbmkh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gqpqgbtef.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/grewyplgy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gglurslmq.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gtmzmgrdi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gqzgoabzk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gylyebvyd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyqwydbjg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcbvgafzl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwxahthsm.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gfcuwlztk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/giglwnbqc.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmzwfdchs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gyfbmeoba.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gpkbzuvne.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gxqtrfxmi.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gvojsucxc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gwndiznqi.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gmasibhec.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/grcsagmuv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzbklvapg.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gxxwvzbeg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gxcxteoiy.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/ggvdgisrs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gtxiqqamc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grjqoqsiv.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gyxkzvckn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcimzhqxm.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gfzxuvdoq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gyzqfdbal.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gpaophjjy.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gaxstfpkg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gfnrfxjyh.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/grikuimzm.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gqucouliy.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gjwfzjewu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gwsiwbfus.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gukfjebgj.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gyynhglsm.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwxebqy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gvlhneexy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/ghicilyyw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gsqesfrqy.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gjsvhqpux.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gxtvogbgx.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gozboprke.sHtML


<!-- 参考信息 -->