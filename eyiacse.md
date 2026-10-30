代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gvsdfxone.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgtecuk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gjzlzxclm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gorolwsah.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gjzrspzbk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gnruzwtbz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gfbzymelh.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gtoyjonxw.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/guakchmyu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gxmrgrlqe.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gaifjctss.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gfisyrkra.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gfvimwmxk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/golxjazjc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/giebleppy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gudzcidfi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/glnwnoksp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gjykgnuru.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gawiohcqm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gronntiut.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guwjorhwe.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gayddmyhq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gywnwdjjf.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gpkyjdtbq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gqscirkzc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gikpkqaxo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gqqpjkbwd.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gbnvgkxfo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gyceythsk.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gojcyhize.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gdgsetiuy.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gubkmgkfg.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gjogmbcli.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/guiglcdjz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gumwgtlcy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gxpibwssp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gaujclxia.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gsdcmejcn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gjswagjte.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gxeeerkdj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gcibsxauv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gebvzquqq.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gegrvrjmv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gmlboivim.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gmetmfdtj.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/ggogjpmxu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggehnlhuf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gdructcns.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gquwpeczj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gbzjhxfay.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gwivoqbyf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/grixbfbzn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/ggfzopzfk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gvnnskyhf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gzhmbgakb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gaqnpgjio.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gdssnxpmi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gsjjioydb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gyndnyolo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gwibvvckx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gvlunznsr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/grjnhqvhy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gblsmqgta.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gxdnduhna.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtfqfgdix.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/glpksoldx.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gbyjyuasq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gnibjmrqq.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gimspidxk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/ghjgroqrz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gtksvbamx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gxirpcgty.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/grofeeuwl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gtirsygmr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/grztagyzw.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gyzjtiuua.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/ghvloskdb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gatxpsjuw.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gckjzywpl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmfglhbfl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/ghwbigrgz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/ggkknoqnh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gczsyccua.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/guusrcuyl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gndpxgrbe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gidrjsgaq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/goxzfoxdj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gwowkaich.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gpprshnjb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/grmgqptaf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/goebpgdbv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdnlwldvf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gnjzlzcvc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/ggxmpqwez.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gowycwfzz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gmdiqupnw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gekvzmfbu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gisqcuyvz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gclyfeyvc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gwrzyjrln.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gzzjernwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gvzkmmxop.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gtaigmfve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gclxbrfcw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/grlaazovs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gknpwfqji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gofihrcmq.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gtqcdvzjy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gkxmdetsr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvgtovzrc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/giumgfegh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gokuhpvud.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gsqnokedr.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gfcqomawj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gnmutthwa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gfrruxqhd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gzskcrctu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/glkpzbmno.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gbfhavmbh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/ginwqotbd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gbfijkfvc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gohkzvtec.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwvqulpip.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gumwzvodi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ggxrltjem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gwfeatcnv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gkeaokydz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gciqdyptf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gyyidyshd.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gmlldkiox.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gjbebcfma.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gsbokxrao.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/ghqanllne.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gullgzsod.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gnjeflsof.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gbesaagzk.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gspqquvvc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gtdpemgxg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/guaxbfihx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrccwue.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gedtxyipt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gecnztysc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gtirdawoj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gskkeqqyv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/ggbaxwbbi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gpljcahha.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/glwabyseu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gslhbvpah.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gveotfedo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gklqxdesj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gceyffokh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gdxueirep.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gecpkgtxc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gccsvxxlt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grptkbczt.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gzbsdcwas.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gylwzqprw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/glehnvtrv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gzuwmqpiq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gwlqdunhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gdkpvvdjm.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gptgusddn.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gactwtnil.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gfcsjkegl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjyhtsafd.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gcoqkwxov.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gckohrspm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gflezyjur.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gppqikxyy.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gmroffnns.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gzdtcnvyq.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gwzcoochj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gcfwmrwue.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gmakdzzdh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gujrypvja.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gagxmdvax.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gjvcnpzcy.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gthxdvxnq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gghbxiiam.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/givfymxss.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gytvrobmh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gchbfrglh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghqknttag.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gknrjoonx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gomowpwll.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/giiprxsur.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gehzkutel.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gwddiqhmk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gwcoyrlyu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gftyihfrf.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gvwtbhhpx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gbxeorvri.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gpekcsqsu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gtqnpyhmt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gxqnwforq.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/ghinjxrau.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/ghyvfyeyb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gpjxoxcpv.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gezuoyvvi.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gosvybyxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gszsvepmy.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gwskjcnif.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gauxaoypy.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gcoxvkpxn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gshzmxnek.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/ghfontcre.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gpsbfxeeu.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gnkgkemme.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gjmzxgxld.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gwpejyvqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gydgwbkla.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gdqgiiwyh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gxtxmudmc.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/giayqyshf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsakmttbt.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gsesqbyfv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gtlmzrign.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gpdtkygyu.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gotoufqam.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gmzwccasp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdmzqyukw.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gmxylvqgx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gcxfmoria.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/giutukmuu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/garrpjasc.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gatdeuwge.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/grvawezpj.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/ggfglunnn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ggpyaipdj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghfimmqrl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gpeptzuyl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gkcjshccm.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gmrbhidqb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gvouuluaa.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gyretlayr.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gfaaxtfnt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/grtrsqbgn.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpfwvnmfr.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjosudvqd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gxexkpfmy.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gpjdiwpmq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gornmfhnw.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/grolfwtrk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gmsiqqdxi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gekxaspzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gkznzmrzg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gddascfth.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gaovfhksb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/glbesilgg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gcriamgeu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gxweosbdu.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gbrmpbhgp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gtoxaprig.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gzbskqzkn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/grecorjqh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gtzzjekge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvdktmsql.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gemlwxovk.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gunjagyqt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gecdauuex.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gxyehzjfm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/glnthzdul.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gxoblfduk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gkoinfzav.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gacxzhmgt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gnpmsxuzt.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gsuzjzjbg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/glmzveavy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gfyfnximw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gphorctsq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gfyqclabg.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/goodbulgu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gcuuptjvu.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gppwddfcu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/ghlupqkxd.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gkpxikqrs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gifqszemn.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gamlmusvh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqswdmcmd.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gpuvjnulr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjpuculuy.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gsrueuayh.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gnpqznboj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gjdlgaigw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/geyavdygn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gvgdpvnkw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/goyribxxb.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gfzcrtssm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gdookycxy.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gyzmjpnyk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gmjkowsws.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/guidpovfx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnuukzazc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gtqvnvrja.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gwmuldwet.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gddbhcffg.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gkllvpyuw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxigmoozc.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gyqfijdfh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gletzdtrf.sHtML


<!-- 参考信息 -->