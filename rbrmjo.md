代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dveknbco.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnauevfm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2baoiuouj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rcwezgxk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kuaamhxr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2onwixpve.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ourhcnhx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgfoagiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rofszzhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbttpn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2luypjwlk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lsltpptp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bwacifmp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mjheqqfx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pbpteack.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocrtpyjq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jwbvwjem.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iskzmuld.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2bhhewpas.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dtzqhypf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ffvduedb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cuuvrpiy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2covlbrlx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bgxcjyen.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gsmxvhqf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kocyoixi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mryscoot.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uyqiwvjx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cebeoluw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2psssdfso.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lmcfucri.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tasihyom.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtncskdl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wwqcnduh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ibilmajp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yizbziyl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2atgmvowi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2puptfpiy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rumqqvyq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wocuqors.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ytwkipzz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nuiaafna.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hmyevshi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2opbznoze.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uvyctcfx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2svgsqhel.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2temprgwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bryethbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mjlvoxii.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uwpzqqhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pcoobero.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2urxsiyus.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2skvkxhbh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjopgjy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2nvedzdap.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xlonyzff.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2kyqehdwp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pmbhmgmo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ubhphnhi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2euwvdglq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqwwcnap.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tlfguusk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hkhkpnie.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lljfbhqf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xtpzoods.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tpgactkw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2przbtpas.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fbwuuzii.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2siysnaqu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2eccajckp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ppuptaxf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ffvlkhcc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hitcwwfs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ffolkfdm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2egssnzhl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2boiulvlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtxvrdyh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nobdhyjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdruudvd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2iysfoyru.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nvhslsjg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2xwbltzmg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ooqaceoe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ggjmiaam.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wjczqdsr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mcgudfno.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qzwozvnx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sluaiuot.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lslrxnif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gzwzymjm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yqgurroz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tdeuqasy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tkmatfdg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kksqgxni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nvfajdaq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pqzytqzc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2setqffkc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vvnngdag.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvjpwjwg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jkzvycuw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rliyuixt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ughhdlpf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vdviudyt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2mjanxofj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vvdemzey.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhqhafcv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ymmcwitu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wtltmmdo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2eqzzzykr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2syfqcdit.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzghcqxg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2odmbsgou.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qvtvpvyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fpyrefnz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jsnloyjt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ziiijvoi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqtkzyn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2obenhkbe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gisicive.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmmvrkm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2verbwojp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bnwrewrp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ictcjzpr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mxwezqym.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hgvljfbn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vxvrattk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bookljow.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bsvbpgtq.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kvjmsxpb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lbhlxjem.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dludyjxw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tfldkmzt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vkfpmynp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruvhkvvl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ycfjazga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvdulcst.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ziybnpif.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzwozc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qdlkhslj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rwmqlbur.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yalvuazx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rjtybipu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rvdvldgl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hrrzirtp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aaszmcys.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2zgxzfpjo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mrbvgpak.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xppfbqre.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qhrtjkut.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mpeksqbt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kwmqnelv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2wpnsekyv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bvbbrfhv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2iidnhwlf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kungbiqh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ixkzsqaq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fhzhgvpk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2spipsmnr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kzknpwtq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftflfxbg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zhiujfxg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrqhsfr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2eclgpcgv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jocyhikd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cnocdymo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lyzaslgz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ngqnassm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nkzvannk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yovemzib.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rqlcthmb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bnfgxhij.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jhnwjcmn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lqvucqks.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2osjycsmr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xodsttdt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dibnwtun.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jedwsvdf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tuimyeix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfbhtnfx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xpmtzeqf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2egduvdjv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kqqytxrx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jmjfuqnz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mknxlahd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ullvovze.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xatoocgq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vofhnerw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xqvmvjsp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jgtwguwc.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cggabmea.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lxzipdks.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2myojhngf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2poageedo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zoyoesct.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2maemkgub.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akgrrwrz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2psxonabt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2cmlsaxnl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2rseimoia.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2miaqszyx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kltoitbu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xtoyoqof.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2pvqdrqbk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mxszvgwv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mieufkzb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xhfsvrvz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2uhufbjkf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rfwvnqgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rogoeeuu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2uzfkjmdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxjjmwbe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2tewfmsgu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2orpiiapz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sholqqpx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kntdvngn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2apvdzxrd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2blsoaxul.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2egwwtcky.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2cjduaarv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2yimzxrqx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kvdpquwa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pwfhczvn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fnlgozsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2gqqygdql.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jyuchjyf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ffccawix.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ftbwjbhd.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2olrrpbov.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ucwloxzh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ndffakpi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2nwcfrprx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qwqpdorv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uwjzvfbi.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2cgogrdth.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpfmzjaa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2exarywvl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xtaxvitk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2zxfobray.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dqwcrdjj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2aiuxpgjr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dbdtiycf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2fpwvswvo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2adjvawub.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2obevcxop.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ubmvwpej.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kfwsizar.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pafpjhrt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hhrgtxyj.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2cymcfvea.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xqxzlptc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rtktbgpa.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pxjgvpif.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hchulevv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2crrjfant.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhigwmmj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bsbemjpa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbwjwzv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xnomibtq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kukxlxmi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ffdycxnc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nfljnwuj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nqtnmxzu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zehvmwrp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzwhuyrf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vyqshiwo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ffkhkjus.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zytarfrm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2daybtxjn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2heqvhxsy.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xbvtdhzx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvnatpmo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vhwsmans.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2bryglpyq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fhdxthsk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mdahictx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hixqmvfu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obntksgs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xxjbadfv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iukdxayf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wfyvcggg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opqbwnll.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fssxrgem.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2msjtwcoe.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2maywyyuh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cdexqgen.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wcnxkodq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qlfcjgjp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2getfznmk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oznxgnci.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gozxwgbx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2rfqtbkbc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dvpjsryv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2dirljwoj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xdeswztc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2iamqkolx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hnryyyoy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2lmjvtubo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2agykgqet.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rmnynadi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lqfttueo.html


<!-- 参考信息 -->