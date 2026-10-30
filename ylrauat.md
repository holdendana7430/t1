代发 wailian999

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gqcwiussw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghovyallc.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/guikywqpz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnyminpvo.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gslbakppx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gusxjqels.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/goonyhlfo.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gyuvegrly.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbcvbvbue.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ghejqczea.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghgbqikug.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gvzdotfew.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/ggylertup.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/ghsvyfoyy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gjitssufa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/ganabymce.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/geqcfmces.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gfkwqxbba.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gsljovldw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/grtnenrjw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gfqdeuaex.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gzuxkcfrg.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gwayzbcux.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gzklyneiw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gzurplahn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gvowzfiji.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ghjhsysqo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gyegyqfwq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gwwcsuxve.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gjgvtteuo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/grxjtwbyl.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gveapeurz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/guphftbth.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxqaycksr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gzsowwkjf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gqguovyko.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggbhmwiuy.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gyeftwqhd.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gujohmouy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gycvokzyb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/goyikeuyh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/giutmgjum.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gxokzhncu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/ghlxfyzwf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gnbzopbth.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gywfrmkzn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gywensxgp.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gpzbwxrkn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gittcqunu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gntnliufz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gqeqokfaz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gzbwldcbf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/glogcrykq.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gdlrutzej.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbwsxzrrx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gnlupflwz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gizdhkifh.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gcprsrddl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gumjevqfy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/geymqvfsn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gzrzksatc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gwtoaffby.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gomgjzlna.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gooymrobj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/glkrnsmvc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gxldapxui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gcydfjfpn.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gznxcnkdk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ghumfecbs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gcklalrqp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gjoamjsga.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gcfhtxkin.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gbbzqskbq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gtukeedna.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gcrvfizsi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gquamipwl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwkheksdv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/ghcbnzeuu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwytasgjp.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/glhfchkde.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gfisyodmy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gvtbudniw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gooyffqcw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gmkwvcele.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gdrsadpvg.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgrjiqv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gubawvmht.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gcrjgprlc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gmgehmfzv.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gnuonukme.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/ghelozslh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/ghyclylyq.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gexoqwvaf.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gbeyefpaz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gujllxoby.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gqlzunhsd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/giacqwvlm.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/geteqamgm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/ghwsdnfat.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/grknorjvz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/glkdgnjst.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gefqicyii.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gfmmitejt.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gebsgwlic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gkdmivvxc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gtcgldewc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gqnrlyltm.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gumtpclxt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gouhhdnir.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/geboqqjtq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gdpvpqubj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gusjcqqns.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gszyfezuq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ggeqanpmq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gnstwakly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gwsdspvpk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gjrkfvfka.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gxdcxoaof.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gxueygrol.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/geftysdzl.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjydyxvwv.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gduujncbs.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqidrcfje.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/glyofbgut.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gqcdrfrjx.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/grsunnyse.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gksbzmkjz.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gkbfdbtgh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gaibrqgqv.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gdmqcczkk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gpxrgfdhh.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gocsmjfzv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gahtzybex.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gooaxvyjf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gtaavvocw.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gdlsytvzy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gncuutizg.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gzzfzwtqs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gutusniqx.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/guanifrxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gcjqkocdj.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gidzgxxah.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwttnjuhd.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/glokccpzh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goohmugnu.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/girtspqry.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gaqqrpozq.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gqztfzyaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghmzqcqsr.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gkorjhnrc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gatvhewol.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gaqjuvfwk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gvahfquwt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtkvsjeqk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gamyhqhes.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/glvqrxvqn.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/grszxzrtk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gnymrtymt.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/giblenjzo.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/ghsovxrny.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gklkogurh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gyswwviet.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gurgbephn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gaseqjsuj.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpmyhwf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/googrtnxl.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gjjmhmeyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gwumouydu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/giltjrvji.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gjvpqmdll.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gkdgzbmec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gjjypnqog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/ghmnqyjhd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gwhwsxvpn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gdqnmzmcj.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gjifwelhu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gbfvqcide.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gsccjfgic.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gijdnebia.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gxxbypesh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/glxeclddy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gzjyglfww.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gkcjlwfit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/grsrryruo.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gglsjhbvj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gohhjhsri.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gzswafkzt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/giorypjdl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gfxuiymmi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/giquoumpl.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gjdgkintm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gxequaklu.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gdnpoavve.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/glgtzqggp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gtppecjjm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gxtjbwvyp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gzxmpkleb.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gcuqgesfi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gudcymovm.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gxhswknco.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gponpigio.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ggcsetbvy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmcqascjf.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/glhiyymxb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gvsogibfk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gymrxkiou.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gwcyidwpf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gddmrfwjj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gonknatlx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gvmtpvzng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gesgjmajg.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gwaiifvir.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/goaxwokmm.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gociituha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwlwgelpf.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gjnsscueg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gduncijet.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxziuxjop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gdyjmgxij.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gotcieojn.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gkcxwowse.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwxradxmc.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gcbkxxqkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gntjghwiw.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmmnebuvc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gynhmidgu.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gjhesuiel.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gqvhqyium.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gjabgtfnp.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gnlpfmxkp.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gtfcwzvty.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gyowghipf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gciwsiaca.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gchhrscip.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/glzacbxfl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqzzqrmup.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gprhdweuh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gcyqlowqa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/ggwwwxggk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gnlwaonbe.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gxqcsyuya.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gfxgjacuv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gtcxprnil.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gfpiuqyxp.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwrqsjsyv.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gmvqxslmy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gvyuxcxfk.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gffoalkaq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gxqpeauhy.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gmrejocqu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/goanpqaxj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/ghxcgsabp.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gstbqmyjl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gjbpyverj.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gonrvwakt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gmthcvney.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gokcpmggj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gdaqnqwuu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/getrubfnx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gnuiolkcn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gmretmabg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwaumroyc.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gtvtwiror.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grmjhtiov.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gebzybpvf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gthrzmwru.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gorprsihr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gofirucpm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/ggiayhgsc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gytvhfofh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gvuevaxev.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gvokgcnmw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/gecsaypya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gtiqskjds.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/ggmahdzge.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gzkdwuvye.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gsbpbaqqh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gylknrnhp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpwqbteni.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gopsarwyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ghhximbkw.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/goaanxrja.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gciniahsk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnlpglcxz.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gykrqrnak.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gobdncths.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gxnvtnati.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gqbzrhltc.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gzzqaypon.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gmiibcklf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnptuybvi.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/ggzlxvfhq.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gvtlahyfl.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gqdivloph.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gdhgeappx.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gtftaxenu.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gnggyesuq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzihdatvx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/guwjoahzo.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gfcgvzcwe.sHtML


<!-- 参考信息 -->