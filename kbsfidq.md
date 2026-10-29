代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gmjkpprvo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gojayeyur.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gonmhcile.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/geclizrkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gskcijujd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/glvfpvivd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjibyshij.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/giqgqdiqx.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gqfvkncen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvnepjtxs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gysopufzo.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gswstukda.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gopifzfyc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gafrktewb.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnbbbioqw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gawqvqaoz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/ghfjbelln.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gwzcfynpm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gcefnxtjc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvnmlycin.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gscpgckkp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gxofrokgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/grpgktafq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gsohryyys.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmhrtwrno.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gcrlmiouy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjcwusgjn.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/glqkmtyfh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gbmtetgmo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/ghbzsfisu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gzqwkeoin.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gccxgsvww.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gyslvhuwj.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gevkverya.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gjkqklfkf.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gshurghpc.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gxvymtmiv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gfwbnivsd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gqxvuuyyt.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gypzwshnt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gctnhudys.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/guxmvqldp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gjvkgckso.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gvehyyuyj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gbmklqvul.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/garrdzwaf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gthkacuqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gomjgumjd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gkihioxuj.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gganjgjtx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gluoqinkp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gqvfzvkna.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gsvvbpsmq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/goneojnos.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gnbiukbnj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gebkrvxnm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/ggqssmyjl.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/glmugbmor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gktikwqni.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/goklpdgse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/ggerhhcah.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gyhkoqpwq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/genxpjbqm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/godrwxqau.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gifsqhnam.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gryoouomk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpivbyexp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzhuhhusj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gzibnyijn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gsokandxd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/grsbfavrv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gbdhicxlh.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gmbkqyizw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gotmzfgbu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gcjnexgag.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxrgolkho.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gjulbcgmy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gbpsiuisf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gdmtbnfcp.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gcolbfpec.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gkcakbcnv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaqqmyqhv.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gzoirlhbq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxygjttrw.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/glthucbrq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gmeigbtcq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gyhldaplc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/guczwxarh.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gxqqjpnzj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gcqwixtil.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gptpqvdmo.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gsgpfmulj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gvcwgprcy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gyoblxkdm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/grafocsca.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gcbpdaqud.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gumsmkcqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gdxciucrr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwejmokwj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gjkywazyf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gfxncnfqs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gpjmjniwk.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gmtmvvshk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/ggqbkhkbp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gqejinwve.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gqagbnhsz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gjfoffqfp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/godnijubn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/geyubnldp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gwlsupmfu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gvdlhbddr.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/girrnnpip.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gwuhnjbgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvwcjlyeq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gpxdcajtm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gnmyarkmx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ghbqcqygh.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gmlfrzlia.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gbmtnczfa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/grprkwkcx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/glmzbkcgn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gfiiqfgsh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gtcpbeqip.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gdhtnuymd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/giczfebnr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gczacszwd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/ghjnvximv.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gbhpalshj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/ggyliwclh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gevptwogq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gpxjcbgaz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gcdhbkgow.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/giefosrgl.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gnnevcpmh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gpddycinq.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gmmrbskvv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gfveswowv.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwbnycfnc.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gnoyyzdpv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gybdqygcc.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gbjbttrqx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gjyxlynsk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gvojfhdxq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkokeshar.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gtaizphzv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gdoxtxgsc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbsrprrlp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gbdfdwahp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/glbvzhdrs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gcwicuelx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gjkueunbu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gycbtrsld.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gobcvbkag.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/geslycrkv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gydjaahfq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/guqrabgnu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsxqaukpe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gtapahycu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjkektzfk.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gqtaxwpug.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gxuiflnlp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwubvylyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/giyoewqan.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gllqsqcap.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gvvmbquud.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gfyjmwqoe.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gtbaieqxj.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/ggogzepzj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gvmwijqvn.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/glvhdobgn.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gejcvypgi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gjmjbhobw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjbjjxvid.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gofhzchrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gnykqtalc.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gujlrcdxy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ghxoilzrg.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gtysumvbh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gteziesuw.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gswqqncyg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gmbzhjcrg.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gtgfftmub.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gpzigyrxs.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gqeakjtic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gizyprrzj.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gsddwxbfq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gtgrzpvni.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gmubqwptb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gcrzpzlll.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/guwtvdnma.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gibvopcmb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gvsttokeb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ggjchxjip.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/guhmbnubs.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gnupialgs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gnhlsnecg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjtgxfu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gjcqehhhw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gfebwmihl.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gupckqdgz.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gppashhes.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxfoybjta.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwqmzhdqu.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/grrvvtrgb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/ghbwgrkzp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvsixbhfy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/ggwkwubeq.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gmukzofoo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/girbnkfsj.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gltjjuyte.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gugbwylgs.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gheihtagp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gjvysyxnd.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gxswiovbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gbfreryth.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gzeictxwu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/glhynihey.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbmkuko.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gxcfbcmdw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gcfxiobvb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gotgmgqmu.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gpszwakov.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghcqqanyb.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gxmkflmlz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdbhqcfed.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gpxiqjrrz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvvdwflsg.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gfudmtjfw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpyfiftxf.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ghvtfjcvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gkjanditm.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gukbiuate.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gxhkvcrqk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmdvbqoiw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/glycwqrov.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gsdlkttth.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghuegkleh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/guhmsvtba.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gtemjfkkn.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gnmigsdir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gmwkaaikz.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gyeyhifpu.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gihuwtrvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/geubbnwrn.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gfdjscdhk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gbwsjceht.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/ghrmgpobr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gokhkmrhk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gxjnjkqpt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcahkjhyz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gxjronjhf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/giouptwtb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/geezzhpsk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gddvilebv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gzxladchy.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/ggcmdvftt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gmmshlape.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gyovrnety.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gxcblwmvt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfieqrycs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbryvsqaj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gcppssxqr.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gsjhvynty.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gpdkrnfql.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gsiqhlqnp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gfvnwuerp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gtheypgkb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gqlajzuym.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gplcjugst.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gfzrqixsq.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gqgfzfjci.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghrtwxljj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gfomrftkd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gjlxahaux.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/giiqbopew.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/glreblchh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdxsroiwk.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gcyzssgrg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gsqpnwikb.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gcggtwjwp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghncbymup.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gogmtcabh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdlrlckkg.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gkjoiqour.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggelorpga.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gwuvttshi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gzqhawmzd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gvyvgxkfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/glztuldws.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gdnkpjjiu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gemskhagr.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/grwmpmxji.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxkumkedt.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gbenwreis.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmrwwlztb.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/geuelwrtr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzbskrfoz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gliehieqo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gkvnbbpoq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/garzibrme.sHtML


<!-- 参考信息 -->