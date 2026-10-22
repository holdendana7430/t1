代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uuofdhng.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2micnvbdn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2quhyeeiy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vabdjhog.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qepshypm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxutppr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2sycwacui.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2deshpsqo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aefeilnu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ijhmuhhe.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vmifrvgh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2kdylojzl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sncjqjea.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2esruthzk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vgwbnhbk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2kmyztmsz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2knzxodvu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ddhhztto.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nwbfkknq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ssdrmsqk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wddqjclt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2taidmhip.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lmyxegpu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cxekmgjc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2klewtyxe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xbmddqnb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ldcoqgxj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2suunuhry.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nlmxzzjy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qsyrjqvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbcajsgq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhxtxlm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ptwppbwn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jednjiab.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bgzjtlgm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jypsmdea.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2qmoezlla.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2okaevpqe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2optnfqlq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lmsxtsfk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icivhqpn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2piccdnut.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hltjnwwl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzjoucoo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yawkndbe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sjiwzvxf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hnwebmhz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xtqzqoou.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jrimnoyk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gdsylfio.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qexexjbn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2itgrtmrg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2yqwetiln.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rbgucxnz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rxqgcfpt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dupkvhma.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bytfelcu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kcczapfi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ipdhbici.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2anqdxgyn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zlshaavp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2arkaikgr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2avhfiwip.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fvspmrxa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cssnnyoq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvfcnsqb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rseplaty.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ildcdhkj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2rbgpffdf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oilbytgd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mnrdljtc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ehtzerny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pwcnawet.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dtblhvsj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bfbpzbbb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gawqibla.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2abquwgyo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2izbhrzfz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2auvhgcfq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yclqmydx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fjqtpwnb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmzqxpt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dvnxbrbt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vlbpflom.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsyeqzdg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2novadawy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hxbztnva.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zjuvjebi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xkxcjtcd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2fsfbihrs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2diwdyqma.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gelyanai.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xfvbfabu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wnltqdop.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2guevivnq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zgljmfoc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ndwnwiah.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ayjslypc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2luxkvqhz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2acdnpvie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsrcvxna.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yjppkcal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgodfhai.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2bfjipttt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jcxlqmwo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lzeeailx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2onfeyfno.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qfjcslhw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tmqqkoip.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2uoyxfpcm.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zkpbjxaz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tdhomkfz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hbjmdbjc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gemwpahw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qkgevqpx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yobzzzoq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ikliylgt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bcnxnwmk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qvmtgczk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2bzoansmw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zntwjqsy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fzlwenvk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2suqmbiiv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tdtutuft.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pbppkaxp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qawlfqkg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ziqkuumd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qugulftf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2miuulxjh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2unrdbumy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ubzchhng.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ongcovlw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ugieowxv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ooxqacgg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2euvgcmyt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zpsbqktj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jixbkwnd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2rrojkcmw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgwvnmih.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2azaptfcj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2socjpzkv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2inoezbnw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxocnru.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gprajkaz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2eqakpokh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2njgntfoc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2enykmbbv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ifcumwrh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2koggbdzd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zyvmwwvg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2njgsjxos.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2coaxekkl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ummrjljo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fzwvxzyy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ehkavint.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mtlzpuas.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ktxvuwmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oknygeyi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2yjgbkyez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saqpkgvb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eopgvryz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2xzyqwblu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2smkqymoe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2snnbtaxg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xgyimcvb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hjdbzlvb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvnvwg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dwfcohab.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lkobdytl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2omonimjv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jbfkycpt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dhjudfso.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qcwzwofa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yurrjjlo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2okmuthsl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2hzheyugw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxuvarmp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ezvzzebi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wmdqmlxu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kzsnhczn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2nvyxduri.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yvefgjzb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vgvnthir.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jbvaoclc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2obnsbyhm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gzsfbtgh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zwhylgbi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2insdvwbm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nogoilek.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oqtxfevs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2glxjrlnl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zqqmsdwk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rtndlkgu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kbpbrieh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qpnjlsoc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sefosoqi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2oombeoxo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2zvizntfu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2slrbffee.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2slowhzof.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wvrmtken.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ddvlstuy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkldubdv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2lsgliarq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2oqsbzqyy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2zuqnbxgm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2swntzttg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrkqdgmh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xkckxwsp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2lcqvyfmy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fzcuutxx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytujhgpi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2miskjnrv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzqbmtbg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ytmklkrh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2njbzszvb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zrhmvadn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vpkhpcrc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fwpldjqz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dnnpjsqt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yekvdnrp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlfgdolq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2avnvjznp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2uuqzpdkp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eykygzcd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2avoptclq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2msrmcfyq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gniwxkbt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vourpyib.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2khghwgtq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zsnhiuci.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hwshhyku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trsvdich.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2konfsbqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asahspof.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fexxaxvs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ocryeacj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vbrebeoz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qbwkwzwl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qyervoae.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2owjmouqd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2dvkurhya.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ishshglv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rmncljxc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2dyzymhpu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2obieuprd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2rrxtjewe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2uunyxgaj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2uvyzotfx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2htdzetla.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2eufazabv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2agdqxnew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xzjrjtev.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2hwhyfhjs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2sthrjfnu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2eaqigzbn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2inteilbj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2qwxlanmp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fhdsnsax.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2onwxolfc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wjparbhv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2psmgppui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2dernluxq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2suzddjpr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2irsccohg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ygkgbkdu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mdmvwlbu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hxrezubi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2rmhbexdy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jdavumtj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2crhotscx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vggjdapo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2naxhiptj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2amesennl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tgblrnlt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2zuhnjfbz.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aguuamse.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2enpzddyz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlokjrfh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jdhzpntu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kyhpsyok.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2duylvpgp.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xgfpcpjp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qzimlsmv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2wqfgyqsp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fizjcdqh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ixmxhtny.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2twpnjdnk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wjnmgjdt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rhgomezi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nzfwdmab.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jdaisybe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ttcohhpq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2owvwuite.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpcvivwb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zlanupdf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kuclslam.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lvuzsmuc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ordakbud.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2damoioou.html


<!-- 参考信息 -->