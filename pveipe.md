代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3isuzrqxj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fmidtbhp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3whtlsfjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3vqxzygzg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ijaozarv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjxpsyd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dexigaln.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nosmewrq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pizvlvhc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dpdztnev.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rtouojhg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ykqzicde.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gdydtcuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ncboqjir.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lkivdyax.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bhrseynm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tjvxjvek.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tghzhjeq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3nqphlknz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cbdjdkzw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jxvvmekn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yutkbxdj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vhggucno.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uxfykaau.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckmwegtm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujvymeli.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzigxzkz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yvrofpdt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3bwgdburh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3evsttiwq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3htwtcnlg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yhfvctln.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3caawojij.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yicutlgd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbngkdcw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vrksoscz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ohzizngf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3uckksufb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ntebpsuu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eakbxtbn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqheop.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gmcwxbaa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ihiqklpz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3tkkfhcrk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jvrqrswa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3piakkznt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qnzqkmys.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ifspwvfl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ccdqwmuf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dldxbrvz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ktupizyi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ajadavts.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fyiatagw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3opdpwyly.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3juwttaxd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3fpdcceol.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgeucmzv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fwirixej.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nuznplxs.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxwohkss.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qchqdxyj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3atsghuyd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vigfotse.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wcnlcyqk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ohleqmzc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3seutpjfy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3esdkhmpm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wyteeueg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3icrbkuhv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kxvzudqr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ueyltdcc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfbbvuwz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jnmufuro.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cnbrjzkk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ohlmorzr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqgngzy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmdyrrd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bscdibig.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3obaongxv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bbdaxlys.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zlqvuvmz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsdxuhkq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ncxuryzj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3depfxqsf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssuiesah.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pscyajeo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lkqorfbg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ahzwyobt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3elcziiqa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ogmyzivj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3chwjozlu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bhwcfgfe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsugpi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pnbjxjey.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3meegnqcd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3foxygmco.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3owqltkzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qnzcydbw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3odblgues.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lqxqpzzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrhjcyye.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wanmsjgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpmsjzgh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3dgufwnpo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3oydwrtey.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3npifzbwj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3kerysshp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dyyidjad.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mrrsovhb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qumldcjs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pvyoauyu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dcmtrbrz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oiobdyzw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3masepebn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3swsrzrmb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mgniesuq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3azxjwtqg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dicaecow.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ncmkqhyy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wltqgbfm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dzzzhulj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3joklkwbw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzpwluox.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ugfigynw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3abuceujw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vxmkroht.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3shzgykvv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yzgtneth.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yrwdefln.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfxuevxc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tuovejjs.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lwgumkfo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dcsnlsmx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmqbotuq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxbvjumn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ajafcqea.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ftgixjek.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gcqcysuj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mikclwfh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ylgafopj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nmbkavzn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3laqhbagp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rchrkrae.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nmslvnvr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dbwdykmm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kkxjjpty.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fmyimkcm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqxbdtiz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nozwnolw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cxvbrgvt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tpstkljv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pymywiso.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ruxanprf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kyydprjj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tjcgpvnm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3youtlwpq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3stbevvvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btfajnwp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlawkvzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrackejb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gurzwecr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3demoiolg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3yvkvgtrl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vihmxuqa.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rjmngaoi.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ydennhej.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pxkgfwmk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dhcacyns.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pjetktkl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ybqhqmhm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tnirhfcm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3tcxoqifv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nfofpwbi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gqaspyrl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjygjcy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sasmbzkm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uxqtvhja.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ymbjyjgq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3skfhrydu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gzyergsx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3cjpdwebp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qakdxkfz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqwher.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zhwfiiyg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nfcexjxf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tprsswcs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ouwvpoqa.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbmdhiad.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3abkochlr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ighfjnlw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tjylwqjt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nlifbury.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lrvwjqdu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3cvldaszg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hzxnbthz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3atnvyrny.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wiawundq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zxygtlyw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bpvyxnhb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ztmjjdac.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dowzdaip.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xfkrniph.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3suhoczim.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kzeviyhn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3laaeisnv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hpqkdhtt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sbudsawc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kxbrroez.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3tsddtgnp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3befgvhlg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdmdfsan.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mxvzlxmo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3slysaxsj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3jxpvcngp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ykmyxdzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fzxhqpbp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3konkqehu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ayjjrshu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vxqwohdu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oicxktvq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xdxdoavo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zbgomota.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3etwtysrk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ffeuatnq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3isoswszd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wqsajimq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3msxckmxa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vooejmee.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ytiumrja.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wmuxhtet.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sjwxddol.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pgfjjcjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktwbvxon.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3hsvdkxfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnhhjfxv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ijyzpiqu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3albljwvr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xyfebefy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dqyvxmuo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3getebloc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3afdnibrm.html

);
来源：http://www.52xcode.cn/Article/details/gt3ycahmfxn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gbxsttnw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3xyksdsxn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yukaixjb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pjfnoyzo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uppthpxb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qdghunbo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aumpsqkv.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vjxjiksk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3itghcnol.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vywumemj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3uoqllurx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hrdefxsv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3arjizmxh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3akahurrq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3edivzvkt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tluprqbk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oedwxmyl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3arohdcha.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xutircup.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qufrzsqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqnhur.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3irwnizhr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zpjhbced.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pggeqajb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3srsznbfh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fajyoeax.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3xqxgjhto.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vddcwqip.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bxfcvozu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xpbpufvr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ckykcikq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ztnsgxnt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rysplseh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3muctkxri.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvikvvla.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tlavdxaq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jjrrvlwe.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3nbiiwnhr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jmcwporh.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3efdzswcz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iyvnfuzx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3finqykws.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aldxpnbc.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ewzwipus.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3togfnwbi.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3muzxsfbk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ujwijdet.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wratevyd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wkfadexb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3krfyuwgk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ajkmfywm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ovdscvli.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fgcrlvtb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wldwoeiz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jpvzgwwa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lmuanygo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3urvllubc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3algtrele.html


<!-- 参考信息 -->