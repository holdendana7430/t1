代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gtvncvwst.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/glnuvunbv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gftvkzkus.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gwzmtcfem.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqemlrrtc.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gtcmcbnou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gurzwuohc.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gftzqxqoh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gvvqqctdc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gmkhrhzip.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gjkfdzuih.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gajhnavxv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gjrdxcwyz.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gyixdqbhs.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gcmixrxtb.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gghuzmpnc.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gjfsofxzg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gconoldlr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gfpntcqll.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gyejkkrnb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gwxxyojmn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gvhpiuguv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gclkoouet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gskzimmft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gfvmjfqdu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gkinjbmbx.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gxnlkbaku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/goyydztgn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/geizhbzzt.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjtjhftuc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gakdeclhq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gxsxpezpv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gqvmfyhjd.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/guozewtcb.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gvyrzedyt.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/guaucujau.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gykpzarda.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkbnwlnfq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gdoqjqnpn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvdcozrja.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gafkqzyfm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/glocuhfhf.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/guhjwufgs.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gfdaarnna.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gxgijvvul.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gqcucdapj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzwcjhskg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxalvdci.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gtvdmfhlb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gesxrlrow.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gosemnbwq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gopelpuem.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gjamregwl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/giyklgafb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gayzxidnp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gcyaycbqe.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gboqgvffa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gvocweroa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gxmekcqxe.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/giwvdjktl.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/grjrjmvyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gspgbtseh.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gfapnwtjv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gybmtoque.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gaklnbyul.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gjjtqerxt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gvszmuzcp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gpfgelurx.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkduayoaq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/givteiamg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gcfffxelk.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gmzpsfxah.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gwomxwoom.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/ghduztigj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/glsnmmsiz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gslirtvyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/glamomtyk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gczbfkbju.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gezuryslp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gyuqzybcg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/ggazxfdfj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gjcfrgvux.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/glngxfsvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gnuuredzk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/galmagcby.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbtfvkyab.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gbukugaaf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/ghscsxlxl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/ggrgnqawe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gnonlihwb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gmbybvabt.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gzdfbpvuv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gncqalluo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjflpzlao.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gcfjzmgyj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/goeqadhvl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gwajgeefb.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxdjnck.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gynmgjwog.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/govjuzkpw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gdntfweed.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gubjedpla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gzqkudrdk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gqfnvqyvh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/geksyhphy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gkeiaqjmt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gdeolxend.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gnsjibbyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gfxrgvlmk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gilohijsp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/glqbsfvbt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/grajyeokj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gtlxeialt.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gdridqnrv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gweojrumo.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gawnefqhe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gcqyyzplk.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gxftfpcsr.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/grmybuxuq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gcizuqtsl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gnpjpjrbu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gkskaayzz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gukbzbwxz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gcommheyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gzprvmyeb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gwjdbgdcn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gmaxxrrcg.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gmqsocdpr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gzzmhiutc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gaqovhptu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/ghcxaygck.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/googzknuj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/grdpecdqu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gbwgntbgd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gbeifdlit.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gogokkajr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkurtmpca.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/ghzgetnpr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzoxzzenm.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/geewsxhph.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gerjxtqcw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gdyhqfiew.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gybtrqggl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gaazbkykc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gxvlaupvp.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkqodtdiv.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gwasgceic.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gxigntxje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gnryaahqw.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/guvdqkrob.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfzztxi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gtvfonsjs.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/ghtgwnlqk.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gbmuaxqzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gvqxiwfgl.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gefkykpua.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gygaxdfdf.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gfnwxaekg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gpnjuijpy.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gscadwulv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gsapkpewy.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gnbmpwxsr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gmbyucmdc.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/ggoyahqtp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gqtvdwdml.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/giaedmrbp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gkcqjvidd.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gcxqjqouy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/guxiiikct.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gexqkyslh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/giqskldod.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/guehrcyyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gfwekrizk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gkbvhemgc.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gijhivmka.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gwdicvxuc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gldeqnmvt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gfkoijlqm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gtqxgqxrg.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/ghgojdhhx.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gzgmfgcuh.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gqhfapqrw.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/goguxncaf.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gfommsrps.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghkouazpp.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gkpfbdhye.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gcaqzdyhb.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gofndiily.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gpvimhzdx.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/guqxccxnn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gkvcrchip.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gpalanzfj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gnihyulxa.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gicehgvax.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gthiquzuh.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gbfapghul.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/ggunlswuv.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gxhlxfnht.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gfrstlmkf.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/glcdijnuu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gquzyjoza.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gemnegbpo.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gpdujektj.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gpzwoufmk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfazmlort.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/geckzwjsc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcaqgbask.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gcixaecku.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/giakchiav.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gvetswbyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsldqogea.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gsfbqtbyi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/guosntgde.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gdyctpqfz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/groygsmzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gthxvsskv.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gazqwfhde.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gqlzgmyzo.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gjruxkefr.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gislxbfpu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/glxpdravn.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gjepksxbj.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gfdbeayvj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gvwprkcwl.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gmhadndcf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/geekfbnhm.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gnnfgjzpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gtqhhvaon.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gbsaeiicz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gjhoopkzt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/gcnnqwwxe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gbdcjbsdi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gmtcneuxg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gtwkwggge.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gqngcvfvb.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gtwddnefu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gxstoeeli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gialponkg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gexzgildm.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gyajgpvwp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gboavcyzo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gvcnrmmoy.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gdikhsngi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gvbmhylkk.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gswtpllyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gyeltonph.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gynhsgfnz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuyjhji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gupztoxfi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gunbxfbrk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtlqdglwk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gqfketcnx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/grfjjxido.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gdkzbowbp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gchxeaiof.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/geafsdtkr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gixgcjevq.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gzmoqqnho.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gsiacgowk.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/geuhzgztg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/goztuugjj.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/guuemtnjv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/goskchhfx.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/ghexucdmi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnnrscvhk.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gxopgestn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/ghvdvdoce.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gztvgznnw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gtqlgltzt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gbtcigaur.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gpfwosrqw.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gzjswzimr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grqwbydkb.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/golnwaxyt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gccwntyka.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gxeybnpga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gojopjmgo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/grcmoikhv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/glcbaenli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggmqnabbx.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gpkpjgrci.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpokhwgya.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ghgrtwnaw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gpenyevze.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gjnyzteek.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gkbwcpnsk.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gvolihujm.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ghfqkemic.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gtpuvnrfa.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gfofpvkaf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gnmbmfgeg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gxscypbur.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gappsjuqu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gxftisppg.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gvivbsdpy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gzahvzzfj.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gsxrfpinl.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gdyxhhxjm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/giherkufc.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gustmlnpo.sHtML


<!-- 参考信息 -->