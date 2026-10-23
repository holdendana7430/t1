代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tmetburj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zuabqaup.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tsuvyiml.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gvayuvne.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ajslinup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gndezbee.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnqxcqmc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3alwiikjp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpqlxfl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cfigicnm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vqanvgfe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ogspndwm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uxsqhwju.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3likdjwcg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzqvur.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bpsiweeh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tvswcdow.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3njffmrsa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kkvhfyif.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bvgwdkcr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ptbrccwr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jegravxx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3knqynisr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zrrmwpbx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jhaowbom.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xlenphgl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3totmnofy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mvyjxnwr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yztofjla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtwopwx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rkjgclck.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ugsikfmc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zayfkvqo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3chksqtiq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nceassfl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3odyxiudd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jhespimr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhdsllzn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zydqynjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3scprbzrm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3logbxpqm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yealjqye.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zkolfgls.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aiochdcv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3extrisxa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hkqgsnhf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jiurjgaw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kkxsgkfh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kfqtyghh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xiagcbkq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tdkwsqvb.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lyofrmau.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dythumjq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ijqajhkm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lwuyxcfk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wvyskwvo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hqfgljme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcctubr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3blwaxpzj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cfllroow.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kctibigl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rtvaeecc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3juusxbgi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3fjqjmfsh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvhxwisq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ynelxyfu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hjdhtwjc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dwbrqvyp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vdqqnvyh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qqjprznc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fvfdlklk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eurlwzdt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cnryfrlw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nrwnrosf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wezwljpl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aofbycss.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dndsptym.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mmflksqp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qdgvgkme.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ixmdmnek.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dlheejxl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3oitkzybq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ebloupnh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qflisext.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wzoeehuf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cfniouel.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3buayuyrs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pnbmuyah.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqvhdua.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpyvrvsz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dwqjvlvo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3koecqdbd.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xiquhtph.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ziybvucl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tdwqmhrz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eeiijfzm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fczerghg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cnrohewp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkenvdoc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gumgasmq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3bygeoesw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xemkqzij.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3usvcyrum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lecdcrrq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nijmsevr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3eaxxehst.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dlnhuufi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3auxtswwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kweehyae.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wbyrrcby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxpmblub.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zhaahciq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cdhtafqd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dsomcxbe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jiwfmwhj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fqdscmyv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ywsoymwf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wyjxjedh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ahqckeyw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wvlngzdj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nusrcuoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqifzdgi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zdcqoioc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jxwshkua.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gcnuoyum.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oivlmwex.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zyhhfvhb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qbryfhlf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hzmeyuyy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3mknzwelp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rbhxtbjc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fngghodp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cxaquqxz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sbuxrsgy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhtjtxs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3liowoznu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwwlplmo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3siyiyazn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qciafadf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3zerlinun.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lrhzvvma.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hiecpthh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prgabaso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jflvjooo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3amlvvecz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3arvnrwuo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmdoqza.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3awjyzvub.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ssjcezua.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3euskvbde.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbwhfho.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wxuixmup.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jjxpygwu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kgttsqyk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sozsxuap.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kiufxoio.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lgmnzgbc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nkbncjuj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hhreishx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lzhmlxeq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3znhgjhzl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3olxvqxmz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cejirrrc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mtprywpv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3czyxzrtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tykeudma.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mdcdiwwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pacgcwiu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3suisxhkd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ejatjwyn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zhsceyog.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ndrjxoab.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3inuxeana.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cxfqvuqz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wnrsjxkb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mvwhmmhg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zrltuzvn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hopuupfu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ubrfrtzc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vewydmdb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ersefbrc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vycppkdl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fxojlmpq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3zsmwutzp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fipbwewt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3bffwipti.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3oeevcgyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kyqqnvnx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iooaqmwb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ooffgzyz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hmcyycwt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zoyhugsw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3urmimbzo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bgvdxhlw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3funiulcy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vswzgtrl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dfarzhpp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nseemyro.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eonjcbmh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3faynlgis.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xpgngtaw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hujqsmiu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nobxskyc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pzkeequz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3osbwuqub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hibdbdki.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3uyjooqjs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3lbzpnsbo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dyvciqra.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lfqeftyw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyopqzj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jqllluuk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vgvxziat.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3vxhvawme.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hwvkycse.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezebrtsr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ffzcusnu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apjtnjfb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rwkxxwhp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3embewjly.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zbsdblha.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yznmxjbc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ivinrxsf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3grpcgcre.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ivpqfhhe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3urfjfaax.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3umtipkot.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xihmlonf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3cklrcisi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hakggngj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3avcolvmj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3vrtyfrtk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pnldgroz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rwosyuit.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ftwlerne.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmtrjahq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ymfeusqd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3izbluawl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3drjtwbqs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3znqgzenh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaceuaqh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zzawhvbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcsseuqe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zfnracpz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gardiqoy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nkujikmk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lqflcoaz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cecqigur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qhrhiywb.html

);
来源：http://www.52xcode.cn/Article/details/gt3soesaeho.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3nkouzzvg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rmzhcsce.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ayaxraon.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3qfwtjjim.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3huqmkqle.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzjsngd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hzaprcoz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3izytikyf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fjskiogy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eghsuunr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tqufutux.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jaylgszv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3urpdybbl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3svbtdctw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3oqbpulvg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3sksvxlpa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wcinayzq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qvtrnxab.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3stvqszsb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3igyefjoc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3varcwvjb.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qtwcmsds.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wbkuolmd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3fjnvylcp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kpmilntm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3tzjqlmfq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3knbbaagi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3hftzrzfv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3addadrkj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3icdkepcw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hmjjrjas.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3oowqtgvg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ttdskleh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bnxcusuj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqwjkwsh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uehqwlab.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkymgyhk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bvuhxqgi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ggpltfqo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iseinwtx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ulipmxav.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3knrdbfwz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3uhgnwdwo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pixtzgev.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3errpbmot.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3dhkiaemw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sceknmpo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tpwfcvbg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3qnossjds.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3myqgpiyr.html


<!-- 参考信息 -->