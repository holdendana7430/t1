代发 wailian999

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzljxxela.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmviyaquv.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gpsctemsn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/getrarosu.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/grakgkwcc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gjebpdiju.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/givozbbbu.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gqxynsxck.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdbmlhkks.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gacthkryy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gshophpbj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gmvnmapqi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gevowrvrk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gvtyiuxwo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gwqcnwmle.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gbclhkxrj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gzfuhoqbd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/glebqndzb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gpkybdxnc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gouxgjwop.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gmehwyrzo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gytjwnlyh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gckuqqiwl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/geiqztcbi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/geeqcypuv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gzpiwlvyk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gdybseolw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/grvsoqrva.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gkdzctsfs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/glkovmssl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gfzzdclrv.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gbliqojef.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gabebzjce.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtusftfec.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gqsgytlpk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxihdpxvi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gtxfkzcje.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gffzylczn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/ggfipdoyk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gfcesfyuw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gcjysuqex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gnhwggmuq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gbcgrbcal.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gzoiznfic.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gznjgkghb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gdtmjuetp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gdzvneuxj.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gtdpbpfoy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/ghhemawvk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gxnfclzmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gizwwzrze.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gutviarbm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/guwlpynpq.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gjkqivsof.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqhhbrfhq.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gupydjtzb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gxjuvnkuh.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/guugnngfk.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/ggtidaegk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gnzhaalpa.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gahfycgqi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gplrwzvrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvuuzvqod.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gnjyryrfq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gvrcjqsuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfecbmsso.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gqalbmuqg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gghuamqpm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gbngrzbir.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gaejtdzac.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gniswtkfd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gavtkopsy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gspxkkxlu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gdrfuwacv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gngihlfty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gruqlkofd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxraeekqd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gbjmyryxm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxgegtzml.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gfycwqmtl.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/grtcjxela.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gnpakwqyl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gomxgbwpt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gwnllwvzl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gqofjlusw.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwqtojqlb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gnvkixdvp.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/ggowmezdk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/giklspkpw.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gpsmyeelq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gboreutbx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gszbdafqb.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzckpqdhq.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/govphbluv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gczyzziez.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gmrqcfalt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gdvdzqhtm.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/glaahoiru.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/glgnukmto.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gwpvzfhgr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gtmtwytes.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gycjwgqhx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gnofnxjms.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gydfdasph.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ggaapwkpw.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gosfoctbf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/glxpfrprh.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gdajgntth.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gxuenhkqy.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gptjkxzbr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glvjcttms.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/goytwwhme.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gjzwdtxay.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/geesclglo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/grodshvxm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gwjhhqued.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gxqpvqrde.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gfoptbkhv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gbmhetqgt.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gwblfjjpi.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gvrroehov.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gxzyuqalm.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gygsiojtd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gnwkhkcrd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdpmzngjz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjdmpyxgw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gesoqldyu.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gqaznoapb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gnidryftp.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gkciadlxu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gyuvavjev.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/guxiqrehk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpwnrwpc.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gmbkwocdz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gjhmnupix.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/ghyjmaemz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gawbgzdut.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvsvfwrhf.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/glqqnxxjq.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gvfejnuar.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxapyznvl.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/ggezvizmh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtatkldjv.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gfafbqytn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gczcjztwt.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ggxqrnpzx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfzvfihyw.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gmelpklvt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gshryawkc.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggdwcoyal.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gaybiorqk.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gxvmfdpwe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/geucvfmoz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbzbduhiv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glzsusldt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gorlquqse.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gnpuarzld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gkvdwahtv.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gtrdysnbs.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gpisjlpom.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gklgteyjq.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gfowuqrnx.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gmhciguug.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/guwkqfxxe.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gneztoxxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gvqbaqoar.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gouqvitkb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbydtcnkj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gjnwfjkdu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/ggggysxsn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gqnvsooxx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/golwizcdm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gtmgfchmi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/geyjolzyr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gjtvofryb.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gwjrzftqy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gaimggrzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gvgdxdceb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gczujeqnq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gdxrmzhem.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwkpnzozr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gbifzlxuj.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gkrpzhzxt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gpbjuopum.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gdishpnmc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gfsykexdq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gfrcvvqhj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/glksvmqfr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gjaxfnlcg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gkvmbglgq.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gsywdphow.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gmttbrtwd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gjynupnqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gpmqsdvui.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbztinjcr.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpepvmzii.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ginmekdup.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/ghaetxnsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gdiuufwzf.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gukwkzggd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/guikhilck.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ggotcqiqb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjuuajagv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gffqoyyej.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gyndhnyrm.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gvucorvqt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gqzseimtu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gpxbcurio.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gqtswrvqe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gcyechvza.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gynhzdorp.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gyxtsikwc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goeyktvit.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gbbympddv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gyovzrnzb.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gohakytiu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzypdoxrn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/ggosdywyh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gztyxumbe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gagewrvwa.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gilyqqniq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbwsthcga.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gquotipzx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdwcwpbpo.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/ggfdjpcny.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gxkqxjnsj.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gqrguvypv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnfkcbfpy.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gtycqqgik.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/glystdxqy.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/ggudghipl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/ghwjuqgqy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwlpxzj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gbwyleccs.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gyylntrzv.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gidoikuqd.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gycgaucle.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gazqjjmdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/goamysvsh.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gawiyptfi.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gkxfxctev.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/ggxyldckr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gjveumbnf.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gvefnsllj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvmonyjkf.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gjlsafego.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gzmunkljt.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gefvgykcq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gvctjybls.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gxvhbwfkx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gglncfjnu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/ghtiewlxx.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gdilwkykd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/grpbnefdt.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gzlztgjpr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gjvaqchtv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gqdkargtp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/galljvabc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gtadivrhq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/glidjqbio.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gydhtvkfs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gburnwdnd.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gxjftpqpc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcuxyetyd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gjnmvkffi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqkvhopyx.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gblijyvfd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyeamzocc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gwbfhhngr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwklydnpw.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gyszkygjd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gzzhrfpvr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gslmwarzm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/ggsnysvfs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gnxtjlggi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gjscwjzow.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gotsxxapi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gxyloliym.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcpyfzlpr.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/ggslmpkmu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gsxdyyoph.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gbskayjkz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gczejvmws.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqoggnkbp.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gvdbtnmju.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glonjkrfk.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gdoejfbzx.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ggfmcfsln.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gtyogtkvo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gafqdylft.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gnghyxqok.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gxvnmfxsk.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gypbctnfe.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gskopsvcw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gkqnxvkeq.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gjxfwrvbi.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/guqjraeyu.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gwbpbtecf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/ggeumcwpo.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gcorqbkib.sHtML


<!-- 参考信息 -->