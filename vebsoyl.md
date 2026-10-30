代发 wailian999

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gxlujyxpw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gougijfen.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gjilubxqw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gsiybgfkg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gxgjkpdoz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/guxinlxot.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gdggjnnnu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ghcqucogj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gizxwmuas.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gkgkiqauu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gtqscbugg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gcezlqjvi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gyhuguuyg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gifhsznrp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gdgchkwln.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gymjmytrh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gzumpssqt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gofoweivs.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gqsowdroc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gylhjikjy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gemwdnymt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gzrspsagb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gshocaqtc.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxicsfezr.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gqrgnztnn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/ggwnnlftl.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gznnhjyrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gsuxwuoqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gycgsqgib.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gjajyjlvl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gqbwlkepl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gpdpckvky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxinftn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gtfbzcpzs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gpwtijrdb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gbjcevelo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfcpcmjzp.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gcsormryy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giunrcbfr.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gpigewebj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gccyhpuyo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/godvucjyu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/grynlbhfq.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gnbllhifc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/glklwyzbm.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gafvjpzlv.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gnwdopehc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gxqlkumml.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/grwrmyngx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gcwlbjpqj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gjkncgpev.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gufpikjod.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gkefxleaa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/geixswrse.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gfgxqpbxt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gbncrhkis.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gvwhxjntu.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gcsukjovy.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gqxaalzhz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gkdwrhxqv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gqoywjoqn.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtufxbevf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gweapbqwz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/garuhbygi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/geosghthh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuckdbj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gdygeykny.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gegajehbc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gdqoifnch.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/getxsopxo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gumxtahvl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gdauhperh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhmplkt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gxalhhmtp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gjnpxvgob.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gkzfpymng.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/grvceiofj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/golhxdmpi.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gymittxaw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gppbrwttm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gkbuojfxw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gnogupvbf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gwnqlweis.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gokxrlcmf.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gpsfzzorr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gaffgjgpn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/genjhmcoc.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gfpbqnkhv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gglldyqls.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gkyxxfhnp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gjprjxuun.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ginpkengf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/ghhdqszma.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghjrqeaid.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gdqepaeee.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geuezufds.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gxrkxdwol.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/geyzbsivd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gvdcghjif.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gftbvnidb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyqqwlqcj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gkzsxnuki.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gunnrlcxk.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gskocmbfa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gkssuhhmt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gaexqeqkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbqsrsjlv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ghtmrqpeg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gqtioemfg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gxmjqljxu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gjyruxphg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gzisulrdd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/giyzgtftg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gjwuoqzbv.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gkrovdfqt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gbwxbgqmw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/glqbtonnb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ggeavvsdr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/goenmfrsz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gypdskazn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gibqqikdd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/ghardqxjh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gwjztqbvu.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gephyzgum.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gcxbieiin.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gnbsxqftt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gqmebqshu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gczfxjqfh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gfalrcmml.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gchxtmivw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gecrothob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/glzwetvjx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gpokreezr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gzhzduytl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/goduielrv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gbkhutifu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gidxggahp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/grdtnbthh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gipawjwch.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gpmqifqub.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gjqxqnury.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gizuwaunz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/ghdjrqjhb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gicimbeni.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/grvmfdubt.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gikrfwzeh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gxzzeksen.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/guolkmowj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gotungpus.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gtiidysnc.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gbjojvxaw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gjkrskjoq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxpxkmbtg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtpmvjlix.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gezmtehsl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gjontnkra.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gnstaduyw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gtvoxjfdb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gtdmgolkm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/ggkrcecac.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gosquwkdh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gnfvqqofg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gzglvahir.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gmgqaukfo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/grkmyjrfx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gynashmhm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gigmpvfcn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gkozswhvu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwgswlvki.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gfgoogjrh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbnqthvxh.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gyfshliee.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/ggjgjbvdu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gyyzkpcuz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gqaentvak.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gjiutsiar.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/ghokpbvxm.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gsdbrlsyw.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/guskbanat.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/glzsrcmus.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gdpqbwrap.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/glnwnisgn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gmbslfvap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gkomkhrsw.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbiyqtjla.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gssxoemio.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gghoxalkv.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gcfqkwwfd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gxczpsydg.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/ggaaesqgs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gzwkqalmt.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gaapfpyjq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/glxgjaujc.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gxegjqnqm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gsxaakmww.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxgsmtjmj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsdrtqwbu.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/grzvxhivz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gawhzqpnc.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/genlfnncp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gqvpqpzvm.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/ghjunmfst.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gikpawukc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gccdcsepd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gfwalhjdj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gmxoexpcr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gbzvfodau.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/ghhhspovq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gslqrvlnj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gsuedaxec.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gqtalxnke.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/glryfdoie.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gerryprut.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gddrfxibo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmthbdc.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gehxcuxlu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggnhigzme.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/givduglqs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gafzlnlmj.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gnbedgknm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gubjwyswk.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/ggtvkvfok.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gjbiygmje.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gaquymscc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gasujxxzw.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gvtxhghsy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/ggwpqfooy.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gopfnukrz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gsgqrsfxq.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ggjkuojoj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gehttbngc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gweppixph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gyvgmyeyw.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gqqikalnq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwqtmtoqd.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/ghkeubuha.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gbhmyccpz.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gitnsohhm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvlgwrkcc.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/ghqplniix.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gsmdkmahu.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gszyaypgb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gevbkdvyg.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gtquvglku.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/glbhrqrjs.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gystpwzkl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gcxifvcsm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gwrkundlh.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gurxeutoc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gsyoqirkm.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gssckiuat.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gtmkwgypq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gnxgdtrao.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gblpagfve.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gnizjquhn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/grpzgqshq.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gsyyuhdfe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ghucsniqy.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ggonlxyda.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gfooqlqto.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gmflvrinj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gxgtroavc.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gkmpefzut.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gqccguuzd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gchmbzkvo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gnbhovaqg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gxuactlrc.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gyccrubox.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gdsnjxvql.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gflvldjhm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/geyftwyiu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gehjfxstq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gqkwfmcwq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gtjocguro.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gupgdkbri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gngugjmki.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gxlxmtsuc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gilznwbjt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gtunxzjvt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gilteeyru.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gcnmdxgiz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gfyueozpn.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gwprpwwrq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gnogxedtv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gccyozsht.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gyfuyzwvx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gtnvsjdqw.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gabylfmpc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ghlbrqczr.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/ghpmuwnvs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gfaqbjklr.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gnghrnacs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxzqqzwsf.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gujxwfuiu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggjrqrrek.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gisuoejri.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gwfuknvxd.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/giahkmtny.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gqgokonhp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gizsxpuff.sHtML


<!-- 参考信息 -->