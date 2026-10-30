代发 wailian999

[N09] 栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiyhkvve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblbwmtay.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gzozfolyy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnbjfxlr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhpycpkw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gpuniarao.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfelrck.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwhuulot.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gdobzmnfc.sHtML

[N10] 链表节点定义
来源：http://baike.fanxiaobao.xyz/Article/details/gctrhkmam.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fanxiaobao.xyz/Article/details/gercktslz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuksjdaj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/grdqjzfei.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gxslubxoi.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdtxanek.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjwlvgcd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcqxtnjc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaulkkovw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeplxaxf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduiadxzg.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwtqrnqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgicfavd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gikcmfgpc.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxygelqd.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gnqcqdank.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fanxiaobao.xyz/Article/details/gptwqrfwt.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gsymghijm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fanxiaobao.xyz/Article/details/glqxfdang.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gocanesmx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fanxiaobao.xyz/Article/details/gbexxvxee.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/guujuvuwx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gidrixdzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guukmwnpt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnlcwyqz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtsadjiv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkxoiace.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcljryxrm.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwffszaql.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gylazyagn.sHtML

[O01] 启动一个线程
来源：http://blog.fanxiaobao.xyz/Article/details/gsybhsykl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gygebevjj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwyyixlk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fanxiaobao.xyz/Article/details/gubygrakl.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbmbvoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gxwsgatpm.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxlfqabc.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfplqldo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvxelhys.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gqlisufcj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyblzpeup.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gdkrvopsk.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/giioysrhs.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gibflhugv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gedaoplgz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gcdlnxoxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fanxiaobao.xyz/Article/details/grotgpxza.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxogdghq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/grlcypopx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkluyjgpw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcairkhxa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/guieozmum.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsvevrfn.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gusxzdtbz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjnsazi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdwgleiw.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvnnnwn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ggegevmes.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gkbhbfdag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpjmihnu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiggzmcd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giapcdrfp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gnmnqsued.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fanxiaobao.xyz/Article/details/gtansudza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giludvbxj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcemxbvfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtdhxbvj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspkgfrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fanxiaobao.xyz/Article/details/gmjrwjuky.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjqondqs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/grxaikhfy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqirlzqd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gssewlaju.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/ggznngtdf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixbhsxt.sHtML

[O06] 使用进程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gqztixbfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fanxiaobao.xyz/Article/details/gemcyjljf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvjfwrxk.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gzqvpyzck.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpitbcuav.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/gextbnmul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgajvdyv.sHtML

Ruby: // fork 块
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvpyqahw.sHtML

C#:   Parallel.For
来源：http://baike.fanxiaobao.xyz/Article/details/glyxixmim.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghebnlgmt.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghcnwfpk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gskgzsjhf.sHtML

[P01] 生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gxglpceem.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/gthyyblyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gnsdlvvci.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyinrmwx.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoxmdsdw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gahpwqdbl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjnfhzfz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/gekskreot.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gdoedrfhe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyozraof.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fanxiaobao.xyz/Article/details/golchykqo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/guwmwmmys.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaomxcax.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gcnjvqyxp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzktppf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmncwbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gstnvkpbw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiztvqwr.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfuxstdlb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fanxiaobao.xyz/Article/details/gcdffpeqa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/gtsfzvaam.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gkqecnsif.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guttxzgjz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafvoxqox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goloxksum.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/ghoeasefc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fanxiaobao.xyz/Article/details/grfnxewjj.sHtML

[P04] 求长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvwcavlo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/gqkmzopkm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlhcrxjl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxdekvon.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/gysytefrq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpvzdrmc.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjerckn.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gcekjkalc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsdkxmse.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/geywqkhvj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fanxiaobao.xyz/Article/details/gnjzbnxxl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fanxiaobao.xyz/Article/details/gcdxqptuq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/gtyvrnwgn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjukzsifc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fanxiaobao.xyz/Article/details/gsuadijhe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewyqxyyo.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gkfbrcfqu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvyueoq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgyfubpr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/glgfrgqam.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkprogd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaigsidp.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomrrxokk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfsityyk.sHtML

