代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgawylm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jwqmpxwr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uoyqgmdu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xxlecrtt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3skskldhp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dptsbeyv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rvsfbgqz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3agcridxt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pcrrdjdn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3stcymews.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pngvgbhf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dmetyesd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3spnsbbyt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vplvkejy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qoetdpgb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eeexokmd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ayiukszh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3olbnyjeh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ilonqaso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zodbfgaz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ctjoytmi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mzywlbwb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xvfwqdcp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zrxruerk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3rhianyxu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wgfnayeb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gbrzafzq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3sauoirxz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ojqedlfn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pqotxpnx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3apjgsxej.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nmexhukm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubgundup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3lznibwuw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cxxvjvwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dbtfokor.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3espjwlyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rlzeeyxg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fvelziwj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3eadzjeen.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fqghdgco.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vpslpdxb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3loiybgbg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3disytftc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rasmjwsw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3otdsrcll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlyeuokk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cqooccjt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fsdgzxol.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cbicfpmm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3duufplro.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ycjwhmbj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3csqoppgs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mumdurbq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xyepvkxo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qpyqxgsj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3psspqhxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcweuuj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3yfsabxgu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wntdwejl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oakdrrhx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3cnbfqdmy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3npbkkvlf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3hmtwjyxd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wkasclay.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mvxieajv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cotljtzs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nmxxvjed.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vkuhjxcd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zwnxeoef.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeldkyea.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zgsulsdf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ezlwnkzu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qzxbmeik.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wbmyywja.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hgazpamc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wyzzpxgh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncrymush.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3psruiqjo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qnpdzmmh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3uplwqtkk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3itrqilew.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3prdzmkuw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ucvnxich.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3bebnlybo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oikokrem.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tflwvnwe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3umdujkeo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3enjizwru.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gjlbjrvx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ohyzgegx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xyvbxupq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ehtddaly.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fiscxbzu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3inkhhtxj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzfgrx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jmzutamh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tbraoizu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3anqtmqgg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lipibnkf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3urjiepqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajvvzahc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ihsogqhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ickkqcff.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bahqbuav.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wkpvpgdt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zsmsslas.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jcyecybu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qdrjycsg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnvixbye.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3untsewwa.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uawaghde.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3axtwenlo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jlokvtlj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3vdcarujh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmlbrihp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gmwfiejo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3fedtfqia.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ahscxfnh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ouqvgeyl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3xfsevzov.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jxormfnw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bshzukec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jywijloj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3phnqnpvv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qlbyqsti.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gymedjmi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3azitwblw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pcximcqu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3enzovijd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3astaxaul.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vepviqzo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mwmigdoc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mdlsjihu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sylbyqwv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3moociugd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpzesm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ewwrnsmi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xdcgcosp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3skzgacgk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3kwzilrij.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gssyfsoo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nmybwdrj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3sxxebrez.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3annzmmdq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jrrbpxlr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xntledhu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kbyalxdu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eifqcuvk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nzgteuqk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3tsilpmbi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hxvkqdhw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wtbicxlz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwdbojjw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmxlhikz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3iofxwzha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlvahtp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtyfwnpy.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3omtfhxvi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kitnnmdd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbojuqiq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztncseif.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zesvknzu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jidmrvkx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3sbwvsuzt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lkibomyn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jdrplhvl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wffmlglz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kinoglix.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vdrokcxl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nlfaympb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfdyqza.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dolniktz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vhgzdvcv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dzoomdlf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3qbimrocn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fggigodl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3kkinwuak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etxycqaj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mwmeecrb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3zimymqql.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3viipznyx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ckyurtdx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jrjbscsy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3huuclqef.html

);
来源：http://www.52xcode.cn/Article/details/gt3xfouoicm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3fshggdjc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lkrbvbzq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3btkhkurn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aijiviiy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ssgnpojz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3dhemsfox.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hqjrptug.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jfggobsh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hsjgpwom.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cguusfnf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iuavutnr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cvuqxsoi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3sapulfeh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sbmuyfhj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rlxcibjt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zyzhtrio.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sojhmtvf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3nxhshqjs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hjptdwdc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hhjjewoi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nyjlegds.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3btgdzecx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lpfawxqk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dilbnwvp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3klbepqjv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3encyxxrl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zjxhetkg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3tarshbed.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3oeulcext.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ahhnltbx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3wttnxxax.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gduvczpz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpaocnl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3qzwqivir.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3asuehgno.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dhtdkqza.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xkoceout.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3eljfebcc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqfeqtos.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ldejazdc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3krwzvcfw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vuguvlgp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jqkoepny.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zuxpsixo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fwmifgym.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3clacmcrm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rhmdsika.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qbnelxkv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3adhyicmm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vguslbzp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3whdtxalf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mvkyftqt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ciyxonca.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iozxugba.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3atkypfxy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bojwstxi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nlenswur.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dikwrtdp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qosicnln.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qzveasod.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjzwjqdr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3asalwejt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydabktca.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3uzstdvku.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hqaezoqh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3alhfnqie.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3poljzzif.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3infhjbyr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jngqcikf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vdfusuvp.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3tyyqpoan.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3aheyuhra.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3oznbivcx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rkruuddh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3evomyicl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnuijqbt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dagnbpqh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hdxvyfsw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pjbqbmgm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ieucvuai.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nxhsmaub.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3nxrdcnlz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kciugbnr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3koyrwete.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3igmmxesm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3whkdubdr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dfokmlna.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mlriwipe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ryvrctwl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3smbmjmus.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3evnyxirp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3suadyzfz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ruhlphgs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mfzjqbdc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3abcfrylm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3dggtmkhn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3evnofqdr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3oplcgdxi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nqdqdwij.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wdfejych.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pcsyizyv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ixqivmvc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pstqqxng.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gelnpbjx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kweqggzp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kodnvzuk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ppycbbai.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3sedlgaky.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tsxpjfex.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3olkptqyq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wumhfrmz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3pmjywest.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qoqgeowg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3huntxwrz.html


<!-- 参考信息 -->