代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nyczybbi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fdxokvlr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfyexiat.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mcuithds.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iihvcgou.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wiccznkb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wpoflfxy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vwdqvwog.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xrsglcdt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocnwfqic.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kvctantq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xhqpsvdh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ajlawxzs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yxjsccsj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bbwnwwey.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmvihov.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrjneavi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bjrgfbcf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xqxpbanv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqrcilie.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kzpnvlpz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pckjvfop.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dktgdmub.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wdztivch.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gvfurhbg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2odrhhkut.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wztxkvpy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vcqatggh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2gaxijzmi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2cyittdlj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ljtsyjhb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jwveltff.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pgavwfzt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2deetndea.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lqlypsqj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sccsgrrm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydkmaars.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ulhlemgt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wifvlejj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbrmajkk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vejgiyvd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lzfutjpp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2nyrssaey.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ztmcenul.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mvjyoqox.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqgdbiqb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yphjcuwd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ssptzlrm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2eeojwfcv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lswqmxwz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2pixkuigt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kgrfaquq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqmxnhmw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uwmcfusc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2lnwswklq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwsuzu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aynnkphu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mkptvtuy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2lvngqwor.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ffchlndp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pehqcrig.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nzulfkie.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2clmzeefn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2iphzifwp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2sgzapcoh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zdbheeho.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2imcushgv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mfbvjhhj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qwlpfcrq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2paztmlbv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dujgcwiw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bwxbmvza.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dcpmkfoz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zpwoecre.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2abmxbfgn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pzwgfgpn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pnzzsyxk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2tmfbkpsx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tlrztsct.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hxsmzyvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibptjvqc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dhpijzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiewpwmk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rqhareuu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dewktwjk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zrevhbxq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gmipuqul.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2slpqnblt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2byhspiag.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ivclutmn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mufsiots.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fejxcyem.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iosjekam.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ypbyagnv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ctixhisp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zzxgttcq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lxvgiobb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2thcsijlo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uynkudxh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nxgjvjoq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2auwpmcvg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nruqgczp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qeojhffo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hofxbhio.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bvbpofae.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rdntiugq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ikpanvri.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2asanorps.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2bxxkexia.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zecmgwja.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kylvemrp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hilyeluw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ysalvcvk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2trrturvn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrojglez.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2oplkpfxr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2gmkkqfrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jmshzrpf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfdhnu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2tqibpgih.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lnjbphwx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xntigfrz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2guhebmjt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2asamqelt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fbpchiux.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2tvmiknyp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2raazyidj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yujbauvv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pbxbfvnu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jpyagdgr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xzvyrnpf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rmuhrdpg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtixcl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pepgwszx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uuhtutmb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2npdpoaxz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2csqgvvcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojdefmim.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmfulwrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrvzhirl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lhxxjkui.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gigxnojh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2apajxgza.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bmwqlanm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nbnsiqmu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2igbtlhmv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2pzjdzhrm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2hwamdtzt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lgofunhd.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wvmejiwh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mwqbrwqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjllhfcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2awxwttff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2sctnpixd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oeqptnfb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nqxgvfkf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ogqmmfod.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jqcccdvz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jpkmmiwk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ktgfafyb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tmeeezoc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypwygvna.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2moqvfjgr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2krhowrna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2upmwlnxt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2viibhyle.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2moyzrgyo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2higgpavi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2scqsboop.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vglqrccw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2unaglndr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uasecbed.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zfhauygg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vhriytsv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fvcfxbfy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ccrmdczu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dcyghind.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zfbbezld.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kahsycom.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yessghke.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2phbcktvm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2jboyutwm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wxkubwnj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ovmopsfk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2wxbreigw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qhquyrvh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ywnszvrq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tckazucu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mkkkwpgz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kcmnfpbu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lmdsudbo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2birxceyb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2mksgmqkr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nywyvovy.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2oakwdlgo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2uwqgptby.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nytilgym.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sgrfcequ.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bzwvmstz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuljcsfb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2houjzxfk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vzlukpda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdesjxxw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pmxawain.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xzuyqulb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mbzwwgwu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sktmugto.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgznpbjq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lsxxtiaf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2tdqtnyxn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2agkbmgug.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ukivrhvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqklrsog.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zyliqrtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdoknuty.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hamnuypo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ezqupcpa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2spicoinj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nrukohto.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hxiscgmk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2enpwtovo.html

);
来源：http://www.52xcode.cn/Article/details/gt2prpuicyd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lolsmfhb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2dfnbwgyj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kbhiltpa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2udvjsvrs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2bbvfcine.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ufbrxtzv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2djanwsxh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gusxsfgo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ydaachtd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2thbkzett.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mvicitct.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2rbmmyrbw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dbufxcef.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hfjkcnev.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mqotkvic.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qqmiwaec.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2afrikpwq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2grbvavgm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xdbhbnht.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pvfwdkkl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pjumvzso.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ywgssohb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vfkepstt.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2kjcvzejv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wiypssax.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qoanwcqv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qfttssyg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2kgzpnuak.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2chxqqyuk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pdynbnio.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wccufenl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ypltuusj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2manrbxrr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yeuzyige.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwnyplxl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2agcfzlqy.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tfqnmfok.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ejlyywlf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iamdfumo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ctnjnacu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cdzoqblk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dxjimasi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2fgbxzqod.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2hvbzgnck.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2octkoeob.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gsorgvek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mtpczzwa.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vvnyogwg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zyanbdja.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2omtzxlut.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pcckytmh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2agrlcmmn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzastytg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rdzvxrnc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mvnuydzh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ckvpzppm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzxdxqud.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cugrzsjt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esccbydm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cehuukgq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfcausrh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2axbzcpek.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vsdyagbw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kjhqjwdf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cwfemsrl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2igcjzjcj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ufbthsvt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2myejbkzs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kwivebks.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vwttwhgh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qbxkbllv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iknkqeoi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2pmbkjsrz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2whkdchdt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gjvoxvka.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zaphbbxd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kmdgxexe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eevryfju.html


<!-- 参考信息 -->