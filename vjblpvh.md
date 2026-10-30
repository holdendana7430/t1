代发 wailian999

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gcvwfztye.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gtpjaosaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdnmuksqe.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gibybdeem.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmnrjuyaz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/geocjkgsf.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gdnivmibr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/giuqftcsm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gektbrtay.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gybctfumi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gmibukhjw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/goebkoyux.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gkwuegugt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gpacntixw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gdzeergzw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gbvytggxd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gplftizug.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gfkkkeszq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwoqeichr.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gvmmeueex.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gkqdyekfc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gwbmesgje.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/geilodjxv.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gvzmuyxtl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ghkwbunwq.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/ggkfdwtmx.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gjqvgnvea.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gsnmteoaz.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gyglbvcrr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/ggxcftjfb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gasdxqmir.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjvcxpvpw.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gmapbzobi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gfimufqrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkbzkzrcw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gahhvfqgi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gujsdpcwx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/grgassyaw.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gkscrfwnm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/ghjmbjgbr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gdpfrirml.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gfddgqhsj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjswikpis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gbgjihmms.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gjlgnlztx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmceuyeac.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gbzcdwdws.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gjhizuvgo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/groadgteh.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gpbxwmksq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gpeymqrkf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gnpmpbapp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxgfihdym.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gklpezmfk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/garcnsobi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gqtbykigk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gaztqbkbi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gqqwfeiye.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gimsvifpe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gexyeqdsw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gyxrxsmea.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gpuoqbzns.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gyarpjauy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gqqgameww.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gbgeksxve.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gyyjnwpbx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/ggxlvyqxx.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzhkrylrx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gbcuxseer.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gqtvtscxf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gewcmapnz.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gpsokjrhx.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gckuluslp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqvautzn.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gtaskpyzs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjfzcohld.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbydqffdp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gceaxuflu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gzdhwttat.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcginsuqq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfepdbjqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/grwdsgudb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gzwkhsvrn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gpflilyli.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gvpmnfeuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/glhmouisf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gszrweugh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/grhsxhxyq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gzjndxlfq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/ganotmwon.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwbwaundi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/ghzjjioew.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gfhiiaxzb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gebsmpowo.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gwxqpvyxe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gciwxdves.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/giwfimwjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghjvlklgd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gvrnqhxmz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gykiivycu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gohcibpnw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/glxywyohp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gcmjutugg.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gjpdipdts.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gkpvxnkgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvkdfsgdc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gqbghwnpf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gjldbohyx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gkknijqtw.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gtojyqtpx.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gxfmmqnxv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/giauohknd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbodhwsga.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/ggyrlipih.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gcvcerwzq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gwzgknmia.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvwdcjvkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gejctckjh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghqkmziid.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/glsypptyp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gkdundgvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gsaugohdi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gdxwukpgi.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gjkhabkcl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gztmwsszs.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gdfbmgiqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcehmnvhu.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gnklhanhh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/grwxirmdb.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gywuyywcg.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gkpjgyriu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/geknhiugv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/guskciojg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gioxxjryu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gpfnxkrff.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/ggrpliuqj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gzouhwktr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gtmugoqlq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/ghfryfekw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gcfqpgtjg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gryxkavct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gctixagiz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gplizogyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gumjecaui.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gcmhwcwic.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gzuuxjkua.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gkxmumsny.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gdlnpxzhx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gguvzwjuu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gkvuwanmu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlfebivx.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gwiekmmjm.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gmmlyhrxd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gvfxpcbey.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gvarreurl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gcxonkcsn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gmpqvhxzy.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gnlnspzmy.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gpaubpamf.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gktwseiou.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gcyhjnlka.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/giolatbww.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gfnhzrnub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfalhoii.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gsbnizync.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnwakms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gjyztfepy.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gkbekdtoa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gsnouulmr.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/ggrbaehth.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gbjspmeit.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gmvcpojoq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gnywptnhn.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gavfnkeie.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gavtcqvql.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gokacsmfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gmfiyjpgu.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gzefdbwci.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/grpblehpx.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gnxsjxgsk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gwafnzyhx.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gmfbbevza.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gzbibparj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gpkunaegq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gxdcozolt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gxouhaszm.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gywkcojxf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gldyzdhjy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gitvqrijg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/glylpeifr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gbtapjlzr.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/glcjlivmq.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqqxztnpk.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/geyzymtvh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkypmoobm.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gzfcjvqnu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/grssmpwvi.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggxagpeyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/grmyqscmq.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gnwohtlyi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gwgkxibta.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gykhbfpou.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gghbkyvkw.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gpmuyzmda.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gpezsckxj.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/geozocwtz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/grzaefwtu.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gwhygwtlp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gxhraeunl.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gqcxdgruo.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/guszjjdrd.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gbykqdajp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gupyilhbe.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gjubbxfxb.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsjjcamfu.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gznvebwke.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giwbxoblz.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gxuxepvbl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxkkejdch.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gscesrjyf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/grfdzwlzr.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gmrdyddcw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gyyoicbly.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gdbvepgtl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gafurfcjy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gowgratwx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grvhizyeh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gfshmlwgp.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gjwzdwtbh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gcvvcvgwx.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gfftlkctd.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/geogdtexy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gmlgbnfvk.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghkpmikbo.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gcalgyzsw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gbjixaold.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/glwfvcaqq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gwxpbosmq.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/giyrlicwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/grnwecabo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/gyhdmbsxm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/ghthikgch.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gydbcpiwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gkedxopmw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gsfyninqu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gbtidclal.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gipslzspr.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/geawscxjm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/girqtsllp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gcwsycsfb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gxkvprqun.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gjkmfauah.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gbidjqczs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gmgwmpmdr.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gftqrerpn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/ghraujjih.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gckcmoclr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glaciraii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkpqvup.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gszddjvyr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gnldepmbn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gzbswuxmc.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gacpjzqmx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/glcyeqayi.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gtvoxqcng.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gcpjsvrdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gpccztihs.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gqsqppblc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gnrjxzchg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gkjlnuhwo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gngpnzkhn.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gegufwrkt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gfizkemvt.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/giwmbyvin.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/ghksyyvor.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gtxuxovgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gbndnnwma.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/glksycmta.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gstnlukav.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gbktooukc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gevpqztrv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gfsexvmaq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gnptwylkz.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gfawmsltk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/ggdqublsp.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/guznpomxr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfrtykosv.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/goxbzvrgd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbabemvag.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gqlmlvfum.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/ghxiotslq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhatfxri.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gumvqluxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqlrdzvis.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gsiejjoxp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjazdmvpn.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gjavmraec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gltmbwvti.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ggwneyaes.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gfryuklws.sHtML


<!-- 参考信息 -->