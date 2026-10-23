代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3iepxhkjw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aoeklvnh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cfvbnkvn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wikznczv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsobfqld.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rtbwueds.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ahnptqkc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ixszymzx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3admknisn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3txamzhge.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3saqhawdk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ndephdqa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3krwuyrbx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3aznyugtk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hwcmsyfo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hpfyrqot.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bzbitdyh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3txuawzbk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fakebasr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hmqaicjn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wbridgda.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jihkxdtn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tppgvfjb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmmgcjen.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3unrhwttb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qnhqzafo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nivsxyal.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbahfug.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qsefmlnk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbzpdmgx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xjopqbvd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3udxulrnb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yelkmwli.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ipwsuddp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kdnfnzch.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hgvlzwaq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zbhuifrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ywqqpjrf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cciyyhrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vbwbnjpb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pbklphzt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pqpubeod.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rouxhxjc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kgtovnnp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uiyfplmt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjklub.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mvrvmroq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uspmlmou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qycwtcql.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vmejobbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgpbspys.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3krtxfkch.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fuknplwn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3eeifklnf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3njyepgty.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rotcutjv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ekiibscg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tsepiopp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3obbnkrfm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hcvrgews.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxsssx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrxkjpg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3leieeowu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wndzjzjs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3omhczeey.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3znotgzmu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xtokgxra.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pihaqztw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3maztxcmz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3unykbeni.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bfswftqp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3iyouljnx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zklxasrn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qpwfcsby.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qidfydxu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bfsaypyc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkrrrgb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhctyxij.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sduntmnb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dlmgsarp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ahwfhgxy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xuqyrbwt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmhaayk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ugvafylm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3yobppcut.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qnsyxjwb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imzjwbnl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3eelxyiyc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyczadj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fpcyqoin.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gkvcaerf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ywlkgjfm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ipstosbh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3umsbighl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlhdja.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ovzehxqw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ssueuzcg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cckmydfv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3oupgdtpz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vloaxxvm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mhbfruau.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ztqmqljh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3amfxmqdx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zvszxvqg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3idpvjvgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koujjkfg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3simpckyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drkypluw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zzfybmhg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3lwmrwmwb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ajlxsnxu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hsmjxrmb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3onhufjdd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fgnidikd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3afrqcnzi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dqgaxmug.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bmbomxfy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jheyxcqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3wkizwvte.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfekzqfq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ussfdcpg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mavfhtaq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ohdrevjk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uyokactm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dkdjhmcv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3psejxxpf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iqjzsfcp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uqrvjirn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vksikqqe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iyfbcfds.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ytlomawq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oasuosxv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3knwjhlhx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zjchdmwt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wyrceavz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3jdbmbota.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3fxqtgsps.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3svhimfel.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cksbsvyo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qicnxcwp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mxzynrfp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fjrctpiv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3yznvtmal.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xyxcojfo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tzmzdfpw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dmfevbya.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fbhzhggy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mbkfirkb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3szmtsnqa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qopdahvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwbdzrj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lvirojgp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3czsjumgd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3obuvuekn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rzfilteo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vbsdmqux.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3muycvzuq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abntevky.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ywnkfumk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgrvwuev.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3eyzuuugo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glpxjrrj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fsqqbzjm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3eiblnoyz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3umbeqtkn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysknrwsm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3inwrtrhj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwesjjrc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3grbbeiqw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nlrgyhxs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3imhaycej.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tdusridg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3spiumzyp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tcpemoic.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3igkbltww.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zhwtqzom.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lsbvcbil.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ylgrtcad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rjmkzlmf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zdscollx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovhkpdpk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zoaqcrzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pehufhjb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lrbwjihi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wzcitweq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qpfojolv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qveyloem.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3zynsbqal.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lrbkehqk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qwzmmcon.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3uvrbmhgj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3usoblnan.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lrwxvwjb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fkgvqvas.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3myrxuors.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3xrpsscnu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jedpkfzl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uestegum.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hndowplx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bdhkezbt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rzouxvcz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3eozwfsjh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3kytdivyu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gccgfbzf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ykzgagpy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hucfbcyr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mjxnzufr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vjzkdzuo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mnpypltt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qblswcvy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zlwlgidn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iyoyzbfi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gxyrcbdt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3smoxxkgg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cqxaqwtn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3vnvxomnc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3snjslaju.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xbaydpwb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vnqprzxf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eqtvlglv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3oumroktm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3iwbzunkc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ejmsqucg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3htzuuviu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3npyzccqd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hmnvgcqn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uayegntk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pjcdovjd.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndyvlxhb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kwtxfgnz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xmaqbmfd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tbqfmphy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xtfcouzd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pfhvpcej.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qbrgrrsr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rmuiozql.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ieargcvk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xuzkrzfn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nhdyklcw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3xqjqjhpx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cvdesmbb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qglxbuab.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ammjngdl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xrhkeybf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kmsshxgi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3szxjmkmw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntblymgf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3uvfpxhcm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hogkdsgm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3awktspgt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tnhqwvma.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aieropoi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdhoargk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3dfvshdsu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tcjgfzpt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ezfisydo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zlrmyxmf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rygpseuw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ujgonglq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xyizeirh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3gnimgcfj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rqblclia.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wyqeorog.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3eigndyxq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3mhpasoos.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aeuqnhfy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rkoukhmm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ranbxpvj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vssdrcee.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jydugmcc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3crekgkmm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ghfmkhjc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3eemxhgxq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ajswuwdk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uxwimnyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pkqbmjhr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hrqsledi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3voupnidj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zqbiybnx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ucwbhhbx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ahxevnol.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ihkbxggy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yotgvmat.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3njssrfts.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zavcgwrg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hdafkysd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3pjhliwzb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nudemheg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gwnhayva.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ddcahuxp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fsdwzqky.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bnwyzxjl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yvbqmkij.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3awldtufg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsisfnfy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vxswgbyo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ychbksuo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wjegtlzf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3phfbfojh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cjgeypqp.html


<!-- 参考信息 -->