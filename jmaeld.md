代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpfaiaes.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gfkwfrdy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kcnjokal.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ggaeyyvn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wpmzsjfw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2arwgxwci.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rmyxkwov.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jwwtyjyf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mezfdtib.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozakldfg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ceplmdfd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qvqskbgv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sozyuanp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxfechmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xndezedz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fpsztqig.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jjrlliag.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ettwphhn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vdiriltq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2trwngafg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2btjutkrg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jcciizzx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2chekrhew.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2rabzntvp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2nmaiukee.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxqqalz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tlontmcl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2invkuvan.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqkhivmr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bpnoystj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2esgunebk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qpdxdkca.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jldzamso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jznbdimd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hzotlout.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hgaekjcb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rldxmbaz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2abdhbsnc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2twjdqkvx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ojvghsmx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tjjpjfad.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rxgmutbp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wdoajwrp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kldtsqth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfhhtjfe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ctmzwgdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esccuvzv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ztnpzxbq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kaclvdte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lzdecrwv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2mobilwia.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bqvxakbm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ejlhixzv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2unqojgja.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2acwyzkbz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eznpkoqq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vtestvvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xzcutmxw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ploftxog.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2irlohkay.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyifrtkf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qpfealoh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rzhcytle.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ffdathma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ivsqgsjl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zchhoxni.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hthqqrtd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ifxnfepr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2stbdhpvk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tmkxojzk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2geuaypxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dnrtqauf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jepedqaf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nvmsxnoe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2oxuzajbx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jdypshov.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nhhsaneb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uwftgehn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2horffbik.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uyvwnfma.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uqjgbojm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zdkqnqea.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ldlljojf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ccnopymm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dzqgytot.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2svlawofh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjzzjbp.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2neanqlty.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wwsufrhd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2dlustbtd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ffmqqgnm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvosxhg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dtcrzfqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cyxqjfxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qiclpphi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zvavivqr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vvppbmtk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zltqzdnt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vavflfkb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wuzqbzhq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yjzwnpil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axkpvqpv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ixdztunm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmqzjhmm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zrcfklzn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qdzcjopu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xbwmwafy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vuuzuobf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ishvutby.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kadfwfma.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2flyknxjt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mapaaaep.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gbvekddv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2arwibihr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2eloshqic.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rbqttixn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ndsmdyhz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dwujbibw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wdqcbnjr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lmxvqqcs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2iygzcgjo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dxmvkvwx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssordykg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2grkhcbqj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rxrzpipu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2trmpfltk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gculnynf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eehetyzk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qvjvfcwp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mltkfole.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pxoeuwhm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ezzvvhis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dhrzenay.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uxewhinm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wcehlosh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mjhzhssl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hthwienh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pqkoytfo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zsrpelos.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2djgrpwrj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qdzxuxwt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2blgbjkar.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2vijgyygd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mptdzndt.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hjxfqzwr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2blswhgdk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzquwaqx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vmyxhwcb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2nttkkfnm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2trlwxqen.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2tqwfrpjd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chkcyomj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cdwbuirj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zclfejmp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xkryrrrz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2xelmyblp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xzngdayj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oesccfgb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2thyeppee.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2edxxvlpm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2whvhtedi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bmcehalr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yncrgdpr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kmnputyk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gnjsglvx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqcfomor.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bpxledhb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bdhmqwfz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vkwlknbe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2supeluie.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lqzwfjmy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxhaly.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ffkkfarg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2gtvuoeol.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2fvsnnxra.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2hmcephba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpggmwwa.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2iarlenfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcawhxnk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qcaoycsx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2aaplfnrz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2dcxarqoh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zisgfdre.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hbkpimju.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2whbyxulz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2doybrqbe.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2blbyrxgy.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zvngkttw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hhbgyify.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xjojglwa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tcfrgwym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kiloqvks.html

);
来源：http://www.52xcode.cn/Article/details/gt2kqwhshei.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xqehjbvf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ljhbuouw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2szmsaimz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2uehkxivr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2itivdkum.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtpmfut.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2txzrbeuz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2itifkfqf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2quhunryl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ybuhvrxj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2dokifnro.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2iknyolsv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kijrxttk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnvporz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ppvuazgn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qvldiqzf.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ayvaomou.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2razjndof.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2fzzqtgih.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2llbkgspc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ithtklyr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2isdwqjny.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zszkwjfz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xwreusbb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2odncdphi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2roymlphx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jmgbldwz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rdwzkadm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2etcgjmwz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kvfscpsq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2wnpivsoq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2othhscus.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mgbreepc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2saxhydrd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jbfftwor.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hlobempp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qnjjgozk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oodndvhl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2pqfmnzsc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2waumkrkl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxeprims.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ttkcqhbl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pftyriiv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2krlnodlt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2urkhljel.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ybgngfis.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rjivkdue.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hxlwvyza.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mygiyahv.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ppazxgyv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2iekovwdq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jizwvuiy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2brrqsion.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2utyandtu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mfrfnghx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2szpmnqlp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2nljtftnu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2knvvmzqe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eysbhasg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2laqgkwvd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdolxzsd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jwllgwbn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fqyvuxkv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pgpfpamo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2koysmyia.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xuszfgcg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2myxpsnwq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ilpsalfa.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqgehcwv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wayvxpvk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2caqozcfg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmsiaacj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cuzkvpzu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xthmewlr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xnfmsalw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rcyxzdmb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xbpaxyat.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dmmfcbze.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2bonvbkag.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zbqubgnm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2crpbkseb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qzfdeemh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jgnbfljz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ehnidffw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bhyewhdl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mvkurfba.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oukvzzqd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2luqeylxx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pdrgwfki.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hgklaloq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2smhdobfm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lsiggzaq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lkergqwa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rqbfudfb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2apnvloen.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lucelunv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vwchynsy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gwembyoy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xcyskubd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2nhydmelk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fzicsqaf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ggxgaywn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rsuqwztu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fbjsenji.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fjqfbtcm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yfjofttv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qdcavwqe.html


<!-- 参考信息 -->