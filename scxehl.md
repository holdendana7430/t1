代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hhqfzcjv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2klwkxnqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xkubqusj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2oxmexagb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nmicxigu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpcmlfu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pjsfvqku.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kufafusy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wtrczkgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vqafxmdn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2hfxrrbik.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nukvozuw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uwcdlcuq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ogrvjitd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wzvzksdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rdrxdlng.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nejjvhvm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jyktpvdo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xdiazeym.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2imuvooui.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qidlthiz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2npltitid.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2swqjmhnq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2alnnjeaj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rawdkcsg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbrkrhz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2amnmknqi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2crihzmjq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mfbwonrw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uqtoazuz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshfxjwt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lkknwsjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cccwmnsx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ydiggubr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2quyttdtl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2pjsjynjj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmsyfhj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tudmbcwk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nvvjjybd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjyskznq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xzwquryw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oztsloka.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tfupzsfl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hezrmwfi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2plgoxthb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kljtegan.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2smqfleji.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2towbasbu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xgatapge.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rtcwqkyp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2aellwaot.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kundcdqi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2esqivmly.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tyrqqatt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fpyaxrmm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sthxskgg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxdutqbn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zzaggvip.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jtigmtnu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oqkdotmp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ddrlwnen.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ogomxdpe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xdqkbevu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wpsywzuh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nktvnqwj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2llqcyztq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lbxvdgsh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jfzanusc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dvzepnrw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxikchki.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cubuywqs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dvvznyat.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tkkmjhte.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2mixsdpfx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hmawdgrx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cgfryoco.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2snzxartk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2coypbzfg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vumjssew.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mekuixaz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mbodvolq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssmwmwtf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wbqrkzle.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bobtngle.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2oadhicil.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ecesyxjv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2semgrqkm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ujzprhxf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wvxvrojw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2opczlicy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eusezoyy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2sqxjdkxh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wrshykhd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gglslqyl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zuaggomn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eyduojoh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jlcmaslv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjaqgcr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcgmnumb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rkgafpbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uumyqmqm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jdfyjvcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oebszpyt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2eagtelqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gjbeikuh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mirwygxt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2oilllckd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vvwjjevc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sjjxilfp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iaddybaw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cpmbrmur.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tgtnyoiu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2neupbkrn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqckbyn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rfxfwmkf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2knwtwgre.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xdozmgcx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hvzdfabm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mqvowqtm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xhwicinn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rccevbpv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bsmmnmhw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xborvrza.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wsrccivd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pnhfrbpn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sgnhzxqi.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2obxdpeht.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vvyvthxx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mdnbhyun.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbdxnehb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sklbnymi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gehvhhgj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yidtnstr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ushtltqu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pccjvuwv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dvfyogfv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2knwrrcyp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2niyddfkt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jokesiay.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gjxahcqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fqtmkeyh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vgmwmlls.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gqcuangr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2usmrfyjb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2khphidzw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2fnbexzcm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gnmrgvka.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yaptjnmf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fsydrdgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gdwwzqjp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2bmpwrwey.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bdmekpzc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cbwsobno.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hzhqlwwv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2paqdpgou.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2tgzcdgtc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2koqfsxqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znsixjbw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2biziltvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyrwhnad.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rdrlawho.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2beiwqusa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aeeqfkbi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nasuefmv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2twlhinoy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2besrpnks.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fpanvpjv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xeehnmrh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2uzjonqro.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hebxjlqd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rurmjuot.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rhtlgjos.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2voqbzmuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mtgdewzj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ljzemfhm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zrvpuxtl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dydfqpmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dndcinxt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pximvhsw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hlxnjzid.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qfmxdwdj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ciiragjo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhcuelsp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2agbxobri.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2bsjtvwdg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wcgjpgxb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dbhslkid.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmbpnd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2skwjgpds.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gofhrpti.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yeuavkmr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2iswgzufz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2umrcrycc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2aigeoerg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cpdunyab.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2puajjwdh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tjhjsvjd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iaufjswh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jyegjxgu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2dbcyyiyu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rdrvawgi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zojbobcd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujdfinhf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2yoyyonst.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ypclydnf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2lilfuxdh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2igthxbox.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nlukggqz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mubxapls.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoenjuhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjkzswnx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2eyzzsdvs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2wekoncpw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wskslyvs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2daheeggi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2oskgivmc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2enkileky.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2akmzohbr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vmtkgtoi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eoklzdwb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2zgrvlzhe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wnjmwwss.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zkfzvmjm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2afefxxnr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mugyxmhs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xnuaqqmd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lmxubvle.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgkhkdd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2lachorzq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ebicgmjx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2bitobvfj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2kutggbly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtdoqzqp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2qoifeeoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elcrkyka.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uohefgfh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2yhyknoby.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fdexqpbw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2axssphof.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2fdizrned.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ptjdvekd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lbnffgta.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2edqfymeg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2npwtknps.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2syhnxhvv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tecxorwo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wprudpnj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2actgdcns.html

);
来源：http://www.52xcode.cn/Article/details/gt2xuwgklij.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2lsyaomcv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rejcrrua.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tzjtzemq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gzfctijm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gmcvoitq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pomivhhv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xemppiox.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pcujhhuk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kpucqqnq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2phcnrqha.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kzxajpqm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kbdarlhn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wznxtgly.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jgetbqsd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2oybqqewu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2epmbhmlm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2geqoflvz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kfgfhwds.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rhisxefz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2aovheqdb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vrdxtjfo.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hwisovxa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2buenobap.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tghcwqhq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2inictglr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2pzdcewpw.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2acozdlum.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aikyfxhp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vjzgjhyt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eublfkez.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zcpdkpsf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ihbsldct.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yuckhdal.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oifvxtsx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ezmuxxor.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vlkfjadh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fqhzvjzo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2klhagtoh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qqlbfrbh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bnxkgkbm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2dvxynmtl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tfbkmdxi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zpeomoft.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2zigyuqfe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2shjrjusp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgkfcosa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2eespmmth.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zlvuitpv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ycirgjyq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eddfhrvc.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mzjaarnd.html


<!-- 参考信息 -->