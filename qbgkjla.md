代发 wailian999

[O02] 使用线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcckmoqnw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gooajnjkd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gquxhvmpb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizhsqysa.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrkglmsm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gjpoubtjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsmiuvit.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsntznvr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gxijbbrbb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaacngby.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdldoukbd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/gkjcdatzd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhfnzoep.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhnqomse.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gieyalbjw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyiqlanf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqfmbamss.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubdlqfad.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaqwtnaq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyecaemy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxyhvsil.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/guayxfkej.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfbotaent.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/guiefeibo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gmkmfgrfp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueudmihq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gawawswtx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fanxiaobao.xyz/Article/details/giywvukje.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwluvsel.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gcztagbss.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxagfowod.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomgsbgvk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyodvrh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gwurivrmq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmthrwhhq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfvpdxb.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhbdbiyg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/gukdlfkux.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghflxangm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gbyswiebu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefgiuzv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/giwrfuzeb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpazvsede.sHtML

Ruby: // fork 块
来源：http://mobile.fanxiaobao.xyz/Article/details/gpozvfpwi.sHtML

C#:   Parallel.For
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxftffuw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjjwchph.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshswzbxg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkiuwmef.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxayczod.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbirrmzra.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvsleluu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gjdjpmaoh.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gjijddzyu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gabdaizxc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gahndblfd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftlpaxw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdynvlil.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbyvbjn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fanxiaobao.xyz/Article/details/guqsmlhwh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqmsphq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxvzjgxj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjpblyas.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxjuytkr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/guujowxsq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdscebat.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gnrwgmvly.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpzlhmscr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjyltjc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzodbrpt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gqmggjscr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/glhfwpoga.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvregnxhe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbqtmfw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqqhwlrl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/glcgxagau.sHtML

[P04] 求长度
来源：http://blog.fanxiaobao.xyz/Article/details/gxlilgkuz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gctqfpumy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gipifvbuh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcnspkdl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggodrwjgu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gfqrqqrbv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotfebbk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gegwcwgbs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgrdbhr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fanxiaobao.xyz/Article/details/gvnbbppsk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gtttkthho.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzobnmn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fanxiaobao.xyz/Article/details/gejognasx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/guqwrlwru.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fanxiaobao.xyz/Article/details/gfwtmfjpn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkiwgtsp.sHtML

Ruby: a == b
来源：http://read.share.fanxiaobao.xyz/Article/details/gofnfcfti.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgzwbntq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fanxiaobao.xyz/Article/details/gzsqchmqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/glipvimpk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzsgnjv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fanxiaobao.xyz/Article/details/gjlhumbzv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfuyowbv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwgviqbc.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gewdujhjp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fanxiaobao.xyz/Article/details/gabziojzy.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdwdostzj.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gabzvqcse.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlfmxrhw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gezupclgo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/guxlinwao.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhrwqedm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guusngrim.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsrdeobp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfikucf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhznisai.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrxrxkbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fanxiaobao.xyz/Article/details/gosrcmxzg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gypafzczq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fanxiaobao.xyz/Article/details/gmiuyjluq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbbaxppr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtvbbtyy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fanxiaobao.xyz/Article/details/guhedqqzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzigyign.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdbiege.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgotfatr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmotwbno.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtzmqccun.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryvbddz.sHtML

CREATE TABLE users (
来源：http://mobile.fanxiaobao.xyz/Article/details/gnonkdxzt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzhmhwem.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gogfcmpde.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkkudrms.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhfhucf.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuelbnlb.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/grklgztzn.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztyjkoph.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvrsxluc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmkwmojw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpjgbwo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrkybwsd.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpmeppha.sHtML

[Q03] 增加列
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmxxpfz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxzyvaat.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgrpndj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/gehzavjrn.sHtML

[Q05] 重命名列
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwckbaji.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/glyqrdtqo.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginxeagbt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfcwxtvx.sHtML

[Q07] 删除表
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrpyyyc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/giegjuupk.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhmwduvx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpgmhiyx.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gljvuhvkx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gexchfifm.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gdtjsbcdc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrtvzjam.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gndcdunts.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/guosiaejw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwstjsmx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyllisnv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnngqbgo.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbowxnxnz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gacfklbbo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdydrgno.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/gscexfhzi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnnpeohw.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeuudeeu.sHtML

SELECT * FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzereysrg.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgunrovc.sHtML

SELECT id, name FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnufgndd.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxembknup.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimkytxdp.sHtML

[Q18] 模糊匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gqziejmaa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gllwopeae.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdocjwndw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gsckiaepb.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gxfdfzcxm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiuscpbv.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjybhhadx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gealbrlfs.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwujghwlg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gnnrfymwe.sHtML

[Q23] 分页
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduqmhkyl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutblgzbl.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gxamfmymo.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guunwjlwn.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gnehkefke.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyphfvsh.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzuiykwq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggxfzaluz.sHtML

[Q27] 条件计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrmtgpes.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzlmyvsfe.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glupobcgk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gusscfbby.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/getesoouc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmeawvpb.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gekuwroev.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyfobnbp.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gxsdxjewh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmncbgiat.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grcczswji.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gsoemtddz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/geopvwpzz.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqzwovf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnydtrzh.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gegauohjv.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzicmpvgo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmitmghrx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxtjvsrp.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gsdkgradg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbsphknye.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdvabkno.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gssepnzak.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeirqlge.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gttmfmbrn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnmvlmsp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gahryydsl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/goyjrsjue.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gdppotcpr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbolesoyi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gcebzcyqv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gknfodzoi.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gnuchudai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmelmuufw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gyabbaepn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkhktjyb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkgmldxb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudpckqns.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gcxhdaaso.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjescocf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmuktyh.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrhwrfhn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gqyewfhkq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgvpirf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnjfrjyk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gccahkrbc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gigdnlkht.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjfpvdgpu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gofnfsgrt.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpjihkq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gobcxgtbk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gjuwvmpve.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gybqkrfiq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfzhwxir.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/guvjscbmq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqefjks.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwlxvabq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gqdukquwo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxywtabj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdktxwbwq.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhcxpxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gywfxizai.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdnargei.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdasixqsx.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogsbgosb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gbhpokyru.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gksggcshi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gavnqoqws.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvukxqyhi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjksolwtu.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzypmvzn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchmjdrle.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbdkkrbv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzudwtk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gsikndsca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gajjguers.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/glwpbbovc.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gsibzcjxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gaxpmqwar.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gfgncqtqq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulkiamkv.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbiwyort.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyorsaxa.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhronvzm.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggazemsgl.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwclqwdz.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajxldbbr.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoslvtkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gxgggolzo.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gxzwmbwgh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcirgoeb.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwzypgra.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqdcobqau.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghhleklvz.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/glcxgqdae.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpckdlpix.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdzkmhan.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiqdxutr.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtmlqrbo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/ghzhsvspe.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/grguidxel.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gthcswwvn.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoeerjkl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gqukcjmoy.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gimamhebh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwazvhpi.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjreknisx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbzpxdpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gpdidrpgy.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gyimonbgz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlndtqf.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gmvmmurun.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnemtyuh.sHtML


<!-- 参考信息 -->