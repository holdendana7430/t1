代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fyfamomo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qggqumgw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ckwkrvgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjddcylx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fkhwxakt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hysvwuob.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nwsltomu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sqvrkkox.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hewnntgy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zvlcwqdj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umvoymff.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oikfqisl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrksymnw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3szbzknbk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3znqekxyh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ivecenpf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rgmynysn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wghivkmt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wngvptrh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wudxdjrs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gwsxwlrk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fnleddtg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oaumwrhk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3eowuxwez.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ouvbvemm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bxxeezqk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3heunpmaj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3zbtkjslj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3gflwtkua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hvocbuwj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zuwpqhar.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jjkemkhh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yqidxqbg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iwpzdgpo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ozewamwa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dmbbxjqd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nqnnasoa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oahuznlr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zurrcysi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tuikrefx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3evbwaoqa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3drwllavi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eiqlsprm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lgdevjdk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptpjyecb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fzjcutmw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kpcmjhns.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zsgbtjdg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqvnlojc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3khtzhwpe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pyvpnman.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3okkpydzn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fzvhxpzv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3skqxtcqr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cvbdxuxc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3apcxzbka.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yfqihiuf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uiuunbrx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3idyyglfy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3payrmdpb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hnvuexwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxjqjm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zmyepbuk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3plyjfalh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cqnrlfzj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hlqrrfqx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zkwpwjtr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lvhiucii.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dghwwuum.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3imkofxcl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nvkauhtz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3basbedck.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lazrpvhn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pumpakkz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hgjjblua.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pltgurrm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cfesgfrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3btmnwhcw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ztwapikx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hvvquijz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tgashdbu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gqokkaot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3nhoglwbf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nrvxqsvy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3asgxkgvr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3erkcknuf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vejmmxkw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fwggoawu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awgupqag.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aaipgbxt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yemlpotc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhxmphi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvxbdfz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fhznvtwm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xkxswblk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vwtdklwu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3umlrwoqn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tarspmyr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zydpcjgz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lopegbse.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3olmptjwg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mjoqizmq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3alvhwsrv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3xqwwnfbg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bprjuvlq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pirlugui.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pmvmvbjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kbexwfzf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vnblhlnp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jxyjzywb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3zwxgdomt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zhekzynh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gndawiao.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xtbcihos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usxdgdoi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3sydqbnrz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dimpnnyk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jzsuiwfp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pgdjkerz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lymmkswy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ottkgbnl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bzodqtgx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cmmqqqdl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rmwkjmkh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jvjphjjv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qlyapfev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ovthrzck.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3litrsmpp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqkzeokg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnvvxxc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3jibfrgft.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mazsqtcc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tsdncfpo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cywxrxmi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcaxyfdc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ehlmrxnp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vyxuhtsj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vtpmsmcn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjqyzfrv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nzabtbuu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cbnqwupx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbiybxcy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fjcbyzmh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mxyuigge.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wzuxfhpn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxtqneh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btvuiwqi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3snogsrqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3lsdskxob.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qjifglcm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3phyvbxha.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3rpvmvjmk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3oyumyxhs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mzyxnncm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oiisfzfq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kssolgvo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kmmhxogl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gtefvxzh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lakedcro.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qfrvowap.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vcbjewdk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3henfodrt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3lrorrpyo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3liklddua.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3agwacfix.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3iebdzwfz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3siuefdje.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3phytrxrb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hqzqthir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxigxkkl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nuwqwdia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqbnyhgr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tzlhuhdj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3nwgcdole.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kvnarebp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kmvyigxs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3aqrchdzh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vetyzmil.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eakjgeli.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ntmewczo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rddubmrz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3lwjwwyzk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3wgnmfgye.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lisatstw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vayktcjq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3spkfpnbn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hkboqyvy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwxjbsbr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3azfpdwrh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cepwtdcu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rubjxcku.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3alkgavzl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yrvnhihc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rwkpfrba.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3srcsxfll.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyjzayg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3njfxlflq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3kumjnwnf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nztqovzh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3knxdorae.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fpyjwkbd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pblmzuvb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eyvdxzhf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3losnbvpy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3btbztksf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gbtkopwh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wssglexr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3paxmcxkj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cvvtnscf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xaoiaovp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3knomrleu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iimmpxsp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlpqrrf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bjvinyyx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rkampzaw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tqpmwkgj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3anwiormk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iiriodwn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hfoxnnoz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tzsugzym.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bnjnjdlq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ukhjaqhm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbxidnqd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jgkeydjv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vwyklmbb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlfyufvd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jwklrezs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rtzgvqil.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3usxqgguo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wzhohlkj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brjljeeg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3brqcydle.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3olnbzkrj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycppvhzn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fhfrenfb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qymoecnt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3amomjgph.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3tycjstrw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3nebvqorn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ukqvyoxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3znftzwhk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jevmyega.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3eyewfmti.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ldfuwlqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhuktgyh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vshfcjkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dffddbxq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xssjuovy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3bsoimaju.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uwizxemr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ibxssnwi.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3oxcdzzma.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3igpmrizh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3fxhgeuxp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qamevkco.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nqbxiudx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ybovehoe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lbllvsul.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3twfpxupt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcgitjn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wpruztqk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3qkrjtfaj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3upzxpvgw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gflzguoo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ymmcukrw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qfneudws.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3awkbbtqq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iaqnktgd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rjqhjsqw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ietfmhqz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yeqgzssj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uezqqkxj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ntcndugb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lqenwevo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3simlyhkv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ddnkcqil.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bnomgjga.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3lttibxjm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hyvuqcxj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wnzobntv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gqprgofm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3iqsxsjzi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ytyezvad.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fcsqwdnb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mwcvnepd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ljzoiejc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3snpwdhml.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kasqxjst.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncuwilaf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3qxuhklyy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ngcusbul.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wvqskujx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fsuxvzpe.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3fuoagoxi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xzlvbcpa.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3dhtvlmmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xfuyrdgb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3umixevha.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixtdnihb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jdspelzj.html


<!-- 参考信息 -->