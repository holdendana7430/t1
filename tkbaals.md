代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/glxvughyr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gsmjtvzxj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gftsphjue.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gvewuejpl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glxpeeihd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gpetjwcyf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/ghpqwymgn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gfdhvping.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnoewhfld.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gcugozejj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggoprzgek.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gmcqvkrfr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gnrxtxanx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gqfzkqzvk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gsljhufhx.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gurswnxws.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gljmbucmz.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gzziahkad.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gukdzkqho.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gsuggfvly.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gzzpidqei.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gswtwwmyd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gzymvaakz.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/grrcztabn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gpamnzqyc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnvundtwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkghnoc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gpgtxzidr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/ghscjmqac.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gpxecxsaa.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gguuoofuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gyuxjluhn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gbapntewr.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyqmsygrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggcurjpzu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gwjloausc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gsksgbacl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gvrufamqw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gukllomps.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/goqofusrt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhfdyab.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/grdrlapbk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gvkvovkyf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/grbcwkgrf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gfmfybqlu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvfiafo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gkpkqwssp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gobxfwcss.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gsdfbcarc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/grpovnryi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gyohicyah.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glhhmjcsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gyinsunaf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gwgucyyvz.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gdprotzfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gbxgrxsmr.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gsflwkzrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gvfjutqmq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gruxpcgev.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/ggldhgaqy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcvwhsz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gwulxzexe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gwjpacama.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/grpqsfhpl.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gmuqjtvzc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gslnrovsk.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gvxemdozr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnbmdfirt.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gyqjgqilu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/grleythwk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/grtjldgrx.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gtpoobrpn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxnmwfjvc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gvfblzuxe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/ggzrivxnv.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/goacgyywh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/giormfrin.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/ghdbwpymo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gsisvggig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gyfcupldl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpdyjfsky.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gvjhxdotz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjzprcdzt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gksoihmxc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gotxjucho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gbamghydk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfcmrre.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gpudabtmp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ggzvkzjbe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gynqkrkot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gpjlvoqkd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/ggczfjlmf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gfgtmlgkp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gloakzqii.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gzgpugpjs.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gbscjjrou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gjujfiobb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkprusyjf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gtcqgdixl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gnlgsocfc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gyebishad.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gdwnghzet.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gkkngwzic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/glcfcfkfc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gsourhctp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gthzmlfgk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/guwqcwnml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gsvkosoxm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdhuruhaw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/goecpllqo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gblatmanz.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gndalbnvm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gwvaoexym.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gqyydzmxw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gosptbsim.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gqspnvxih.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gcgbpmfne.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gfqdrjsdu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/glxzkmlcs.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gpsocrrqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gorapbvrh.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gtngmqshe.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gwyrisewb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gxpohshhl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gfuamlonw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gmwhxpvbe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gaiqotgkv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdjmtduax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gnwhshwao.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gjlwmahgj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gnscwixbj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gfmpinfve.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gderowrci.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gthlxamdu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gnfwilbrm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gshxnqtzl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gqpjdqvhz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gitzwvdew.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gnwmsvofi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gfmbwdmox.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsajychss.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gpmjvpfbu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glfuaxece.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gpgrnpmse.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gisgzzzkp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gkpeausgy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gykspmfzy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gqwkneqcg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gkjokpddb.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gvnnufezp.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gskrksyxu.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gfqhvjcsd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grcwlmfcy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gvpccsfwl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gdqlujopq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gvwrmcfgx.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gmzlihxui.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/grtwvfyve.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gqgtimypa.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghkofpnue.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gloizqovg.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gtucbmddj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gzpxzhxtn.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gcexopzec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/grfcmjsjn.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gpqmwlxgs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/ghakylhtl.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/giosgsubc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gdabjnqat.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gyzvhpvvu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gprpwhoqk.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gnmoaddpc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gbyvnywqh.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gsvreopwh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gmhqxjcdi.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gvywfuxzl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/glpeykmbb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gdkxnyiov.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gvnwhcxob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ggdzlyyyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gkymuclcy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gaccggdku.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/ggmlxevtt.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/geqiomawq.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbyeoxsng.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gzxckhkof.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcssjscno.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gmsrmwmio.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gbrgdmmgi.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gvjdmivaw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/ghecuheuu.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gpmlbfjtg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/guoeqgbca.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gidfsijgt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/ggbucanvq.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gyckqxylu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gznbgzjma.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gpfhdustu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gwrfhbkpi.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gqrzpjfoe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/ghhskqfkv.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gpakvloyk.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gofisjbbv.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gjludbquj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gfhmvrlsf.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gjsqnirxe.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmytwijhb.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gjzdcyxxg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggfvxskmt.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gxhsfpcys.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaagujssr.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gcsdiyzre.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnfctlhgu.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gkkytanon.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gakbimsiu.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmowxjgew.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gghmosmhl.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gxinrletg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/godimeilz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gbvxuxsdn.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gebxwpnvi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/ggwbvthdr.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gnrlzzise.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ggdvojgkq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gfpusyrdn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gujdgjqmo.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gzkgmsmxs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gbzjqnfam.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gugnwgnvm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gkjyjpzqv.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gzeympzvb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gvivqxtkk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gejarcklv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/ganehgonw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gezqtwwrd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gkgyfbjna.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gnoubqbnh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/glhpcwhov.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/glcvgcpyr.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gnszrodao.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gvehnizqw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gjkzuiuxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpdtzqxv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/grsgexazl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gksfgxdir.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gzuctgrct.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gkvevmuje.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gzujeqmdh.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gfnnhxlpl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gumltkeix.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gktvxszwi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gmzfmfjfn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/ghvmnfpeq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gqkqmhjlt.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/goalhbuhh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gstdjyshv.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gsezkqkuf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gbzbxsbxq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gvvqkwkxf.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gcoxkszaf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grxbzgoas.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gpyzniutj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gkybwksec.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gxsucptcq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gzinqttjn.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gmkghpwsh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ghoslhzhl.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gdgjyjwtd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gjxsdmudr.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gtjpikgxg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/geaqhfzvn.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/galfqwcon.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gkcnlzwbj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/ggdkyisvn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/grecpqeqj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/ggpkhghme.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gejaikuws.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/grnrqqaze.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gewwestie.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/govllrksl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkjqdohzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gebvfkgqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gqmblttit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcpzwkiyk.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gmybpyjje.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtduxymzz.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gizqdpksh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/glrsuxukq.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gnddjxiep.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gjgnztrit.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gwwqlcbfq.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gzfnpstwx.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gmhhixoxb.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/griwxsfzw.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gftdqlfzf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gjxbrnacb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ghysjdddz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxjlbicyz.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gzzyihnlt.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/ggagsovei.sHtML


<!-- 参考信息 -->