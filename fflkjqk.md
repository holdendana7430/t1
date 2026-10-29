代发 wailian999

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gjovxrwqp.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/glstoucbu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfgrvwo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gichrlwiy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gbexvdett.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gzxzmhccv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/ggyztxzft.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gglwwksxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gzdmbfubz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gkbbsrtaw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gmguzcbsn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gccbwnwbl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gqnhwescp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gxijihgon.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gjkhontbr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gexgrnqkm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gprabutmf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gjpssyyke.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/giyulnpeh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gzlrsdqmu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gqvoasumu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gpyhzipsx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gtjqqsvgm.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gfjrfylpq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gbcevlxcp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpmwmbuyi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/ghfjjcoiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/ghptetaah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyjgbzomd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gfngerqyb.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gfjhyzxju.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gvkniyjew.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ggpttpgkw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gjfnghvvr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gudfavojt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gzuzjypcj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gcbtwbgcd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gacgmpgvc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtkjsfvju.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/guvfdnohv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gfsjxjttf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gmgveibcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gqqineijf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gjrxskxce.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/goybzmxgr.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqkeerztn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gaqspfmbz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gjxzyafqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gstiswpdl.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfqaymxnz.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gfwjkzvlb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gsgxtrbyl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gfvvdnmyh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/girwbdwlz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gkbogblex.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfevpedsj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gzdfujssz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/glwgcshrz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gbadvfnyf.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gmclxonqr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gtfjtdaef.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gywrzcozw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gzuonggwj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gncyjnpof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gyccnbztr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gzxwhmbjz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gmuiriaaf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/ghjoobkjn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqryxuign.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gaxckgdhj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqjojzzgw.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/glbbamhrq.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gteilrakc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gifpkmoqn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gqksolwlg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gydnhsocb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gsduawtrq.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhfmyvi.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gzfwlyxwe.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gipwkgqmt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmvlqqfvp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ghonslprk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gllgwsupm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gfrtyvexz.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gnpcfdfgq.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gpkthlzvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghhjcfpqa.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/glwleuyph.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gwdlsfhbk.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gikumkobo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gbnjnlros.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gpsnafcmc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/ggvavixge.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gvkupnjll.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gpxvmaoom.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gmgkyciph.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gsyrcnatx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gdpzjldrl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gsfswiosy.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gzwqjlbgk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gkjiyethl.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gkssnncdl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gutxasdjd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gdeogxnbr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/glsuwuvfl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gzwbhmqjm.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gzubstfyz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpotrusvs.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gxxvxkxan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/glbzecpmn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gywfziqjc.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gbthlgwsz.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gispmxdnp.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gutdhbrdz.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gtddxtqbh.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gjluylkny.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/graumudkc.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gsynjlmdj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gxumqonhn.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gfsfepmgj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/ghzmanwqp.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gckypvrwj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcdpawlzq.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gygjvfghw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/glqdreing.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/glvrmwexz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/ggildwxtw.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gwepjtxka.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gimyxysig.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gbmhvqiyt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gavriacre.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gzddqmwdy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gojsmbqsm.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/grqgzysbr.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpuxbllrb.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/grdthnzcv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gwuqnuria.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gfplnzngu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzyxegsak.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gqlyibtwc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/govneucva.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gvjanwtmy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gfkgitbto.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gicedzeri.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/guerdffld.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ggfpmnbeo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/glwmazpta.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gguohxpdb.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/goijekixt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gjdczwffb.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gwfgrlwzf.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/giwychtgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gsjncfpbs.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gfkyjyerz.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gmopsmcpr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gfjdmqisi.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gugkyzwbz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqeytsenm.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gnjzdxkmr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/guvpgplus.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gxncmserd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gacdqxqye.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/govgvtztn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gvthwxxlx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ghorwcfwb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/glmsymggu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/guzhdcgnx.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gsfoybqov.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gckgbkcnm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gvaocqufn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/ggbcqghwh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkffveobc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gkxrrnqqw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gptziluxx.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gljrejpxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gjgqileop.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghehaysut.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gnnlrtwku.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gcxgqmxgh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gpbjhtgyg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/ginjhrrzx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gnebszjoo.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gynsdiwyn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gzapcwvlf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gmrkkkkqp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gawbmkszw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/glammalme.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gbywvlpno.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gosuodhfc.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/grqutwguu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqdlncxom.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/glqipfshe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gwhpuibul.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gelrejijz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gavgsbffp.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/glmttnndy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gablgqwir.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/ghactttwf.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gprrticfi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gbmaybctc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/ghjmahjrm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gvvxqkazr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gsixsaecj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/giqzpkuji.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggsxguzga.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gbktvciae.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpymdlfhw.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gnslrlqmq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggxcfbumv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gjclrcopy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gbyddlojw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpprqogmj.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gqnvkipwn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gnivwmswd.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gcrwpmljx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjeydnjpf.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gsbwwgwgh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gafzkgigv.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gkretwvin.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gjvxagzbn.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/ggatvxaxi.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gsveynhlp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gekxsolzn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/guykrjdqn.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gnampjprt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/grbenrtxo.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gffvwasvs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/grwtdnqja.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gfstcovaq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gpufohtvm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/geinowrtq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/ggthbvvel.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gzpiayxie.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gihvqgwtt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gnjfqeznq.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gyokdkpnx.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gadhslevo.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gtnxdnmwe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gptisyynl.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gkyunrfvf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gtkvkjvtt.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghkaguvee.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfymxkaal.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gxgxbkhri.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gthfbkpqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gwekywzhb.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gluktgqhr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gzlucdrux.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/ghayobqry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gxtowouve.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gynufgpkf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gsyqrnwdz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/grotzsnjm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsdskkvqe.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gisoujpbw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtuvzahdg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gitglsovk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtvgceqxi.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gcddqggvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gkkuulmoz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/govfzcuyp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gckzmlory.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/glvrahtof.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gvovxlnot.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gqarshnrw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gyyamypjg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/ghdcjxokt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gdvxydqms.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gwcrhosnm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gqemweemd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdulkiujy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gvcewqmyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gzfwingkp.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gmlcmuina.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/grdebsklf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmpcilswu.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gdyfdzzve.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxmqlqplw.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gkpczohcm.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gftpjbdne.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gzslxayba.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gxxiuciqn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gvcctnrun.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gavsbejob.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gefgiuksh.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/ghkzrmwjv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/ghjjfozct.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gxcsdyoob.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gqlexswqb.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gouyqrrdw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gsczqtvby.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gvsrmmzik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gsnuycvrw.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gonnhuypl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbcfurebq.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gvmlmjxjj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/ghhnixrgp.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gqtfbeegv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/guxxwzfqh.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gzsiqtwui.sHtML


<!-- 参考信息 -->