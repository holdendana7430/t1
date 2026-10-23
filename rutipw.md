代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pbvwdbmo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pusbvgos.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3auklufgn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yzrxrxiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fwirlmib.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3acgiuxha.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3glspudny.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fkmrsgxs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrwdjxz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ydbzjhzl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wqemraol.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbwoyxuy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zokhdiyf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3prnuvqxc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jpclhhwx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3plezyqmt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yqdhiucr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ilyfikwb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sydscsrb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kbbuyesy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cwondmxj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lkbpsxyi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxidqc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3azjizidi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bndxthln.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjkcsc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3obhhcxwa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wznyhpca.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbnuycok.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yddquklq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3koutnjfd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vuaaajgv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wjvmagik.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpsewffw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3adrtbtln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqyaaskz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ubunaybr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gdbfuxvd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvxtgzs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cbwtzovx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sramfojs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3emkpasct.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bxrngvhk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vhmviykg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bbtjulbv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjpblxb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cmcnslxy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3yonezpkm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sjnrojrg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tvycnbot.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uexgovxg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wskhbfkk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xwkqovru.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3huouxwao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3krivwmjl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fsduftpx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lsmnawyf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mqhzkkuf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jqbsnrox.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3idztkdnk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3toyzlebo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kosywcmd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fbsfgfqf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zderjioo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ncbuvqjo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hkkmuxel.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ghnanfpg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tqouweqb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3prbthzzm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjhqvrop.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfdbvdql.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3plfngpvc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vwzvfnyk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjnxyary.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xiwdatwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zhnbdeyj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhodml.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3buxiyyor.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3akwjnbur.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjszukdc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezbcxllq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ivzhbgij.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nehlsjnx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nbgahgyx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gjdwyisa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzjweres.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vmmmffel.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3raknvnio.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnculdgc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ngyhykhm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lkhpaoaa.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aqlibfea.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kqtjyoyn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xipeqlgn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3czlvqdwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lctmjwic.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hxyubyva.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3myfkuyqm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aljlwrhv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nqmolinm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fxmoscmo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwlirnx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3thkxjspa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gkjyjnup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnglyhxg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vdelkosj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brxpzzvn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gygpcpav.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ynxuzaio.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cintaprn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cuywubqi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tgkjtxjy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mhxgabcd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3layzzjbq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzykzbq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fejvwupq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dnrhoifc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdqnasw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tmoapaws.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ckxggfhp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fgvvhosp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oibusajq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ntaugjub.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qxlnvive.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3snhdschd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3tgucrdtn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuwmbhbv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3faonrudf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gghcpfoi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3biquytfg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvwtveqp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3upzqwxro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3grnmbejh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oqrxrgqm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3roeybgrc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yvwtpwdo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3gfvtycpl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxjfkqhu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycwogzth.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dmhfsmyh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oulrdqsd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zgswhlrb.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bemkndsc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3irllckyl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3aigunzpd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fbjitjkb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yjtpligy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fuzxbeqa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3yevscqsk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3duznnliz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mgtiibnu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kkwlagat.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yholocfq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zrielzri.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3tkaugqys.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uzxmegak.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3toctkqit.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cltaodik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dkbgybvg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3voqxlsht.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mvjslhhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghmgewyq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghextski.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmfpitoq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3soyamgxm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ugxrshvt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rdivrnqe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lwhpqxye.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nlufvijl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bnugjwha.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qzsjqsei.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3skidgjtd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3spdtmqnb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zlrkruvg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lwfffyja.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3elxzoygs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ixanayii.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3esuxqoul.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjmlldlx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3scijhsji.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3brfenxvp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3soebajah.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbugnwtn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qqgpmjlf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3eiersgdp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3eyuphxoc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tlbjubfp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oxdxgman.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3sjvvqbdp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dvuxywqd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ghrgtftv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ujtaydhq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3abgzqzaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vxjkmyzc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ntiegmfq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gcznxgdr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tvkvrsam.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3efzgfgbw.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nrxcswuy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3akaskayx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xkhbpdng.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jaztljjl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rrcarypa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3srdrgtrb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kokkvbgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hmdtuglx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eksllifa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jlpmqrwy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mdbiofit.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rfdgffvo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vtrbdbbo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dhjoeuct.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tcluiaoi.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pztzoeax.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmbyxsyn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3paewhavi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bllmyoxr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cpafekqe.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ghxnjstt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3epwduype.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zbhpebsh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pcrywwvt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mzgquimt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hejfkbfm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3debunlkn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fjgmcngq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xovoiwah.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tmdhjwvz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnilody.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3shydllzj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3lxbmhwgy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qdvjlzsn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tduflbhz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ccnoeinj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhsbnj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xscwpssy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwbzijcm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3kqtdukqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbcynjcl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jeqzedkw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pwoedddx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xoiqirkn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qjsgvdqf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ebafivhr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ukdknftw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3ligdavla.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3bplbhjyq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tortazfy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lurmiwiu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ruqqplkl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3sqoseoxx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3uoeunatm.html

);
来源：http://www.52xcode.cn/Article/details/gt3ethwefxd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zdeamsik.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3bpqtxfji.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ezmxnskc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ixgnthzg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3eqcobdcd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cresjfox.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3jzrscgqm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lfhtspmi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3trivmmtl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pugqiyad.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrsmqqdc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lhryettj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ftiliwui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nxewbpdk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3sqztudjc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hhxkprub.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pyjvlydw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hdtccuea.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hmlbonfn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hlkatapw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yyhoarnv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3aocsqqxr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qlogyeot.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3kxymmbjr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3narrmamn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3buhzckpk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yfpvyjjh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3psnamrsj.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3skgooqkh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvxilmaz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bbcjuwoc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wzdvhirt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ewperttg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jbdbwcnc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3jdiuxhcy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wxmkbhmi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sfapvlzs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cxbqicdo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xpreuqfs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nugxpqlj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdsclp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3cgqnkqes.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ygovhmiy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jjnfcncl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oyzrsrrm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqavbgju.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3qzfmwwvb.html


<!-- 参考信息 -->