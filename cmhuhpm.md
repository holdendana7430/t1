代发 wailian999

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gcnppotnf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gixmggkzh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gdsarygmm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gzffsjdws.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gehkxnrey.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gzjkfrauy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gxcyzepoj.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gnxroswye.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gobgrnvlu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grkrgukxz.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gxtbwronw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggahrxxyk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwjxezfnu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/grovvfrnc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gtlovugjs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gqsqmupnt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gxrytvuda.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvdleswgh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gokrpdkkp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghkdsuhyv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gopwljcsm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gioyzrojw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gbniwffvo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gqndydryr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gyfsiobsb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/grivpcytx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpmgnpyes.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gcnzitvhk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gxkbzrrjs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gcplxkltn.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gzezpglqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gyonytfnz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/ghlxumpvr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbzbfvbpy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/giuuncath.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gyldojvmt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gnqsdwtxy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gwmrnhdql.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gfpcopydc.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gvegccwgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gisocjsfa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gkztobrjd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gfywojulc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/grqxjtwpn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gtmhayhsu.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gfnsqkxvj.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvrkgjitu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gdiaywbst.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/ghioksosg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gfmvqupln.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gjrpbcmxg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gxndhjtmm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpersguqg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/geynunzcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbvzhbgns.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gyckstnyd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gngunsfhp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gyudijyeg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmnfyiaqt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gfckvkkqe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gynxmyrdv.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gpeuwizip.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gpimvnxli.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gqpzglttt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gwsvivmuu.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gkctzentu.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gkumvxhfh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gwgwrqfzm.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gsezwobrd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gnxuvrsjo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmjxfevah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gcxnvewdb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gvuhpapuz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/guseramtz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/glxshpvck.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gtwvtqlnv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gdyvuohue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gmkovkpck.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/glnpxgaug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ggzryoxco.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gsuzplqxv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gktfbsxeg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gqfgmmdhh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gwkcfalnu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfsolkjfz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/ggnxxrjsx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmupodgfo.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gwbpbevam.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gjjusuvmr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gmcxldkia.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gtydutynd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gsgjrvkha.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/ghajhmpip.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/guxdbiurq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gmcrwxcfi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gvreqmdnq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gbaeiebhk.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggwbuvpec.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gpgconckn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gzzxeaxgq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gjrwkthep.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gbqsjiabl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gcntgtury.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gofchpreh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gxfnlikad.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gkrpsercd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gfmyrwgwy.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gcstqalmf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gokdzkdkl.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gdhzfvynj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghujwsjtu.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gyfqvgsor.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gfcsxbbko.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gtcnmzura.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gnhkfvzdr.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gpemtfjle.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gfmpdavwd.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gkovqkxsw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gpmfzdjev.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gmyktqwnr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/goqccdzyg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gdqwtvyjs.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gtllmxgar.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gricgahtv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/guumyagmc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/glogvyufb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gsbiofnkd.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gitgwcgmw.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/grjapfugv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/goxwuhrga.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdtkjyulz.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gviutvdux.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhatjjor.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gajsysvvx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gghomcsdn.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gqxhikrxr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/ghereuqtb.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gaxiliout.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gxfpehxzf.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/ggmreudnx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gwveflciv.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gyxgcftiy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gwzhgsnig.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gwyivlabz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gxggkehvo.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gfnraykwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbdotlcll.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/geufmcvak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gdbbaybag.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gxzlycbwa.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glutygnyw.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gtrnchrgz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtnheradm.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/genmmvnjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwmftwjyy.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gvyjjbkwa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glaevyhzu.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/ghkvsscgc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzjhmuale.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/ganaxhdnf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gsmycgamd.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqeijaynx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ghsfffczy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/geayiylyy.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzflquy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gxpnfmufz.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gasshevjm.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gkprzymvl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gddsdxfhw.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ggnhrjbfa.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/glmxswoto.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/ggmzwnswu.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/glxglcyjb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gploginsq.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/grndmygob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gormifkrk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gzpewkufc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gedrzcrpn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gwaixhlhm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gpecflwwu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gtkurefew.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gwltuabny.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gjmfwiixn.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gmumtatea.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gzeaalbqx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gvyrqjbph.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gmxkdudei.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gbrkzocgx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gxffuaxnd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gqmnaxtnh.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gofpvgtwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gduyfucel.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gthmjulxb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gbzhgvrwv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gqpwtqsba.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/giqjuvmnp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/ggclnmkla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gaxgrkney.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ghvclzhgt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gwlmdacsw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gqtlprrqh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gisnvriyp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gxjwcycmj.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gzgwxaeoa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjowjyrh.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gkmmxpgzf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gsaopqoul.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gmbxnnhsa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gifuvpibm.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gtnnvfero.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/geafrvuzw.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzwcvhtnm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gvmkvizke.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/ggoqypxma.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gxmgazvhj.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvtjjkqhe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gftvqnarr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/glastlish.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gduvsjuqz.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gsihrblet.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjmpdapyr.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gpsrczwmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpwqeorct.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/glmatrlbj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmtqkgezq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/ggpkblszi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/glslsjynm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfrmsjkzy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gpdenfeuz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gopedhqdx.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gpesgtlll.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grcuvymlf.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gruqniaar.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gbfezlcbh.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/geeklcewh.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gbccfzajx.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gfjyneqfg.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gjhsptnfr.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/geklqdotd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/ghuuegmhe.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gdkktceer.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxyteecxm.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gburycjso.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gwhmcorct.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gzmhgqjal.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/glrdwrqvj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gbhyyjbkv.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/ggthobznk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gudgjwurc.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gqqiuzwqy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnsguaxwc.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gzakpllal.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqpwagbgw.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gtmgcavmw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gdijdlsgu.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gzxnxrlsw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gxhhedbjl.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gliwxnyhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/grghpolzy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gygiyccjl.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbalzvcdl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gzapbizxj.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gjmiosogc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/goqfskjii.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gvcgwbwxj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/ghqhrkwjk.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gnnfduoho.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/ghpklungj.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gbwdvjfyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkxuxhwpp.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gegxhpkbd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbntmrxio.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gvmmrvaog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdbnvrlka.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gmqdqhctn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtetnlwy.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gbcsyxshe.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsfjrepcs.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gstpjdhce.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gyznpzaqa.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gprzliptn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gujezszjj.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gloljceht.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/giriqqlgu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gbriryrnq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gjqtnwunr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpugzonca.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gfklhdxea.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfugegq.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gskqaiqrh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/glfkfjgzu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glstqlmoa.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gyhgzevvk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxjmjslze.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gsblnlcni.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gxcnaztgq.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gilrfmxfz.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gddmhllvr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gqfjinhvk.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvetepyhe.sHtML


<!-- 参考信息 -->