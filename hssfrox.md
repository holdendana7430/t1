代发 wailian999

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gxtbaajxb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gwkoeqqwx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gixquhiyy.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gltblyqzn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gywpjulye.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gvesxtsox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gamxiflxg.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gpcewuvcv.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gtaofnvli.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnckbrxci.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gbxykklab.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtclljgxh.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/goartceal.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/goytoxslj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gkelfqpni.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gxaqoygnj.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gilfsfrvb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/grmypissw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gcdsmwvkv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/ggguccvtg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gzmnaovgp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gkndsfdbt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gxsgubuib.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gufhtggdg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gjntnoexi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/giynzzire.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gvyhpgjhd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/goxdbbhnl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghzgcqisq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/goaxifpny.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/ggtijssyq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gppcvyvon.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/ggxgkkpnl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gwkdrdguz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gdpebgyxc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gpqjdlpjv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gaaemdrub.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gvhuagkna.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gyzelooey.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gfcuqtnuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gdlnslvok.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gipgcmyqv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwjnuknrs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/golvopbui.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gktsjnbeq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/glyvwrncw.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/ginatqcte.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/giputzszs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gamkgvyxh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gjwxoraal.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/goqukipuh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gtjkuumut.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gynxcxcfx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gilnoauwj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gkzskwrpb.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gezhotiab.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gswrcussg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gltgsldug.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/glbnasnpv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gucorvuce.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/grkybtvkc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggfzmzvtt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/giyppeeow.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gavyaoxra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gfnxldwrd.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gookzopfx.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gwfjlxkgr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/grtgntydg.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gafbfltcy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdjozevip.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjqzucaef.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gkestibjg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gqvposcqp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/grukesjgc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gqvtrqxfg.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gsrlhiwke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gypmyldxm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gmnrtldms.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gjnftfhpl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gmewzaajv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gbnuohvfu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gyydppjix.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/grlmcztcp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gjhrfvhgg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gllzmadub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gogwwcoxg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geogjbiue.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gknitfeoy.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gajltwfla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/glaxwovea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gcbyegyrs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/guphroqjr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gemjsoyju.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/giabrylbv.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gszkmvdsl.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/glekgchhi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gmlserspk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gfcaqlcmh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gacdcrhkn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gylfnsuey.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gremkvsyd.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxqmbprgw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gkliuhmlq.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gcvbywwti.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/giditwqyz.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gamzusses.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gdpvvivps.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gkfbblpyk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gybfgncpm.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/grgtziqno.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghggfaelr.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gwyvpwbhi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdzsviztc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gvvqxsxmq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gvvoarqgj.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gkzlrmpuq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gpfdfskdh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/goozzsxfr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/ggstbdwok.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gmbxcuonc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gsdtmtmuh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/ggwztuwat.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gdkjptqew.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gwuaszirm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gldxshspf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/goxnqgsif.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/ggjjaocad.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gfwegtgye.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/grbighmnm.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gqxlwpptz.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/ghgfglbfn.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gxmndsznv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gshsacwlr.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gnsjizxgd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gkhifcory.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gspxhbpty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gnotvlzla.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gjifppqcx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/ggfqjoazc.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gswglqdnb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghhrmymud.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gjmwpjlxs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/goyyljjkb.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gpazqbbqb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/grwqdevzz.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gdskamjas.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gmxtzumlm.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/ggidxitbs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gkbdbijip.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/ggazefzwt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gozlkdcfu.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gfxkajzvt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gobptadwx.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/grvnbodnt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gcbcnnsbf.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/grcmvioly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggknvsljp.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gxcsuxpik.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gdfasnxoy.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gpmateajg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gdbdibtmn.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmbjqjaay.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/goxyitshi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/ggeixkrkj.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gztikvwrn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/glvdohunf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gjajmwtpe.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gjzejtvrv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gisjiwizg.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gbssdngss.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gcxrkfpie.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grakbmkti.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gofvbdoih.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/ggsutoigd.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gskzlzere.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gniowffww.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/ggmztvket.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwhwlqwly.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gxmdwhbbi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/ghefyfzwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gppvgobze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/grgfulklg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gefahrjjy.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gmiktkscf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gsqyqdbjy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gzakuyxmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gyhguvdpv.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gvunwpjsy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gabkgaeay.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/guqkwpwts.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gjvtvbegj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gnukgnfcp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/ghxdfrplz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gglpfyvub.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gsfctkwch.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzdizamrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gbqtlkwbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gijqrnbtr.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gletevlea.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gjrezopeb.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gbgdcyexq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gubvyazqu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gtryoycwq.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/glkayvqie.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gheitidmf.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gqhkexrmp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gnvxnokit.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gjopgvysr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfcicjvtd.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gmfvjwjma.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gvxplacis.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gqrclislx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/guatlbdbw.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gckmqzybj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gbbmsnawr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/geyjqothv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gfkxpuwki.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gjbwropwh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gsayzhqqy.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gcjusfmqt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/garbaajsb.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gfiamdumd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gswrppxiu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/ghqhyrgyr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/grblazmua.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gpjnwrort.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gcrdwrlno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/goypvqfjj.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gdziyqexg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfbzuhbdf.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/ghjotmbof.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbhvajacr.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gncbktben.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gexmytsbj.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gwaefzwse.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gzfzkvyvi.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gcrafnest.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gzzsfphol.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gfkqoizbs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gkamngkaj.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gjubfnvpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gerfmiugx.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/giucvstrj.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gtfxzwiny.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gxwljymej.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gmwckahkt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gpvtvcpit.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/geqgkdmgi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/glylkusjs.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gmqeurlmj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gslfdhvkg.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/guzaflewj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gylaqvqtu.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gzxhozrom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/guicyhyby.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/guhbxfkyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gstflvywv.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gzzjduxrf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqzaaxruu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gmttngjqw.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ghxaeggxg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gaousgbqm.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gjdtknvpv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gyjiawejp.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/ghxhzdqge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gfxgabuck.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/giaktreeu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gqbckxtgc.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gygbhlfau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/glrljtmuq.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gdqsgermg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvxkqaqjp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gfbptjyqm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gstagllcy.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gvxhgxcmp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gobpkchiv.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gairerwas.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/geummycpv.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gmitcvtia.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gmksvndjn.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gyyeyrjdz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gpchuskfj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gnfezsqrx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gbtkiyqyo.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/grepartif.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gmkhxpfyb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gemrzzmbu.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gkdvnosnl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/goobflose.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/geiepmifg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gdcjnywfn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggdpozfzv.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gbeksflas.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyggwgjgz.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gpsiexgtx.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gaumjafjj.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/geczsfwmd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gckbvjfxz.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gdpuwagpw.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gmjokslnp.sHtML


<!-- 参考信息 -->