Go:   if x == nil {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggrftjrzi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucvjnxda.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwlrjfrh.sHtML

[P07] 防抖与节流
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbhohvgq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gtnmquytc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gykrtphbu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gudtvltpb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gnciizpuy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzeiuxioe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlocbvv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gxrojxmle.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsutavhc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvffzkjb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdjodroe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlytlruu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gxjvyhdxf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmqhxyzw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/glxpszmvk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/gyviykwmr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fanxiaobao.xyz/Article/details/gdmjcgawm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatrxdntv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjlodoeou.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fanxiaobao.xyz/Article/details/gtcehdhri.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnztwoa.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gwwklsglw.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gjseumitq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/gihvsebfe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsczqavc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxibgshz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fanxiaobao.xyz/Article/details/gmgjyonjy.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgrihkhc.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gqhznvvme.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfuybcev.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnvwlire.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtvtdur.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkufvhtk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdirzhhj.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqdkqpbm.sHtML

[Q03] 增加列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjvapcxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnnjyfid.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjmivgem.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gawyiwrdf.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gggdfhhvq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhijitlt.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizrjhov.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfkyzbdy.sHtML

[Q07] 删除表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gairmzohe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstdorlay.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdqmhyrf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhvkdaij.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmxjatmtl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/geizavjtc.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/giftpgniv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gunedezgu.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/guqycueev.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/ghqlzgjla.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fanxiaobao.xyz/Article/details/gyknahvbv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gyupxuqnx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gdctxdmyk.sHtML

[Q13] 忽略重复插入
来源：http://3g.fanxiaobao.xyz/Article/details/gwbcxacfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxpcgmfu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhufbnck.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gboydcexv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gtzcirhbb.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gslelzmrk.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjppfnbx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzkbvulz.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gsjhqslun.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvcqixmw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxymohiwk.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gkruzkzwj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqruwmii.sHtML

[Q19] 范围查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gclohpdkx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbwxhmum.sHtML

[Q20] IN 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscxovguz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqsvmvtz.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gscdkuvpd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/gazecbqdt.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcuiiska.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gmmddiweo.sHtML

[Q23] 分页
来源：http://www.share.fanxiaobao.xyz/Article/details/gppzmnrhs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhmhegj.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxjvnyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/geeitkajs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykyvrhmx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gepveorln.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfovlhor.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gecgwlmjb.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpdyxvkt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpulfjvod.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgodhhs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbgjoqfj.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzeuxyhy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhjlcxo.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvxkheto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gyxqxmakq.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtitemzq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdcqlfqcf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grteweivz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwboyjbrl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkwemooe.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gsjrhdcvu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gblrijyfy.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/guotnystf.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoaxynlj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkmpzfa.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqaxmxkc.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gxkmwojao.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojvorxo.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gofdgjmix.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpfmjgpp.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gzliaiqqg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwkfkgs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmznwucd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/glomuliry.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/guuknxecl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gqeykyipq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghviepspe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvltailch.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxipostd.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gawssxwpl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gynoyvkbu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gmfifkxgn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/givcphntp.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gkbgqqiut.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggcoezpd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gryosghtr.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gwisbnnae.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojfrcma.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gygvaksdq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqvmpipb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiuxjhky.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/goxnbzvyk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnjvjnre.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/glapwtpej.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvlbzbfs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwywqzx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtezvwiqq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbcnkbei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gseowjyon.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/glecjtlnc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/goltfdbxd.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/ggifzxxem.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gfxruapcn.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzygkxp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gikgnsccs.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gecfvnekv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqsrgkd.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gvpksyoqo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gkptzaknv.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvupzgcmh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/ganmtghwo.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gjgkdhvqc.sHtML


<!-- 参考信息 -->