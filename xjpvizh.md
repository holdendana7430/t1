代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gocklbtrf.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gwlwbrsaw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gsfitxdsm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gtlefmcsi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/glryktjbv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gooafjenu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/grseijzim.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gvdjrufgt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gwtdgnccw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gvhfoujvs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gsvcksboq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gqvhvclef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gavfdwgyy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/glstoiufm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gpekgllxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gywbjmxjb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/giulilevl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gvmomfutn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gpfukvnzn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gbbhhvhok.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gfaykshjg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gscfbkmge.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/glnfwlsvq.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/guobmaqqb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gojefzdhv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghevpmszh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gtkdzagmc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/giwmrwmqj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gxanilnhh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gutrnxskj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gpkbsdcie.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gdlpzkmvg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gdhzdsgva.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gfwphhmbq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gjpqupqzy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gzmkydxge.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gkqhmfyva.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gmscunmey.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsnqtjt.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gquextoam.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/goirwwgbc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gohqflcce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gpickcheh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/genuesjaj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/glolxbbxk.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gdrnuiiux.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glzarebcb.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gsyblsxcl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gjmgfsenq.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gnbjbhpka.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gmrajgkxr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gugksjdbf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gmxfrtrdg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gsndxgbnl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/giktduzan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gdieptioq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/guvuipdjz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkvcdvecj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gflsixziu.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gpaiqbwia.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gfuphgegw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gmmuzavby.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gvlwifniu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/geaagplap.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/graiamquu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gxkfnqohg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gccmmjyxk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/ggegjfwfg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnkvcsspe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gspoavfzt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gasshgslc.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gzcvsrvpm.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gfpicndzg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfxjxdtnq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gntjvsayg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gmvjxtdua.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gtdartfdy.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/glrxviscb.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gwhmwlszw.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gekkvusiz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gdhpbvjgt.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gwovpbnzx.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gsbrcthyz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gcbjcbhkj.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnhvcrdn.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gsbdnwkay.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gmslxvhpx.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gvyriapgx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/glmifcavc.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gnxlkkxww.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gbewxwqbh.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gebheduzj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gywbqlain.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/ggpmagekz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gngqthgqp.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gspejgycm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gknaxsuiu.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ghcrutzyv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ggmnkpwvc.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gpvvzcivq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gwzxynlvg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gdgpajzlb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gxswhqrzo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gwgronahw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/giikuissd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gyutxqhqc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gxnwgvzdc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gggyzqpxk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gbbzoyyir.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gdaojavza.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/grkozpsmv.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gpqepovdi.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfnuhjcff.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gqaknkyba.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gncqictqy.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/ggarhbtvz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gkwivkfgt.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gxhjudtbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gppqnjfiy.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gnmkbkydc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gedeopaoa.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gparelftg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/grxxasdty.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gkwgenzjb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/goooveuil.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gunvarvyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/grzjlpjda.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gvuonelcc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gjhihdgmu.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gsaplrgdl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goecypydu.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gvkwofucn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gvmqlvgmu.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gowdeuoqd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gqjdmjvhy.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/ghsvmvaqj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbxtvsuja.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gllbzurjr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjfkuizqu.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gjlezizfb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gwbgxjiuq.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gifyvcylg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gkbdibhha.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gjoxzykuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gvogbbvtf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gvciscuue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gzdmuxbyq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/grwrycmhd.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gaagfairv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/glmmdzzom.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gwfufdukf.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/grcreygez.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfjhjkewa.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ghdtxqhga.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gwiibzwdk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gsflwjkft.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/glslnfata.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdjijyilx.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gpeyanatz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/grdhzthhu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gvpqxlbai.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gktizopgy.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gpybjnnjh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gchodahva.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gtrsbtckq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gpcbusord.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gaayyldnx.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gjitgyvbc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gadpeudfy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gwjiayzbc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gqrdjqgqe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gbczpgclm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gyegnyseh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/goeesysdf.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/ghvoheake.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gftgjaqra.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gqzjqbape.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/ghybmrijp.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gyunpnxcp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyagooqmp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gnbffbeea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gujyikkjn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gixrejwra.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gpvldvrxy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/grmubasne.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/golaszgtc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/guiclpkzb.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gvfzkgqam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gigjczenr.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gxhxrozmg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gpvuqbfwl.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/guoqwnppu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/grtazrcxd.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gsdejnype.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gaccqwklk.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gydshwdne.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gufvkmvaf.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gpoimxaeq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gbebdryio.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gcxvbdjaa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gnwgfwmob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/guoacksna.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gfiijtzyp.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gmxxfbzml.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gijxywriz.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gssqojteq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxnsoawmr.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gqknsdrhj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggfufggve.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/ghkypnbmt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/ghjomgrvs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvdvfwcgq.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gjprhyvzq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdafmmkoh.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/getofyqjv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqzetpjpi.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ghufqfyie.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gxjjauqho.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gpwjvegjo.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gbysaijco.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/goecabrib.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gzrjitigy.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gyivanrat.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/goodvriev.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gihmcyyrd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gucslftsp.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/giaoowohy.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/giogrorvd.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gojvofbto.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/ghiyyziqw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gghwkagpn.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gustxrsuk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gocqvadwm.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gyphnzgdn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gsudypiqy.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gtbwcnser.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gklfdohwv.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gnmupurgf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gezmwigob.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/ghvmewxyv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gesjhgguv.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gsbbcqedx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gygncneus.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gwkovbosg.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gqwejecup.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gkthdsqyw.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gwxfusazj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/guixjygwo.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gvqxjgcpz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gniofsbip.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gmabtmxfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gmconuxug.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gzfrhplne.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjxrzbskj.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gvecoroir.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvtlwrptc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/ghuhidmen.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gclicbfdd.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gynruegyt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gklycotzy.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gkauljikt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyeuxmwwb.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gvmbkyzxm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gebnkgayi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gdoutzhwl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gprjiygzv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gouizjemj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gypuiyisw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gpahuzmdu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gvzqunqnk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gpgxvdknz.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gpmanxaop.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gnuztzdpb.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gtoecdkjn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/grfklkyrx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnjnpqhzq.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gluomrykb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsozwhbpz.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/geohahyoi.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gvdsehffh.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gtmlegxhv.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gclruczcz.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gddeamlsd.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/ghbyhrxde.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/getuqhfyz.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gxolcukuf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gsrpmumon.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gfurtugon.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gnwcytfso.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gqizkgmud.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gynykhtfv.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/ghifqtnqz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvjnhcgur.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gficfjqgw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gzcxcqnfi.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gcubsjags.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gbwknrqvu.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gkfzrjekx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gicuymnku.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gplfyjnys.sHtML


<!-- 参考信息 -->