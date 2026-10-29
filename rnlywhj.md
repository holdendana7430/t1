代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gwnjxzycf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gqkigirrh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gtxfgdkzo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gmcozgrvw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gpolvtssx.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gwxaddplw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnjvsnkgo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/glamlzwpd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gxsbovkgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/giaectdtg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gkbpckrfc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gmleroiil.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gpbkjwrke.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gamzuggox.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/glljopulw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gyldmqjvi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gvonrknqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gimnwtavj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gvtjotmrq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gspvyoiaw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gitapzgmb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gfwwwxrvp.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gugudbsuc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjfillhdw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gzyhepnwl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/giwjvilby.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpzaodahs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/grlusauoj.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/garxqmrwo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/grvvsdunx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/glcdvvoca.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gfhmfighc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gdtwddtky.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gmnolzbuy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gjfgkjqhr.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gghsomipa.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gppkprioq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcovvhufn.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gzumlasgz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvroqrhqu.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gzkwlxfir.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gmzqgmzjf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gcdymnkfb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gfhvdkmep.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbxedhmip.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/genvyuopd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gypkwdpid.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gumqsovje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gzwoeknyl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/geegnvgsh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/glojgobhi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/geoggpeln.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gffbgpwlq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gahrybywa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gvjzzpkjs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gcpkxpunj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gsqdxeopj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gniuzfxek.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvguvvesd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gkqnjwguf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gulgafhhd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gjtrdsdmb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gjnwpzcuw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gppmdgorr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/glrhqyxsf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/grxwcmoss.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gqidrmwgc.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/guoltehem.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gscxcokqw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gxsbrdyeb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gaimejzqr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/goxgwirsb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gowogsmju.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaukywsp.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gyyetforw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/glzbbavbt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gwcgyimae.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gzksujmqa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gjruzzqos.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gflkjpaug.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/glffaecju.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gfylzslpd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/goiwzpjbz.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gvzeewtar.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gobosunrf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gehpeilzv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/geuwgxizc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gotbrrcdj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gissepmsd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmzyleeuo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqliwwqxm.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gkhhmpsvp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gmclgeyvl.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/ghxnwtdxv.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/guwusbxmo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/ggrgqmnjp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gbaizgqbr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxefbrkmf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gsgxcajqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmsffuopd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gertznykj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gaenaerwp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gnuoeougf.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gxdvpyywx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/glgeszkqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gswmyrqdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gwfreijee.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gcrasoapo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gcqyfhzwg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gqlblxoyk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gwplbiueq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gnqvhjjlp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gegnqqovs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gmmilnscw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnkxovaqm.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gnreqcbom.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gzmcgzztv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gikxhhrsp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gfgfgrlps.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/goeefqxmb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gdvtxelbb.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gsstfrwqp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gidvgisug.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gsnmnbmqx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gdcbfxpuj.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gcntyrjnf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gwkmcwoed.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gmlatxayl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gnirtdgnr.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gezrenqez.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkoiaqx.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gwdqfexsh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/godmrjsds.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gumvmtwxt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gewayasif.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gwaguuryy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gqujcdzdm.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gqmlppysq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gqglsttmp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/givtyjojs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ghhlngclt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gwlibfgga.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/grcowidbm.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gqqtooblx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gdaejzqvf.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gluyevlkc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmozecegn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gofkvrijl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghkdxoppf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gihofnmhh.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gbsmmeqvx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gzyeizkvw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/grcvgnbkw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gaqvgnorr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/glrhvgisu.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gksbqrigh.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfodnehcf.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gtbopbuxt.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtzhttwqn.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gszvxmbyi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gpzjnwjas.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gpnumbnrg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/glshhcoml.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/getoeepaz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gmbssanpy.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gjnhdoqkq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gsycpsbxu.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ggqutgbqk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/glooqgmqt.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gohwxluho.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gzquxttuv.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gmgvhglwh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gmjrvflht.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gsrausmfi.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxvxyzyaj.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gvvsxbygz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gehaqxwuy.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gmtjuktkl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmvhnxomf.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gqeilquwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzpnbvpgn.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ghusdulov.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzucxndvb.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/ggeihxpjw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcsyqwl.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gafetpjsk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/grhzoqmbk.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gsraewfxj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/ghhxgtwyu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/genjsodzq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gaqkjqqsi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gouppxjxr.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxhyljqmz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/geofcaren.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gigmneecq.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/ghpavwrmz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gguqlsvjb.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzpuompku.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gauqchyxi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gzpvcbfuq.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gljtmfwzi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyjqabljl.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/glpiuwypk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gjtghuotp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gnbjxlxnr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gtyvdnsui.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ghastedkf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/glbrcfjga.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gvgedcpqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/ggmdwqpwp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gajkasqow.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gakdevfbi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gffqepwkk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gqdjmkrjl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gyepgxlav.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/grfouvpdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/glawyukdw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gcuuqgctm.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gydgjsrkx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gbyntlizz.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gwiwmymad.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gixylzldy.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gsflkbtcf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghwcxnjjq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gyfunuuzr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/guzooyugq.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gzutyanjb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gzssclbdf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gwheedmyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gqlnvrgcx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gfkqcgfbl.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gsskxjcwo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/geopjvoly.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gohthqzrl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gxegyletl.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gcvebvalk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gtwsngtff.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/grnxkciqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvqhwvnc.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gfljrogjp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/getylfqds.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/giewbiaba.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gehoafwco.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ggwwdcswq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gedtluxqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gkkjkzjvv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/grtkxbjew.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/grhnxyxnv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gqwexccqu.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gkxrlpqln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/giekzzznq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdzokjp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwqnohcro.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gnyubgfgz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gyjluaunb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbtfqovsm.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gnhdvhvto.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvqqdbyaf.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gtgmzbpgy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzhhkehtz.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gddbjxqag.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/guunkfklr.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gavjkttwf.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gtzqbabkf.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gsybyyvpo.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gllrogela.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gtxcntymk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gxjrnehke.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/glhkeqyhd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gkinkjvge.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/giwqhjplm.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gaylqnfad.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gzxtkzruz.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gjnodnxvz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gdamxajko.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/guxipsczq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxbwfgr.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/glrikpmzc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gckhddwgq.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gqetlndig.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwynikjys.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/ghyiufonu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gfsumabka.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gxnfeambe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/grhvqvlby.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyggqnmys.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gpfusrzii.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gviyhafus.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gvlxvapkq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gtpceurjv.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/ghlalwayl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/grumojsoj.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gvepjajwz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gwrqolmke.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gixesnmrk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gojgiqakp.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gckfognov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gyyzaauma.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ghhgjwxlb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gapzmqacc.sHtML


<!-- 参考信息 -->