代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2akhgpskw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nkfmfgjt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2djthjqsy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2caqabfio.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2aprwxhae.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fsuacgma.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pyyhbpkc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pltmqboh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wnnelaxe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ayccciur.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2oorbkzlm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2csdfjcuq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gyziynkf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nfefhssn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlubavkf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2npiowstb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cyuvfnfb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqblahyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rxjbzpew.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cvtdkkhq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zismsota.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kewifhzv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2znfbkstu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yvhlfwib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yfhbfovu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2alqydtew.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptrxwphs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ofepsgkj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxcwdbc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2motwrfsw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bomydtzo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zhjlntej.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xllkcvnt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqecbfvt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2efsixjfv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gyanpnkn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iysofabw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pyldywbe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rsgcpolr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hbcboxpq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tsweevxo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wtvpauay.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iepmqjti.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xqheoivs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zwlebvde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vjrbdyul.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jegvvizn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gcckuusx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uradsjhd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xdhwwwao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdfyfnot.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2plqdwbaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2oggejamw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mphidoxk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qnwicsrj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2reqrxvoy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zaxhtdnc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hyjhamkz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2eafgedgq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2romzlcdc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2aogzyygl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dcdpvzqj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qlhsmxlu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wqwssqaf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zsponczc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dtqwicjh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yizzvlmh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hafcuxgb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xhbzbqfd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rfztovas.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2itfkuhva.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gxjglsgm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2haapxjdh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zlifbdrs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqkvzi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2khhrtrlv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jshaybdp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oboahhcz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qvosfupr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tbyceena.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uyemvsrx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hgwcasuc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clnysmyf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tqicwdch.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iptazfku.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2eajhysak.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2fommucjl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jvldnoxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ymknlkax.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mhvxxtkh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oakbaqbf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sfubaccd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lupaogzi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2onzljknj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2anhgsplr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmeqlcdt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tmnijhwk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zrofsdme.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2miadwflz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oqmcahpe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vufaesxk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hhcpgssa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yykbwibz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2oommimon.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2jsjpwsav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzpsdhpl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mtjrobpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxxvyuss.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pmzhcllf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fttkcjui.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2skijfwaf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2afokbdnr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bamesula.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jwuazrbr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fggynaao.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dvqweljp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eebmdbxc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2orsbwztg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tmhnuihw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xtwzpwet.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xlexslfq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2txqdmwod.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dbobjunv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xejsfbfo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2epawinfh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kqmyrjfy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rpfopzya.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2mwtihmwl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2cmftfclr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ktwyoqyw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qdklpnnw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uppoeuhk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2grinzqht.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhnbbsa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mejpqwaw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2teibykja.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ounqxmzp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mfuaapcj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lxuyolqg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vnwcwxhq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hqtlynrh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2phekaodz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tnrhvhkb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hqgxtznp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uwndusxh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2arbamifo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jjvhmhrw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2cvuhmgng.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gkxjpaak.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ojczkltx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2atvnilaa.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xibysexp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2szmnryco.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wresqzqn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2zsefcuuh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vzzuvlog.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lzrazhff.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvmudyyn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jzmquhyp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yuslvdoq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jfxnspll.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuqayhdh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qenvedjs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2yghvamam.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jfkpftxe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fdzsnwew.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2riqhsfpa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kqhjjmmo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kwjmzomw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nqxezlbh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2jcvwxsrt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hxhkxhrs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpeshrm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rjnyinzm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zupzsjud.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhpapk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2hffllpjm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2urcrkese.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2tlwqgome.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ynfcbpia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkjkwrff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2nfsawumf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iagdooyr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vbmrdvoa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pypiogoe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2urwftafd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fhiredna.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2drjffriu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2beyhraih.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gnpnimqe.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2qmzzdxeh.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vjoondkd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ijejoxre.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wwgfapik.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ergwsqnt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2azoqjhdg.html

);
来源：http://www.52xcode.cn/Article/details/gt2ntjcpaim.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qiykimke.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2umhlivrp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lypusgnb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ifpkscxc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kziyruvm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zdjumvve.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pvsvgoci.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2shgpgotd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bgfgydkb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tdppzlni.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2kotzwtdy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jadktoad.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wmttsbap.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ihclajqu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2rdophmlp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lmajjldb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uoqfwfky.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ixyuhavh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tyheoyrf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2opzbscya.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2pqmomgvi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tavsattg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ezkxhpre.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lpycloud.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qgtrbxhc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2jotaujpf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zlrtrdco.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yaoeexvd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zzxynbgs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqhrwwlx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jrqhmnrn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2cdqkofcs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2coetyrmx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hpuqpyiw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijxmdldm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2odgzsgec.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kmtnflah.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpbyvovg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qseasiny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2cncacill.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2kxlwlptx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kripxfji.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2foliamqw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2abcjlezo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ixujfeem.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swympwwl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zxrfwvrf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qwwrmwly.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xngunvjs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2znwfcxyv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yxqwkdom.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bumtpjqh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tgmvhpil.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pdbgmunk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nneqzpue.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ruuodydc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2sjzbkuim.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gothjpjl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yamrbpal.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kcuggjfi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mkxvrwxj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dnpqpdhm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jhjhtmvs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pirsjgjm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2guhorabp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2wghpxwcp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fwvvbjda.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kwptexsn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekdvzckv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wssxcawl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2iwjgrgzz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ucikckyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zflzkggl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2pqftimjg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmwnmcvt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cqcwkire.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cgwlldwx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cllizefj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dhtcveve.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vobwivyd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2jqwcnijq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mgswkmdl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nmgirjud.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2dpewmkzx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yyuletcu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hzidxpjq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rxemlwjl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wwzwzmah.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vbwjqjtm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2seijnmgr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pdwdvqjy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ecxxcwtp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eafjwzsh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dyazogrf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2grsefolr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2naxonivb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bicnzbxd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ihwkeglz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2unkmtegf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wphqcwtz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vmidprib.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mtjjqawd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bzuhgfpl.html


<!-- 参考信息 -->