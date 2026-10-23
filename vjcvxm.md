代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3bnpjtslv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kmpuxhmh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xqdcwuxt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vvxvmvvq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wunfbcqq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ngmejcpd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubcmsrbj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qggrbmus.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3btzbgcvg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfaarvqy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nqfggysj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nrzjxydj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmncxqcp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vdmovqjr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwjxjwwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kjzuuecf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qykvioow.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fcuzdbtu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fqnrordz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bopsmdbp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dzkxqbgh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gxbtsuom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hdfarsah.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcohlgtw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3inubctbr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lsxuedyw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jfabsnqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3igidlpiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3azdhbmnx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzwpoyfw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uaydjsqd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qgmiombm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3kvygsbuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zmhtpixp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gkhvodwf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hlddhxfl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hlyvfmwq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3izsxwvti.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3oftrfqfr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gugdbufx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tbnhilmh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3huonlwua.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3iljmupgm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bqhuetsv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wjsvqnmh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3asdvuzrf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rxdkhxqc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nsmghipu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfsmhfzw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3taspwqys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etpporir.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yckeycil.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wnfaeeyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aoxdznwp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kiixpuku.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3unxlryjy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qqkntclx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3upwvezmc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbpxrkr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3djqcklrq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vjzjdmsu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvrjauq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qlxyxgyy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tfavtiww.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3chqulicx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3eafiyohz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3xqagmgdj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3htfevztc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3blqlgsxp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jaytsuyf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwlnwqvd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dfgxecae.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qtakbeby.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3djopuszb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rngjthsr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qirvjxak.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gxyoanie.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hinzeoju.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fvyqopwh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jdugtkkg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mhxoouqj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpytjnsm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aibmsdna.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ynbknidb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ppigtkew.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vngjufaw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrepisip.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3shvisfak.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yvxydolg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3bclxhzcl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kztfurym.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zqmefeqd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3aorosupj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gdrgvitj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3afaqswzx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3glpfgrdu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqqdmr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3btigrdvy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jhfyidlj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xetjtocb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ajzqkniu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ybkeenwx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wlgfgjzx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xlqhosij.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3atdfrbpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccbgwuco.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwdeqfmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miutdjbd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gjjuiuoe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ucjfmywr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ykuwcmvm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3stmltfqk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qqzyqopc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zizrbcrx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kpwxdsid.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qgicmnia.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wlzgkvrq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3meqrmlgh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3fwrccutm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ictadzqu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kocvuwgd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nczjzfbk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzwvsvk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3adhcaecy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wrthlfko.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bqeouudl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ksacxwyy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zxqrlprm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3boektnin.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fyaszctj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzifzrn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gcdveemg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eibsmgzj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eebvjufe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xofulwkf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zfyloink.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wwrrknag.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3snprltny.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ienbmrlt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lbcpbdza.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bxlqqriv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3elvyyjro.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3jsrtzgpp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3weuswrdc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3pfysainu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ewshpypo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3oroiuobq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3uykadbab.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gkiwvujf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ggujqkmo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vknwkbzd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ymvrypgh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3akkjdpva.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zrwdhzet.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ujvctowm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mokfteby.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uyaacfbh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3utrkaysp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxsgtfjj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bciekblj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3kxkqbxof.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgufisvf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sxpvabsr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dqigrxiw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rgtjophk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lforikst.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xjwqnpiz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sladmxpa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3lfopizxz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pxcwdact.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wbocxpvg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3moettrxb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3gtnrdcci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3klwyljha.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lhlktxpu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yaqbhely.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wlymqfpv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gncypddl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tfqgkvad.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gvxvntnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xplezcdu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwjqxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxmrongw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yibknskl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vahyptav.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uxliolzr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iomstjux.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wpxchhmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bmcxkpqm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qmgtqqog.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3tqkiypky.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3jdpoagzw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3djljduuu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tauvydco.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lhiahubj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3izfmvpss.html

);
来源：http://www.52xcode.cn/Article/details/gt3jzpinsgk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qpyvbmej.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mqtlcgji.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvrkinhz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3sfxidyuf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3anfefqpa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qlxnrevj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dueugrht.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hqgzylor.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3llwwxkus.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ypcfdkmr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kyzabvvq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3inprjeov.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fycyxesw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3thseavou.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3eiyitwlp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wmpdzwqz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3dufxwwsg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yjwxzgns.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3tclxmchc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dbknbztm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfbiyw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3lkhzgsma.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mkseaieh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3digjdwoq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kngudkid.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ziyiippj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3krflqknz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccptjbxc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ybsrtmbn.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3awthqsqo.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3cbvwfged.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iylnijdq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3goucsfvu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hjkljeoa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bgfbptjb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uwbpzuwg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eiglntka.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajdxvtef.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3fulixryx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ygxmqszi.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3txvmiusa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3eenfxnrr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3gtmsnvfy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uataahdy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3usygsbvb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3irpfsxfy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3vznyvgom.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3flksjjdd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hnoutdjw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dklzycjt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3rrebuqjy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aqcclvne.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3lvtlhoxv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dqcdzaxx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oqstwfuo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqlbrokt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3jycenujn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3limjuqol.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3byowulyd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lcqhypae.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3spepqnqj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nkbormix.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jnwsjtic.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lfkzujhz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rkercpej.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yzppeddq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3obecigai.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gkzcsamp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivmmihoj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3bbdodltu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hpkngnwe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hkiktufs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gczmnzcb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3yxvywctv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yyfsmdvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3utkxxluk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nahymhko.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lorrkymh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3zguulgzi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3szwbyclm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3rrhgugkn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3meuqmgec.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tkkwzgbh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3epourlnw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rkxejxaj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3redqryhr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hfqjsmag.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nekuzzpj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bzfadydj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iuwzfffw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eezhexkc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qedqhfja.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fzizcuql.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ktlddndn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3djdneqbc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ubebclgp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vufjwrea.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bnzidiiu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ziusnjif.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bidafvky.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wygctnaa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3enivqxro.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vqqrcsir.html


<!-- 参考信息 -->