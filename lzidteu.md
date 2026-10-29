代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gxzabzycc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gvsgywwmt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ghwktqaln.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gwwfblkjz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gjruennuz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrpxqny.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/goehwhtjp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gssqrbaqt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gwshqvvem.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggvkhhnop.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ggrdoafdn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gngazyuzf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gubxpcemb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gxprdrqmg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/ghazzvlfs.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gkvpxuwjy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gjqfcuxqg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gfycbwavw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkppqumjc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gmirgvfjn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gpmokyjay.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gohinhsxo.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gcopuzttk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gfloetxdk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gwdajywlr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gohzeuwsq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gqjoxhyay.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gernctlnh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/giucmypaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gexthheeb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gapuactwu.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gxmluwmyo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gjtrsddna.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ghardexhy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/grepwfuxk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gaogbpqfd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gtstygetc.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gktqjtico.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqxlcflqu.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gxovmdaeo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gplvvxdas.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gjochmvld.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gvqerwuxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gmwprhrdq.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gzxzdbufy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gjbgkhslr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gmsfnmzhc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gmrtcbxdp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gqpgwkepp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gcsoaxtlq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gtfynjieh.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gtxjkocdm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gaifnzspu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gpwveibpv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gonqszuhn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gpolacjnz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gfacvukup.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gqjboiszi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/geuwchtun.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gpwlxcwvz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjsezigy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gjuobylmc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvqbikbps.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gnivrmabw.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gqrpclztw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gbpjwbnqn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gajdkigzr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/grfrunhqt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gsuvspppt.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gzlytcccl.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/govabnjui.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gdufrkxdt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gnbvoxhjx.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gxptjdeje.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/guoboikqr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gowijliye.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gahtexowd.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/ghdvbbaho.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gjwdugaiy.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gcftfhknv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gebpjrkwz.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gmhfnzimx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gstoyadye.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gxrlujfwl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gdszggfux.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gheznivur.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gbpltxrkh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gszjwsawp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gyukpcacj.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ggwcrrldn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gkuucetxl.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gohhsljbj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gbkyhopch.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gayuezigx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/guhmnseak.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/ggftblhry.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gryegryxr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gydavesfd.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/glbjhjvpq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gxxrbxkem.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gjddkqypd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gmvsuwavj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gvoaivjts.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gztoioysg.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gknukhglt.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gtrlowexf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goinagqyu.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/geyqkuzee.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/grogawjeb.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/ggndrbhvu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gyvwulfdv.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gswugtayu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gkmeutfxa.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/guesqpenb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gjpfqbcih.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gobggybfx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gpskzzmgi.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gyyrzlvfc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gynxypubx.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/guruvxluc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gewimrrtu.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/ggmqyzetv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyjzehixw.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gokncyznt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/guoxtxetd.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gkafhxwmx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdsrygdvi.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gnibkayhu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gkznbkyyj.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gnzhhchjw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmbatcrhb.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gmvahcsdc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gmetykhda.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/giqueaonh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gxljclxnx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjmaxhoor.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gvvvyupvl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gdzkzkolm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdjcgihup.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gaazoveaw.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gvoixmkth.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gcgdfjwwq.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gkuyoncwf.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/ggyabhtzp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gcbmzcfqz.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gnhqbxtxi.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gzecjjoxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/grligqwym.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gdybnhlii.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbncqhsji.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gnpednbef.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gatbzvkmw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/glznsvxpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/giehveoqt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gtcirajjq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/glsxcmptb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gzmaeqbnz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gpeufsmxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gspiaibtb.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gzgillqic.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gefscltow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gblzqhzws.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gvwtpvhnh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gikwjhtsu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gpaaaqhvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gcdlgevdj.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvcgbclmg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gccxrhvdz.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gnfryyxxt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gtnsgdwty.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/grofyyacl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gzzfsoygb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gvcfktbsl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ghegyqhrj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gziwajdpj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gjcroxnav.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gtbjidycw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gjflfattm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gbexpwhvy.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gwhoojczp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghrfelbyj.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gxtvrlhfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gjuxymtly.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gyapksmuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gqkbsloaj.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gmztxffgz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gepjzdxeh.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gftkjsgzm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gdubsxgho.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gjesrrwwu.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/grfyefcym.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gaztbomny.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gquvvklle.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gvlvzhzmz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gvqwsztpb.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gyiwjlpch.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gybedslzy.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gzfpjojdm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gervjfeqi.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gltmahydp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfesmcpsc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/ggyjgzuuj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gattirtwh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggatqleug.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/grnqytjtc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggtnshnif.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/giupxhrwh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/ggyqfdtpp.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gtlbrsacf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/guwxbukvv.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gmvvdzljj.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gvruverqn.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gaytgzcdo.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gpcwgfnlv.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gbogkihgb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gxfenxwol.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/guheisbch.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gzihczbyf.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/goopbxsah.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/ghwteercw.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gdrzfjokr.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gxdpyayjk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gmhztulwo.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ghfalsopo.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gratztqew.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/goteuzdcx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/ganuvoijf.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gwvpozjxr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaehbfbqa.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gaephczxq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gsujyzogb.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gzuucycqn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gooinvdrr.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gcytxuvxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gycfxscog.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gkdyjxbbg.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gwcliycpe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gsktabqil.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gornsipmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gpdomnmnp.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/giwakzxzq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/ghcndrtgn.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gacdvvssy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkgjsinyj.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gdxnpiibd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/guhzbjatj.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gkhaxiijc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/geiabyisk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/ggmiljrmy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpmkvjkhw.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/goupgvtze.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/glypqrztt.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghblllkcp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnebiztpb.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gznqfjkgi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gevekabdk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gblmhzfwy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gddfadlve.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gtpdtzhyi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gvbykkdio.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gkvilhfgq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gaveejpkz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwrsjtbae.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkffqdidn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gmfownwwg.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gwwemfjuo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gqjestylj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxyseyyql.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gjostdxsx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gptrfuhpp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gvgnwmmxv.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gnpvikrnr.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gknqjrhvh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gqsdffksd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gwougtjrm.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gvrgidgko.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gzndcffux.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqlihhrhw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gpnlbvvur.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gtboexkux.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/ghbueovzg.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gtopusdfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gnvhowmmd.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gwkautsns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gudfumyte.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/ghpxbzgzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gvadontfi.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gawrlhgrb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gdeshahen.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcvzqbrqi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gncxnxves.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gdnyrqudb.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gqglvukkz.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gvomqovdg.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gkeqzeatt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwezobecg.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghfzvuwxb.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gevrhsygi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gtwnqbpit.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gumptfrnk.sHtML


<!-- 参考信息 -->