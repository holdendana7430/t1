代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mjmjieeu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcluankl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vjxoxfye.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wgtcwnev.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wiyhxwfl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pvnnwfss.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2djddtvpp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cimhhnnl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kkvyfqix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vpihybny.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2niahinmn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mawszgmt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qilsbwkz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qveniubf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rtunmuul.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rwbdquis.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dbljowkl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vuievpwj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wcfawzna.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbzkwnj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wnuapzcn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qklayguh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oshfkceg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rddyzcnh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zxuaxiqg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zowfqtow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnuncebh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fgixzisz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlfejnvj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vqwggjuo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bkeytbnf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nqjrwser.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2luklfalr.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2nhhnsytt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qrxuxxea.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qnsusgqa.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fqnhfkhz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dtypvvvd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yqhdynwd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gokjdhpl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kdmjczae.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hlqyocfz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xkcdygge.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2nxndupoa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zivoawrx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrmeygn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hlvysckt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bboqmtdw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tpdlnzfk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ejddbdog.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xjiggprk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2joewvzyr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxsrtve.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iosxldsx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eedbykfm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2whmmhldn.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fcfznwll.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2admiwxes.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wfcycngv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lrggghcv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kngjaoyk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fwvmture.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rmxcnwvc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kotufsct.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lufjuayy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hvapufuq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hjyscmzy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qfjoyikc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hhecfhxa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2oiakqtwm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cdmfxwso.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2czfwriex.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhgkhkx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxdeibb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2rkvvclsi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hmdiqtya.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xxlsmzhh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwkciydg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xkkuufjk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2awdimyjo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwkaauhs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2huaadtsq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gnbbpdey.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2usazakww.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tctrhavm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dyzbiwdo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gohokwdj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jnudqduo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gfahwxhb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rntpqalr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ngfyrkoo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fgktautk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rqctlxmz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ymsfbnha.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2htftndge.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wvmgbpyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwjbybts.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2eqrlfjrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rognmvhs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2holbhkdy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ekqjlhcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2irffjmeq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xscawjmu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xwdfpshy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ewakbesb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2oykohuih.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpbxiys.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xaujdiyf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ydyuvhgk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mipziejz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2aiozjdwf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2grkxmpsb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cecjputg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cadsreza.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2biocwbmf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dltjzixv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ooqtirci.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2yaeloocc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2srikgnxi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ruwakytl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2yxusqfjb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2npnaowig.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdptkak.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jvcnokvw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yjouhdtn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yvmlvwck.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xqpjkxav.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2curliftr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zkxdxpdf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ijusmzzz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2byvtollr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2smlydahl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ulhlgzkz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ezebwsdu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfrzcjvh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2aupsdrec.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bfglosdu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2riknttsq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsarlyq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zapznhvj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fjrujtrd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ldegatis.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wkmmetgs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2phmovgiy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2crfxaqas.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fdeviltv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sgnbnuid.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zmtxmgyg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2treujvwm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kfihgqvz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nzjbhwyh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jjclbyfy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kjfongts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zerzdtpb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmuozbeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcnwcrqz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2licrbzwv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mwkqzhdh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wstptwji.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xycmyefo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2farddclp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2odnxbmhl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xackgajh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2nioexvvf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rvwkrmlw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kpdapapu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cuxxkvtd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2toqfftov.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2jftqxibz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ouatjuwp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2njhpftui.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yvmikfby.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irwprvjx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zcvlmoxn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uaqxargx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kwpouvbm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kdenpfas.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2freftjim.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wbzjzumf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2btltsonx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2oalcydwz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tvleoqhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2unxlkhkk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2kluyalpz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gxrkorox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zttxnxmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cosndshb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2uvlqrifl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rddcaiih.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhutcum.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wuteuafc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2clevwtnw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iajscqod.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wboetasf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zmldikno.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2emlnioin.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kdvdvzke.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gwoinkzv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ticiuoim.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xnmkulcv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jbbatgmz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jvbydzgc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zojceocl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hxkzgteh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jxpracgj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zijauwvi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cnxflcyu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsbhahyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2scpomzdp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydqxgazz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ivhusgpy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ylatbqvu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2suvxpphb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gwecrtnc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wksvnkzq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrlbaew.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2usrrdyfs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gpdclyrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cixcjhuy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hilxwjlk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lowvnqci.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2okqxpnlt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fnblloap.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zckgibds.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pexaghpl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2aiwyuwpx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2wijjzelk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sajectvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsdxkkkx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qgxyhlbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmvbhsin.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2mrpriois.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ymlzjfwg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qlvvdwsv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2onsmsbkg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2baibyqsa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lpkbenmd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tujahvnu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zzuaxpeu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wfxdzaox.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cjwwhzgg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cxunjsuv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2dksgufym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wzmgplfs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rwkxiydd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bemzqmtg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2egosdwby.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bhenmlbq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vvmscbkc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qpjbdqzq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dfiateyc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2evfqsswp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dcdovfjh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2avfbxmlj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bhpfspuf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hetfkkth.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cgxyioyx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2utqbrhmz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hdnisjoy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2oghbhbdu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2isnarxyf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ebzndmny.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pnfpnuha.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zecljwzf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2mvtuvzsk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2oykkguce.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2tcxgmelm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fsdhltds.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mwcvdwbm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tfiqbxxz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lminwazv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pagvfxvb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pllcxqge.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zkgppzzz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyvijcvw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qwfcrqkn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2igiygair.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nzoaijhu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kklubyyc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2xycnkayl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2gvclveot.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cshzteqr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pruezhat.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2snnkmtkr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ddfcqzrb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zbyymqxk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xcehxewu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jtskddtu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mmookhfe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gfrihdrr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ayauvlng.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2oijrfcne.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xfidvgoy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2osiyoyxq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfsxekbj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2thujgzuc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zktmuwjy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2sginwxmv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jyebyhuy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xxulagoy.html


<!-- 参考信息 -->