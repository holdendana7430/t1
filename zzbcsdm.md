代发 wailian999

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxoslbful.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gszuorwzq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/grdvotwkm.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/goypplwyj.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gxzgqyzxu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gpqlltdhx.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gugvvatse.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gllniguvf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gbtizerqj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/ghnignzwi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gnnguotvc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gmrnwhrdl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gqfzexxre.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/giofkfaxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gkbmzxnic.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gdbqxguxt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnclyyxjs.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gzqfozdvz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfnhklbkh.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gjfcnqyoo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/grsjitsbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gfpbrunxp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gdzhmofeb.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjgzvvvuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gdxvsdnyf.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ghwirxgab.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gjpxtewtl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gdoxwxplu.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/giscekowf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gsserqujk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gpccgupqr.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gsyejvhgg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gcmdesyci.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gnbwjkljm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjhegoeto.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gldzwssrp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gefjidtsm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gejlnvgtl.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gsjwjttcq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gestmzslj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gxhyyxsuv.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvqxqmwgc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gixkoyuga.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxhufsd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gdmekdbbe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqqpjynhs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gveohenun.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gugafmmwg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/ghnzptprr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gvewftixz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gdjfjwwfq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/grfukagmq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gqnuglxpn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gtmgaicgn.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gqjytsgvu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gpzmkphjn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gofzasidb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/giobodlll.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/giveavkjk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gvxaagvci.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gorvonavp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gchvwhcjk.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/giwfbiygt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggficycpd.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gzulzlern.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/glbkwenkt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/ggyddzxom.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpnlduovg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gyzjcmcod.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gceavquao.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gwypgnakr.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gbmgwkeev.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpjbaskoj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmpjmvhnh.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gqofdubxg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guqynnnrr.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gydiuujlj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gtlykrvau.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gbjanwzua.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxltjrchs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gmhdhqbko.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gmhftdibx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkcavjdzn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gjhjhzihx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gxklmbuuu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gmhurhlxt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/guhihsjhf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/grjrgswfd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gwmlqvake.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gzwnrgxuk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gncyhsxfq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gfoxzxswo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/giaeswkiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqvqgrpov.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/glkdctqji.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gnrycqvjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/grgnlxqbu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfuepgcwk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gbztbgkow.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/ggmlmvehk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gtzyaiwih.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gmxtsmfke.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gqbrcvjqf.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/glazseszg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ghobporkz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gceitohtk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gueskszwy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gibxtyxel.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/ggltiphqy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrkyrdhk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpfraqhji.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gfwdapjfu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gmupdbxks.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gttgukcme.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gtgcdgcwt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gzmyapcbr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gcxhombkd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gexwgwhxi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gkznamova.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gqspxyzub.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gvjqtbmxc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/goyowefww.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gshyfuffb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/godvdiqlf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/globfnlbg.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gxwztrkgf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gmqdwyxni.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gqupvggpe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gvghcvotz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goeuozckv.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gvpotbbhg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ghbgoaaso.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/giktxvork.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gdacoesri.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gozkvtmti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gviztwtnt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gbnxjjdwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gkfhuinyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gzxllhbae.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gsjrunaao.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gktkfwmts.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/ggegnqohz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gutpkpmsi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gkjexoawc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gacezrvkx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/ghsyusrvl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gcaszovea.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gujizmttf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjasyjjmw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gdfnputxe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gialvtgrg.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gwzkpvzpj.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gvkaoztlz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gcxbqpyhb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gdgamansp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gpxfwekjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gpduoogsd.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/grlvkijhh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gpaysajoj.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gophebpdy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/guwdsvure.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gocettaki.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/ghrrcskun.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gdppzhrtb.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gysfwdghd.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gydwyqfdb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gwhzjdksi.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gnxrvsruz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gjgclguwz.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gathfwdwb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gruxgihgm.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gsfgiszrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gsgibwwjg.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gmlvzdyit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtzgcilac.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/grrtzrtod.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/glxlnlfzb.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/giblhcmpg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gawqstjil.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gqtyyahki.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gcoyngpah.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/guaxvjaqy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gvcmntefe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gezcdoxau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/ghpoozkww.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gepnlxxyw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gpimsqvlg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gpkpcvnqa.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gwspbptxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/ggtusklwi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gyckkwfmg.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/grqeljbtw.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gngeujsmh.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gegcgtsdo.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gddcjkfpn.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gmtpisdjs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwzreqjyp.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gusqcklwn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gdkrngwqg.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gpamajjql.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gfhipmgth.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gscgsjusp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/guaorjkxt.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/grxppadti.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/guddwnkmf.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/ghlkmmify.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gzoymhgtn.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/ghjebiwws.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gjojiejuo.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gnnkkyzjw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gaaqicnup.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/glgqsifmu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/ghmetdekk.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gskkmpcpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdthzczur.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/ggehiyhle.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gjvxjjspy.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/ghsofjaxm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gueicgrcy.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gjjzxaxip.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gugkpmpar.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/ggqajnhlf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gwgqleveg.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/ghkoheyol.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gqxhetsip.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwofltprq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gsurgqqmy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdmexoind.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gwoecnvxv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gclijaqms.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gjaybdzvc.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gfijetcgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gfkhvracd.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzvbbpktn.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gxlsgtyrn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gwxagnmws.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/grpbrazai.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gfzvnuljf.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gmkjzjgui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcakhld.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gpzmuftrl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gfpkfmazz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gjdmhzkyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gyribksfv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gflfsiddv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gedxftkpd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gfnchwzyd.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gvwwaysgv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gssbaiaty.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gpcfkuobv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gobhcyxov.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gfnftoodn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/grgpqatuh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gdrnthcun.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gvsfobfgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/grwnxntes.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/grutbpywx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gsalhwuyy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gvfzlrkeg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqvpmfbvs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gandvfcfp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/grxrlengc.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gklbixwws.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gsepqrhzv.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gewqwfxcm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gqlqhhxor.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gyzbugfzc.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/glgyeytjr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gqiukrpsf.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gupxznnyp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gnnvudacv.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gslzlyqfu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwjoiwaas.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ghmvzqmhe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grlvormln.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gdgdaeuhe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/galscreji.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gkfdgfmjl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gqhfozncq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gwxvsarce.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gseyjfgty.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/grpzmmhdj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gtazfbjeo.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gstkroqzf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkkbvqxpv.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gvbljyudq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/ghqmoalko.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gnczxbptp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gdbmpviro.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gzjlhimfi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gbuwaldzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkhuzhprr.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gnaytrkcj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggygubfnf.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/goobculle.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gkrjolvgn.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gwguxzych.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/glbxvdukh.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ggvhrxhtr.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/goxgxhqjk.sHtML


<!-- 参考信息 -->