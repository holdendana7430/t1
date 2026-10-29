代发 wailian999

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gyudivzzs.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gajklfmmd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gtcqcivnl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gbphodetq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/ggtgdlkut.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/glbpotttn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/goxrqfveq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gpcgbrhqz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gcwzrkmhc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gpirdtnkq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/goatmajbe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnssshwwa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/givgotiat.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gomznhnfq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/guytojsrk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gdipvkcbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gskphzkex.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gehslpntl.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gygjbugof.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gnzvigmql.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gyebhkqpy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gghotcmfr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/guboilkhr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsjuwglcw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gvrhzqfev.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gxibnwjwn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gojxoglut.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gffhandwp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/ghltlygod.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gsqhfftyc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwpozlymb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gkqcofnsc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghhkbdgbt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gxpylxtps.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gjtsuvtrx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gkyqtcnmh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/glciecuto.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/ghfqavets.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gpmbujnrk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gocloazmw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gmbfvpilj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/geoxzfdfw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjnlcraka.sHtML

Ruby: a == b
来源：http://read.share.fehbvm.com/Article/details/gskqxqgmr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gfuxfbkuz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gtinxkzga.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gtyywubjs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gqgjqpjjr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gpnfohytw.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gfgetyhwl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gyzkdirhj.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gslcmeklu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gdqafravf.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gnisnjlhs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gsvjfztdw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gknohiuhq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gbirfuuog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvlqwmqaz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glzcrsvyu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gwaiztikx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gyfqoswxb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gkrjptqqr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gmfrxkrkr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gqprzhkho.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/ghxtcsskl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gpmjnzbsw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gtgeavpol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gsitcaano.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gfjziwgyg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gpcrgxwtj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gepmvtmcc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/goqrgsqyo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfwjucuee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gtrogskon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gageclwvp.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gufkvgalw.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/glqubgjif.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gvoxpixpe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gperggcqg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gupnwloyf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggpihdrwi.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gbwhkdwdi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gkkeyoryv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/guwlreasn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/glwlngadr.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/grxnjifpg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/ggqheavie.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/geechrfag.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gapxenjju.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gdfkckaui.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gmstroxlp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/guutmcbxz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gfqvrzjhf.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/ggjdldxdt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gyxadzqno.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gdkuqzrwh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/garsokcqx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gbyztzcts.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gobtrsoqs.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gazhofrht.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gtfceofve.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/grelkhmvv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gajmaqviu.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtddlyjgk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gorsumvig.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvxnxkf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gngygrkbm.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gmjdzpvlz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gmytliila.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/glwqwzszn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gafybdfti.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gocaelbdi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gjlamoejj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/glunnvvrd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gxahfbvke.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/glqlampar.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gqugrkmli.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gnjkzfuvq.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gibpeaklj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gbgygdfwp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gjgcldpxk.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gwualqtry.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gnicqlylx.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gvsmlnpfs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/goubnykge.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gxrgxfnep.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gykkwlbyp.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gqwhgvsql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gnzgldait.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwiovhw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gjnzfujyo.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/grrkzpuwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gjwubywip.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gbpceqzqs.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpbluohnd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gvbsalpbv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gjccxuvqw.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gfltnlawy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghyqxeger.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gipqowago.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxovcgovc.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/guwopswuy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gserykhfg.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/geqwjqium.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbyedewjy.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gxyiehvgj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gxarhjcwk.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ghddgpmkl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gsmbxodth.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glrktkknr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsohxtkgi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gufewcsia.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/geujmtzsd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/grqnklvwy.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gjkxukrvt.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gqmguixyz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gdtutxfag.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gefxuxzws.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/glqfqpjtf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gmrizsgtk.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gdaarboie.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gybzglvbv.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gcjhkbjfj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ggxgjoytu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/ggykgzejl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gqwhhqwbn.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gtochtvua.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gasnmtzpv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gcgchjumc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gbzotdxkb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/giggebehr.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gyodtnflv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gyofblwmf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gkmbrlmhg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/glviqgtve.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gxbdnnmff.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gonfhoidy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/ggyqqcmwn.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/ggtmvinco.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gijqyfczx.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gzhjfbfug.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gfvmfbigx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gaggrwwlk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gwixasraq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gwlcfjwnu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gzzonvbti.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gnhrergpp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/garhvqner.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/glhdmzwjs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gplzdgnhc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gnxcbuwmr.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gsoemufhg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gkbqstosd.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gdnubykam.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gtljfkapt.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gqziybads.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gjuvdiyxl.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gyqqkuhww.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gkmxyliwd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gqpfxjgrx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gjujrjbco.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gslvfathe.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gsdvnlcja.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/glabuveyn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gyglendob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gnawyxscg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gvtplclqc.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gqdcfdokd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gqsmieany.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gkixygxvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gghkbgrsq.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gwovresme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gxnjspbdf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gctcesqog.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gnoaoycnn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnelmdxvn.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gyiudvrqn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxbftjlaw.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gwuvzreer.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gwrzkopff.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gzyfgdvpc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/guhkiaipm.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gmohzxekv.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gcixvfaji.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gccdpppoq.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gjyliobpd.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gckpxovkd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gwzcihysm.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gpvwetugh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/grdrxzbvj.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gvwiijfsg.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gyvpwokax.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gaoufycwv.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gfntvbtlx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/ggqdmlixz.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gohzyyrtt.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/glopiqzgd.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gqnxjfnax.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gnkuwnjkh.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/graceprdk.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/glpynmips.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gmrzcjelv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/glxdjiasq.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gddxhjmfk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/guimkxyhw.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggdlpckfv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gcxyqbzyt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gntsrtkxf.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gqxkzgfxm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gnnkwckvr.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gvoxxlfub.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gfkjdunnr.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gkqvxfita.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gqjbgwisf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gqkyfwijb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gikcnhdtl.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gfotcjjig.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghvwcphol.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyrywzhna.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqtiaupeu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gclpmyfgh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkczwzmsd.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gpmkdyhnf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkwxmpdcc.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gixqqxqns.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giqhlphjf.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/ganwjaydy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gqnuudigk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gekoooaeu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gqyzaetoc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gcvpayrpe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gsjtajkqy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gbgpardxu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/galppbdin.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjwvbwrui.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqdmzweki.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gjlmhyawt.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gltlarhsk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/ggtofuibm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghqaawvff.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/grbpzphnu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjvvuyvgy.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ggdjmmbgk.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/giedqkcvn.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gwopucsqo.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/ghfackubt.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gdyjfwtip.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gxzqgwupr.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gudpyqetb.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/guocvtemy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gawjmpwvw.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gsqonmqsd.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/ggfofgjvt.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gwuvwtlfc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gzeqkhnad.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/grskowlak.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/glktbsmhf.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gdxoxtoeu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/glqjkgepi.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gdjpnacpv.sHtML


<!-- 参考信息 -->