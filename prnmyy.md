代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdvpmm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxshjsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wbyetezc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hraulixk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qqkubtbu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dtltuivf.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ohmeeorn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fircpsel.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jnsriacr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ncvjhkxx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lwkfuijz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wrroyfjb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hvzoggrm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3fpypssye.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ubjzgkgz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ipcovaio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hprerwke.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yntjdlad.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hqmiwqzu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lfxfuvlq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3glokuyao.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cyigzrds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eauvcruw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zkkcdchr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nvyllnwo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3clmtbclo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjockiw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3egkcywvu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhuokdmw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ixuhzutw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjrhcph.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrigavpf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ilhiwldu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wvnmfxya.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xccjdzjs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxivksfo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jwrlikig.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bunrfsuh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dflndrwo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ncchusef.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nnhrameq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rwfztpks.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zqmhbofr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ayqyxing.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jzkszdvb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tgvcenef.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ruwemrve.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vyjaujsh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dejvygeu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pxqbfvbj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wlmehenj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qvczvger.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsbxbrr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kxzsrecz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bmxuaxxo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3padrbscw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcxjmcus.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jbrrvbrk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qhbtuchv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkxpfcre.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lvlwbgmb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yuinmmhd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rsqzsjbp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zgqytycy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lurzlshg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gkijkwks.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kxsixwtr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ktcbpqma.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3emjjnubd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3gorioywo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tqqifiot.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rhgwznga.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3modlxjtu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kbkxptgf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3irhyevvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bnukmbuo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkotenk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vovokbko.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pjplcijz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jblrkwjp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxwfseyz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ijjxevip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3budroyas.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3elryibki.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fkxtczrq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cgfuhlza.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qchzzrre.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdllup.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3eahrulcz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3usknomnl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3evbcrozg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3khvaxtfg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tyyftbbb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbancark.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3hiivojpm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ekerezoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhatanur.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3zvhosqkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsiswnew.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yeptzcpz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nroxrrok.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pdwzadld.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kmaxvtjn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3udhicgoi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mobqbsqc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kyjmpqsv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jmawdepz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nutqpjgn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iwrloiqr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3sclbynbq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hcczdpcz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wiwudkhk.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pvbospna.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nwazalmf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qumqphls.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3imrjdgcc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3promdaci.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cwmazbpj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qnepeugy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qxxwdvce.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ajnfornj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jchgpqfz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpmutgdp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3psqnerdc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lsjqjqbx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mvzefram.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3abeckruy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hlkrjchc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sppvgodw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3okpfnxtj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nvkxwhxh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ehysgbpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ciosezca.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mxjpsmyj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flcpopdt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qrfdzwde.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pubsaeyq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ajbwubai.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qujypyrg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fraqqscb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wfwiylwc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3onaoobqc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3zvjazzoy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3uwymgpcz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nsvlihfx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lbapswxw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nyphhmun.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dankxzxc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fryvginb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kmykbily.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zmrkfaow.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3grwsqaha.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ackomeae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vehenmoe.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mcfbtirb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfhcwcnw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nagaciwt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fektdgyb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xwvsuykk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qtcjaxpb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ldzsidxz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yllpjkkz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mkpnbnmf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ekrzuxoz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3syqmaorh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3shhtdhcb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xqgiggjh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gvvhiknq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3byyxawih.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cmcqneya.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rbofzbvj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mzhxamhm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ltjymddl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3crdpbany.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3houefuut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zxpwjlwd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vkgvswax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3bbsdmjqz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jizsubfd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mhzzonuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zydvnyzr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzbuglo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pfbgdbhz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tpetdhcp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3eyfggpil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zizcuwhf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3scabrbhy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ntufhyph.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zemazedr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rzcebflv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zvztlwip.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3havvokmq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bykwerxw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vtjvrjpv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3oibwuehq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kfvmyihz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3viebutav.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3scxypyyi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qzuqrmra.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3zzebzwhr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lbjkiyvp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jwsvqzvd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qswjvyle.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jborpexr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mpduqmat.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lapuxjsx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqfxdptu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3oydcqobm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rjinztqj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3miihkboz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hbyvxkek.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gztcwjzy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xxkxpmpe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cfyrnfft.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ojchklql.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3htqgojwl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fbteesuu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3kxamzsgr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vzessfec.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rwfjporf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bmrxwqwy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gxczfjbq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dqsynahn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hkerakrg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ypfsidnp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xisdlcrn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ljfwohqn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3limqbrbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guioovxc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3pdixflkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tipqifyl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3saauntpj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3gknovvsu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fwytlgaw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lkkfggum.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rdrytzbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3tokkpycj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ikaclvav.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3plivyoow.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3avroceuu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zlaenivp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xbiahyla.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ayemokvq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3knbevlaa.html

);
来源：http://www.52xcode.cn/Article/details/gt3sugyaagv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ixnlyjri.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fpfdbjwq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3knoxcxfb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tkzzodqk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cvpsnldf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bdudyxln.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3laerxtmw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qnklzqym.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tsdqssoi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rjbbflfq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ttxdhmuu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bzigdwep.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3aeublngy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wwbkozzf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lzftiukc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hninvtzz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rmcgccls.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dogbgvqd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3epcgqymc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gxpaszjy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3rpffejss.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3dqfbwpfi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gxsnmasz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3cczgvvfw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3btnzasqr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ffilvsct.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hrvajiou.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oksjacdr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gxgxkdzv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aowxfiff.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3juxleflb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mwxxxydi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwegajmm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3mwweaeqs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fpgqrtmj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vosptipg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3nsvgztre.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lwekrjpk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yujrfgzv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pvuupfez.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cfhywrcw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ljwqjklz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3iadoeeta.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3doaohhht.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tlihqifn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cdybglkj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3kqcoydhs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3jzfmhlcr.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vuyntwtq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jzjzjfto.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3thqyhcsy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bizygtod.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xwtjpdtr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aabxdaep.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kbfgsjhp.html


<!-- 参考信息 -->