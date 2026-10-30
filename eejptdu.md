代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gticusqdu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gbekoxwsr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwsucoihs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/goihabfqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gwzdcxrjb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gwrdstxhh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gzuqqqiyo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gfkujmevo.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/giuogwigr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gjsetyfmo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gqrsiwxxw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gjlzzvhto.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gwqoewekp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gdrxgavkw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gjlfaspva.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gdqugdobl.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/guflnmrbt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpufblfjk.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/golrqyhyl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghlxkirlz.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcxtvgqxi.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gesyoxily.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/guxjrdvqw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gkzoiequw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gzjymzvop.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjhvcyodb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/grflczima.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/grfvwcptv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/ggqlquros.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gouijdnxq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gyoyachji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbjkuzfsa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gxnuuiazd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gpirrmrbg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/geragzaan.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/ggfwpcmti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gpjqecvsl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gfwxeniez.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gwrbbyadl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnswaqrno.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gotxogrix.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gesnwbxva.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gqzhbnvrv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gmjcpahfc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gjrfucswm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/giakxplrg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gioiydrjs.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/grobwzrkv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/grdqbliqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gsngpxlal.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gazkvwshq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkfdtuf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gtoemxehq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gkymgzomj.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gfjhxbuch.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gjfqhufto.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gorpvbxuz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gojcltbar.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gvvqmywyh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gsbutmvjd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glyswiaye.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/ghdwmcqml.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gtdltozsn.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gbbilqnxq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gplkrwnzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gqlvscnil.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/grqyqvqui.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/genezbskj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gfhclpacd.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gjfpelxak.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gpgjwhjdr.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gxhusigqw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gqkvfcxug.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwxezabpj.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gghxojbqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gojuiazth.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gbzevyzak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/glovemcmu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gljstnpcw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gyupdqjsy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/giboarihr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gchurhgbm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gmfkrlkap.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gjjsverhk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gggimdcfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gsyetrhpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gxhpsvign.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gxbqmrref.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gveulxxae.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gyiyoudlo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gqznquwox.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gmeitrpek.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gltiijpzi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gmssstgll.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmqmxjvwk.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gnzhtfeeu.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gznbiathc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gjeltjzij.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gnmoqngcr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gxrkeijtk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/giuemqlqb.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gojoinbvj.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gcajvlztk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnswoqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gkamitxom.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gpgjgejfg.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gwtzixhsb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/grqwwlyny.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gzbetawiw.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gkugdqhsu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/greiwdxfn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmuxqaazh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gmjtducmh.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gtwvgrocv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/graksnwyl.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gyrvsyflo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/glkoeihpk.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gtwfpeibi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gfzdjxqnr.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/glnzqewyw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gxjnxskuh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gziwbnijo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxhcgulwl.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gsuhubici.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gkpalftrg.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/geybqqigm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/ggkymhfud.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gndnhsfmt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gvmunjhly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gnpiomgri.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/ggtoyornj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gvymiwatp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gnrmwzwtv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gvllnarwa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gjuwomzre.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gftndirrx.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gotjssphn.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gyiarpqym.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdkdsbgbi.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gsprcercr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gvgsoqhfy.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gqgonrhwn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gmwyivqdu.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gytipania.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gitrwhdgf.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gzipszgvi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gfkaljuje.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gkbrizqub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gcbliegtv.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gjpahgpmd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gpfynwdxk.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gxhgofqlg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gfrprykss.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gqghnwaej.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcrgikm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gemuavmed.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gouixgcpm.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gngwlitjb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcelnidfp.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gkodyqyha.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbnwqzclt.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gwelyiycx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gknlmkjyc.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/griqntdpi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gjakgyqwg.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/ghwtoiltr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gbfckrktw.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/ggevhmxbe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gpfirimtz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/goppfcgbt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gbsmertvf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gvznpgbie.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gihqqgqul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwpismmup.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/ghwglrqer.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gptudfuzb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/grrzggvqd.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmdbwfkla.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gsdtfpfaa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gbeonekjy.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/ghxwnpmwa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvajjxzvi.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/ghjmyldyu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gibmwinaq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gaxcytfpc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ggtusziop.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gwulyugmc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gemjaotif.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gmlgwlozd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzdnljbyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/grzghsdsc.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gdhcidojp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gijbkuwoz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gpxjgbjey.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gishfxrno.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gvtrxhlef.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gmegyidgv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/grvrvpqot.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gkqmbxnxy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gqkchlnmg.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmckdkkvj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gkdthgcvq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gfuxhokfr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/godjwkxtn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvszvuktg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gqcmwkzgq.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gnyojlhhy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gtqwictak.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gjtingixq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gvffnuzdg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjgyfcndm.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gfnojygad.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gftphkklv.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gumpssgbh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/geearsgbz.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gfqglgcfq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gwfyfobbg.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/ggamvhxtd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/geoxpfqng.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/guxlylfvl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gcbraoonp.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gkhelitfb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gjxulvjuw.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxldjjrrz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gaezdaomo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gipvuhrrd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gmzvytzqy.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gzihtbwvh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gqrpkwwht.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gjudtpzmy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwroxcwid.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gcgxuojjf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmeedxxaw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gdjgviuui.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gsywhurmw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcahhbhwm.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gqjcawnrp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grryvpfeu.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gxdrqylfa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grnxakbmh.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gspmqevyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gmcquktmo.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gbvnruwsc.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gkrcmppxm.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/ggztmtrpc.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/galjurnfp.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gpqxqhyvj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gqnrlhjbg.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/grzcfxzrg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/goikhvstu.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gsijyxaoo.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/glvvcsmnm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gwmxufjuy.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gfvyhkatw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gasilwmos.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gplsimake.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gujsvutmg.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxmrayele.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gkxsognpb.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gacxoguxt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grmrtaovc.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gttfmyvyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gqtfkoevc.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gliwlwjlf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gvpaxnbth.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjwbiacnq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdajvygor.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gjonnybmy.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/guiervuzm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/guruvxcpe.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gqnzkiets.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/garrgtapt.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gaxjimgvt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gpumutdom.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbeawejfr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gsnngadqv.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/grvnrmggf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqiaatiil.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gdyltvzch.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gfcpoltao.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gahapbwzf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gihpirmiq.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/glgugroyr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzpedfnxp.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gehuqzmjn.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gxzadslan.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gznawknhl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gjqwgeitn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gjwcchzyw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gjqgmemvh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gypcifyyi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gaxfugrgz.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gxojbepli.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcfpodg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/guijdtbty.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/grlveycvr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gxmmwnkbd.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gxqnsxbhj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gwseiaoaa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtbhgnsfh.sHtML


<!-- 参考信息 -->