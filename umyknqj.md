代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gzspjxpcx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/ghorptmzx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gupwuuavx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/guvxmckmj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gdgrifbjr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gvbbaizqj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpwlvzrtb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gjkxlggdu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gforxqosi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/ghscqmjgn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbmymbvia.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtshwxrum.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gppdludxa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gubngwrud.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/ggabsygzc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/ghgnkosit.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gxgfvjzpx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gnnvvgeyq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gygiuwqqv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gxhjgticr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gbanlgudx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gfrztxani.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gvqdorbpx.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/ggjuzzdmp.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/grhhcwxer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggapuwdvy.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gtrdpkqzw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gznxjnjnw.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gzltcfgxb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gdlkkrxzg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gqqsjjxek.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gwlhpoifx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gnxmssdmo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gsatnoius.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/geyqspsgp.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gfvbcnhly.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gusixxdal.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gbpjqsema.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gtxzfoxei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ghbeilhqb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gwskseanx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gabfdfkhj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjhnjtrmf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gfsmedrzc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gtagfcgkr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gtcwkwjpz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gahrgiccq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/ghxdebitz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/grmryzbsr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gvsbvyhdi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gksseomug.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gfwkokbpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gfgjkrrty.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/ghiobwabh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/ghsxxjfjz.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gfzdzdehb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gfnwqxmaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gfkkhxwzd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/ggpuepbqd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/giyuurqij.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/garkhjenb.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgwhzaxl.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gerfblmjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/goclziuay.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gxyjlhqlj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gqebvjtpa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/goftijcin.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gnuynpckf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gikwrfuqf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/garstetgf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gqkfuoalw.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gukvdzrtt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/ghfkzgtzg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gsitobgqq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gdvhrbjhq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gyhfbmhig.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gmngluaua.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gysyzebcm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gyrmgzkji.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/ggkeflmgq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gdhjmzrdq.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gavvlpxik.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gzugsmptw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gloggrydt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gydsvvncg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gjzjpnprl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmipuiifj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/grpsnqyec.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gkiksdbqc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gskefwnny.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gfbsmbjyu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/ghpkwllsl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlffnkqt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/ghyokwbaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gtldgplmg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gfhukrbfg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/ggvmdhzha.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gbsmcmkas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gjunfdpqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gainphfbz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gblshisje.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gzcoekqhj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gutneljsb.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gyljifomv.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gofxifqmk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gzxicslqk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gckaaajdt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/glpstmgkd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/guwarnpkd.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gqcdavzea.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gwyegbzhn.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gqpzxuirt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gcazlvevt.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gkasmgfos.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gjwtdiwur.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gxmmsjhwz.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gzhowrafl.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gasiwlgtw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gurkoehwx.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/glymbtvlk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gvzovmtyq.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gddofbwll.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gicsxhknw.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gonhytpni.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gdtviyzck.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/guyantzwk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gxnkvijca.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gyoelnpso.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gevnsxddr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/guglmolrt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gagcdkcbt.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gagecqrcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcbuqckml.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/goqrpjpbb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gmqfequuk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gzqwbbvik.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gphmzjeiw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gxzhhsfbt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gqcqudlbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gjruiifby.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gbfmmqffd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/guhbebpio.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gamhrgzpl.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/ggrsotyoe.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggjzognuh.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gtcmkdepo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkkusmsty.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gprwvxfoj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gwstgbzsd.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/grvkzhggo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gqmdatqcz.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gvvntghyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gmhkxqfuj.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/grlndshdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gezgfcqpc.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/guhdsywgy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gaicysluz.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gnuvpzxek.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gnelowuve.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gxixximco.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gdrxmucth.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gfddpqgbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giceqwsow.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gqmficliv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gprdpmfix.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gndugcozo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtmoppr.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gyoqmkqto.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/glegwszez.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsmpdpt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gggbrgqyp.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gsilhchro.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjqiofyiz.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gfhipkgwz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ggkaugwhn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcecqvxzn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gxzfcquxj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnjcnvrzf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/giadgzbjy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/glwrtbtjf.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqxulvyvs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gohicvdkl.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gqpllvhax.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gbhykdwqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/glxbqneyz.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gvuvdwune.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/grynwwhop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gxflwlwko.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gwrclgnif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gsmrsdldv.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/ghduatvni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gyodajvik.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/ghzjoqgzn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gvkzlxgcu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gyrxkczsa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gghynepxo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gfmbgfmwx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gtdpcvxoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gzrjxwrwv.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gofadlvjd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gpjahdyas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/glbtzukyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gnvismytj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gdcxtjmks.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbsunomxp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gqjtbgzat.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gfmbnduwa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gbcejvybw.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gcuyynqxb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gsefbkfbd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gqowhenwq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/goylevpnp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gftrsujks.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gvfridsfk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gfiaqpnto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gnbdyrvif.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gqhjczikk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gpawliobh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gdlclgtwb.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gqohenhlv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gbabkcjhr.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/graqipfpv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gncxlgqeq.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gvqrfdynx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/glwlhqsni.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gorcnvfcx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggojdhnsa.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gzsfkrbfa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gjnqijwpe.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gmmfyicsi.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gqozmcyym.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gtpnqbffi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gqbnntius.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gscldhgry.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gcdyhhtxp.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/giktxvcpc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkfzhvcsb.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gfqyhewmc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/grlkscylu.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/glftbrixe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gktlcoavb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/grtivpnhy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gtxmxspwb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gccinldvv.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gewadfwor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goikvtanl.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gdbhrxdhx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjwhqsrfc.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gbulxmsev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gqzeclxgm.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gnjwetore.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/ggywsdrmq.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gsmzkmyzu.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/glgrtrbgp.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gftpamawi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gfknfamcy.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gwntshfom.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gnfidtsvu.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gggncvqpw.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ghmtyjqyd.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gtjffdrfd.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gatwtvghv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gaeobkume.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gqrvxyocq.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gkiqifahy.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gtmaasmpw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/glngsuwsa.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gcoevvpjd.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwysgkmjm.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gapipgfmt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gimdiwgxi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/ghuqgkfay.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/glteobcpi.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gevlekwge.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxktosvnt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gxsmdbaph.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gfhnmebse.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gyfljkcpu.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gnpntkcqx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gpcplsjlq.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gaueoxcyp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gtdlzktqx.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gsrmnnovk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gsptcuixo.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/grdwupvcj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcmqwjcwu.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gduyqkfgv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcouhiwwl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/grwdzuche.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfcetdczt.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/giqqxbscp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnqiplbxi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gnehidypp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqladpkfy.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gvwxbwzrd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gicglzwmf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gujsdfstx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gizeohgac.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gzrlwhckn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gufyrxjhp.sHtML


<!-- 参考信息 -->