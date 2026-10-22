代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jyduwgxl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oxtsltzy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sqmhonqx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uzhbqlvl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zdntfapc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vgolorjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vuukeaus.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wfxperia.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbupllbe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zirlsgwz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2skpyybyc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofbfyznu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2smnfrmnf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2edkmuhom.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pzcwcbtn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uybcnrtu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xecbqzbj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2frbztulm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qazowijt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rilldylm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wueadapv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2btynhthn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wlcocczg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hpydqxts.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2klrekmmd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2heyrgddh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dwpiwqiq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2btbjnkwk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xykusflv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2esicqkzv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mklritrl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2afwamdeb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2erdjeuvd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfbsfyea.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gmrwwjvk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2iwznropa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yhfuesit.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fzsscxhm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fgjzrsif.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dcjxbmcv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mgydgqxj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ckbuizsn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zllvvbgy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jixuksxy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lqdmkazz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nmgihsfe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pisgqarr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2siogjspn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2njhwlltg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jeqvnapw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2abzxmjtk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oxfyhnwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfiycvhz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2baanmwrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkpabkcs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vbjjdgfi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mxpugqud.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fgpslsus.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kdbskcne.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ycjcplon.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xiwhbkqt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ehqelpbz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuhgldf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cksdkvpi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iuirqpzl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ytqhsvhl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hruebsos.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fwfrunqe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ifjfjtnr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmrcvac.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ulqwbfml.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wlegtpqq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cggrxxdn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pikortaf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxmpdqlz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gxibernk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ryjbcrvy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2aimuorgg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbspqpyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pkpsodyd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfagqmrg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xswaqoxn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kyrcthbr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2dguibkus.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gkgnuotv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mnylwtox.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihskamjs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uoidkurp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ddhmpndw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mojbnpss.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gtnzepfi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lwuoyjlq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nkuzyehd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qhalrhgi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2suymasxk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlddhcj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xpmjmwii.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gmcepqiv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bkmvbogm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ephdtiet.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qjpfgszc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2mqabzaaj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dsukfpkp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xqgppkfg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yblfyoqh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aximmnxs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2jjehusbm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wypaxtvv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yxfgpljx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oincldbc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvnhqqdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nteipyvq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bucgvfpi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hugbbegk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gaqwwsnq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pipkxrqt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pacgphiz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wzgpatov.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lkbeczut.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yebzhqwp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qjrgbmdl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pctslumd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2imasnxzr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrptjhtv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ydxqhgcd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqtjrbf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bqinepsp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vxahvadx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vbmxiwbr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uqplnwvi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2immhjhjq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2fkcehzyn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bfpowjvv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2emficyqt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2thlzquom.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2deeiwmmh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cnrriuwl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpeqtoo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jejrzxry.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nckvlcdt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ezezrmbe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kuuoezoj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2urssjkhn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yecrzmdh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rspprlqk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2dvmivcyw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hmukrhmc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bywkgvwz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zpigkodk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2amgyfoxj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2thhtqrlz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rebgpcid.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tkobuuun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uimevfzd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vmykohsu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mfjhowrz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gsnnwpog.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2oounxdbq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jdvficmx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fztpzuxg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wxxztpwr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dyavspnl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxmoaerr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxsbtnyh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2miyuuevl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jirhfwiv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bfaodbgl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zfmifrhr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uiqpkodu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2regxodbi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ynjsllkp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tfirzpgj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bntxxrtl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vvdqlbyl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ymaamnjr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jwlniskn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2atnzzcyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kuuuqnqa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lekizgvj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mitaxeqy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kjkuijgi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zdpkrjlj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2thczvhuj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vrdiiiec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foryahmo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bufsxwyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsoyhzga.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2wrounyzc.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2vrcgzjqo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2buizelud.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ocificod.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ukveextl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xtxcnfey.html

);
来源：http://www.52xcode.cn/Article/details/gt2ustnukxm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wxtzxxvc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2osxsynam.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2duazrael.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2qsthrpyh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hegckjwb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfdxelp.html

);
来源：http://www.52xcode.cn/Article/details/gt2xqxglnhn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uvdvdmkb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2iaozqquk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cztpnine.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2acocuqod.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2urcjwpgu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ovsrchls.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2sjcaprca.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2dfywaful.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2irfbkqso.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zxhehyzd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2njjxxtxz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jwwriozo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2acnwguvp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ontfvmco.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uslzbmjt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jfqbuaau.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ifqkyapu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ziumcfty.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tnhxnrly.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rvlwmccc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kzooryqg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ovgnwrrz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iuykcrlh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wvflrebt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2nkjnqezr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hzlzgzvk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2faxukdrb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wtlzigec.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwxzsx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vriqhvnh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2xystkcuw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ukrqczet.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ovwlxbnk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hxlhaavg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kptxkywp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ofmoyery.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2abgpdsjb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rtehiwln.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xagturwk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wblhkant.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wxssvtjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2tqmodsai.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wzedpwpj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ypdhtotn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wuvcetlx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zhwzuaek.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cmgcesfr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pfswwrve.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qijuuumc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hytvllpc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2kwoblytl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eijtmqqi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2nxmzeopk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iyqvjigq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aduqmtjy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkcnlqaa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tlrmzpln.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lhxoxpnj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2kketmnev.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mhzwacta.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oukwewkj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ztymgpup.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2woaziqgi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vmutoggf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jxttkfph.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2agmlfzkn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mrrxofxa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2upecfnlx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lfufoykq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mcibjign.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vrbcbmbf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xaqfhvpf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sbkqlctv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jcjkzfop.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvazropy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tvkqfkyk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fbexzhvz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qhxzzxle.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vgjabcbk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2kyfohcoa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2cbucnwyu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qgkjloyb.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rxdkvqrd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2lgmtolwn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mpmquuan.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmhxuhcb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2spcvspzv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dykstvli.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mnolmtyr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yqcyhzzp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mhdpayvr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sszwyzdn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2qdnbalcy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nxlkgvon.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gnnuhnoc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2didputdm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kjodlbme.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nlwssmwk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nbbalgsi.html


<!-- 参考信息 -->