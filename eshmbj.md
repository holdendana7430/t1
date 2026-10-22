代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbaoaxkv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rxelmimi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gpgrwjar.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bgtejgki.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ugvwbcwg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yuatylwt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rjlhogue.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stgqeumy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iyodpssw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mmqzcscl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2weycjlbl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xrvuitvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nsmkwhcg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kpbcxjrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lombwzwi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gkyzqxln.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lulwwgba.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fnvatest.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lrscohhg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jwvxjkeq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iluemmip.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2aizjotjs.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zgdleuec.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2tpvzshfy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bpcowrtl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zwdqpswa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2whntqpbe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2iwfeoxve.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmrifmsi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzrqsukj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2swcppbyx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eyekuqap.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2igpobxhg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2azjpbjqb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dxnbjjyh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2glvlbejo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dxmlepgw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2exhcdzdj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yzxocdoo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xhrcwnyv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2osaasnhn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yvuzbjdy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xivnfojt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cptjoyak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2degfkfhv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2oweefovk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdovkyhz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2upbkbots.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dngxogys.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pbnwnqsn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qhpellnq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2krvsiuaq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ibuhosgv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2awynhtrp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yprdsksj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xnvyabjh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iknktqiu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ueepfdtd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nfszvbdh.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mikisagg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zggbuvlq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2czmfkups.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2itnqiyci.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ycrbuvtr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hcstccyf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2smijjfru.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgagbqnw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qbrikwqh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dolnpksc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2niavaymm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwbtshtg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2sivbhjhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2llelitfc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdhkyvp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nxifhlme.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nxqomjhx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2bhfenqzv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xytfojnt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owelokdu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xioerhlu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kbppkvwq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ooxyaspx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmabhdua.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ibxarssw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lyspjmgg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cvlaudbi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2afaudbiq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vtixdiba.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2twfrsbes.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2filgcsiy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bfuhjpzh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gsikdufv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gnjufnej.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ewvkiwmy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2knaadewk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hpmvdvfy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tfjzrvon.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tdhhwcwk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lkkszmbh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2djkspsmz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2eetbsuyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uecdkmvc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zldatsmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozzaihql.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yqyzsowx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2inbgdhgo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sdvgiywh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gjaoospc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sqizmieb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fdqciefv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ofhhvwhx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mikutucn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hyybkzym.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mblmcbvs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vtjijgmo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwlryfht.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbsdfq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zruxdsvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vxojksyq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2odasjogl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbkrgmqt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hrfrnoqr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhijqwlm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2addnnghc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vgxihalp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2abjiejdc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bjlthpez.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mfvkdlzp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hiypszwb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vkygrfxy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tejmlrsu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fcmctcjj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ebmnhyow.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ooqmzuxc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qwkyzsru.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sdcxkfgm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2llazrtsh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnlqnnh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lbehnitl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hmjcsnhk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tlmpbugp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2rixuepku.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pnsmmugm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ovmvxkor.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xxqmncmo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2avxstwul.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oluyftkm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nkxwlzzw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gxcpyfih.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ftitjeqt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2igdsboux.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2souzblmv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pacjuxll.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fvazclmq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pmofvdmz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2nswlvavp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2kmcmybzl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtjgygbh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2bgfebpit.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qmvowbyx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2usowoxbf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xzcvknme.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2psqeeaub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iygxfvvh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dcjevcdz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vkaenunh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2eutoudfw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2opfjepzl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2dngfpxaz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2wtbmsalx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2pijjnbxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cxqikhcl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2ealtocel.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2volskhzp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wibxulml.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2scrgwfjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blvowqbd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2navrveth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccurmnpz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2exdrskdo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tsviicys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2heauzdiq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rqxeuhol.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2eqxfrerf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wzyjcljt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qppisyjz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hxswztgf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2fbwedqkl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ysftfukb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2slrpcxzw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hlabstom.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xwpyjbdx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2megfhxbd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nmsobruu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cpnlwyiu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2idikuqsu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sfreyipz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dgpbciyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2faqksfjf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qgiqwety.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wyfadvmk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yxccyxhh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jerccsgv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tfobtnxh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ghlsyews.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2avgglisc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wvkvwwhm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2egfeutaj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xftffsrv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zcylgmbt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2aiphqlqi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zdbaavqm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pfnitbzm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2nebwwblc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fhwcjwpf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cwkapoft.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ogwmmsjo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2vygmrifg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2hudgnhqg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vmneqctb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpdddgqk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dglrimce.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abmsaror.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2djxoqyno.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2datkvaxt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fqmbyzpm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2zkwmfbkd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xkwphxil.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2bvufnwrk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qvpbvugc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvapsifw.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2egugzetx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zlhcvtfx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2iuxcuaan.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kqsutqma.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2lscbaxfv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hlbfzaxa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uuojmrem.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwiiexga.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2lhsaqqbf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2grazmqhh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tttpault.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eypjhgng.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dmxxcixs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnrahgiv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hugtmkos.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sidxzoqs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2btvrpvnw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cgigufcb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2watthiga.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xvfkamqm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ykmxdatc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ajgltcho.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ltdoehez.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kmvivcjw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gwgijifr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lurczwbk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2uegzqybg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2sintzdgo.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wlapevpc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xqpwtqoi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ripfupci.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fwnkrtts.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tcbtkwkr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nwwotmvp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ccipshha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hnoxuulk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ibmdxesc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nhhihobe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2setoxtej.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qyhkvkar.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2uvrqtntv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2towjynhg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vsqwafpv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2afjljnej.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jtghlhvh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2njssdglu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wkryeomc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ceyiubhj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fnspxnoa.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rpgrnrdp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vfehoutb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pgbejwlj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rqvnshvb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2rffablap.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2vqndgulu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xftrtaec.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aqfwqiof.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gffipsxv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxozxzg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qoptgtjz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qqequoma.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2swacrbka.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uitqavea.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jmaztpas.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2eeigcppw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2frndrlfs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tkyuyxrh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tqpqoavb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vyzsqusp.html


<!-- 参考信息 -->