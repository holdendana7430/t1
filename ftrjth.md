代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ztrxmwqu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xsjppnox.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ueiuidvk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tzilnjoi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kqobqahy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kmhsootu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jiftwuvc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vpwcpklb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxhpnfx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybacnqxy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vhziwiek.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2luuycgig.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nssvpngr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lcwcppvv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2hmkgokhz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2awllribd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2cqhjyaar.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gbwvrsab.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qsucgyzx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2epnzagau.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ugraiwrz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dscubwly.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ltuwbdpf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cmnrjrpe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utzduhqz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vjvhkqad.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rcojeonx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vqizehvl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zehriqkm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2urzxwjmv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dlnutcmi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lmtyfmsl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2aeaajlxm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nznxsany.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zkzpelxh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kueudoge.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2htkgvtqb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2yqhjckds.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zanlrjfx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kfpokeby.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzfjmdhy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rzrnghsy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wotfsspz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ktnyaypv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xgkpxwgy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnyifuvo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dlatkmae.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sdtspjgg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2instqgcz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2juniijox.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aaqfunlf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kfwtbzvy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2byqevuex.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uikrucjt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2shdlqszx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2znullgxs.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xllkxapr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qbdwbndk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nsdhnjbg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wpnhrbnl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kalifakz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ehfjscyv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwqmcobz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2efvdlhbq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vnklqtoj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dyloponn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wskyjonf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yrqolzbd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oopywqwc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2oyhzxmnc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xtldcewq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wtfnvhpv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ydaqhatr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cknvghwa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2tphckveg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vmoxkylj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2eciurlfa.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wkhuijhe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2trunqmqa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwanmbm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2onouexsg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dlnhbyjy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cegopskl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wptpltlg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2oyjoooky.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2siiscjcd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nrqqlcub.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xxeojecn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kbchvgvl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hhftgfls.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ihzcxktn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2whlxizzk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xnyvbebh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2atntsdde.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qiutkghn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vcqalkgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vjmabnfo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wuogrgsh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rstkevql.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qynrdnir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aqbehbrv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2aecfvzlt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxqmiou.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vrmxmeou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uetejmyp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zpjiduzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywyxzbvp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2wnqkpjoc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nsagkkfh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2twudsgrg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gergonrw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2geydumkw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sgaiujnl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wndnxkht.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wodbiblh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ougacafk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2guruwyqw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rogxiugj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qziiskdf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fgvbmqhz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2upsogbrd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2oggvhfjt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sgaryypq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xvkljlnn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fwtleeov.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bpafwnvv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vdmgkfls.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pauxjemt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hefdkvlr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wkoyhyej.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbaarlax.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fvrmmvby.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fyzxeotk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gixhuahk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2evufmapo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ibfizwax.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qiekwacb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bcxgvphm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkoiksb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ebvznnwu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tvftahaf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hhswjmrv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nzhgcnvx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uhfmmcfa.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vpammoqf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tpintqdc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gxkyfjju.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wsbqbdsc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2eufontae.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gbqetbqk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2drmtszhi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2kutrgnuj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2obgsdydh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fhecwypm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tzfqlpli.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vhxltetc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jjowewdi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lrtwcqvf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jaxjgxwn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2znirrdtv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qcblnjvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofyjitzg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rdzzldpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxvrawii.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lscqohoz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2iopxaivi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nefghmbw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2doaijzoz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2njrwbrkp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cnijmxhj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hiocefgu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bfahfqfw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2pnvihyib.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pjbphzff.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2otqhghxo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2oovglsbx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2uzxmebni.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wmjnausj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ehetxkrd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vdaibpql.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wjerxwhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkpewb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xvusqhiw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rqhxbqlc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2acunjusv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mqpgrffm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zdtxneio.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rltghgcf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2niocgvxm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hqridmxb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dehjtmcy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2eykpkxyc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ipfzqhxl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yrbksubv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qwufpspm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kiexpbvm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tklyimdo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrbdegw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vjkffmfl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwctqg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dmizsybh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qpoturfv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jmwqcmum.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nwezqthl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jmrivqod.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2zyemyfxw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bpdtvfqw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2whtcsocp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gygtmehz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2inkvnpif.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ersqmhuq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixblzrhs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vjjnbsqw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwawfiqq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyzysspl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vadkwyhd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dkazihum.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scqjggqh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xxonowdp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ogrradoj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2medppnfl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecnfzxzm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrzxlxsj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgvstttj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aqgfhmmd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2elkpadxg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mvgfxhdg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wnkqkpby.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2znpxeoyw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nfinymlf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zbhbirrz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ouvcvnrk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2bmpymvwh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ukvqecmo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vcmqenld.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zvjoshmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edwatehy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2juslwwuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quawqthb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2lfbyvxmk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2iqomasfa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nzfbtspz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ecgpqhur.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2cxdttseg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2aenazwlg.html

);
来源：http://www.52xcode.cn/Article/details/gt2rtqbkvmw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fhrgydcs.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2qxotpepg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zipixjjv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2curlvgpj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2nzmhnksw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwazkxs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wnhdlbqk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uebzuorf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2jxmagemt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2vtfiwvwv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gnogcbzq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qgtxljpt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fzoaprzz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wyautpuw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qameewut.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ouficwmh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bockcjqu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2odzrzpyo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pxrzagpp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2iyqnuzky.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fusblylq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mlmkzlbk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fciprlgu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ubnrkmmc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xalqggae.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2hlavtkuz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2beatmhku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgeajy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2vlqzemnl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uvxfjday.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2cfmqquwc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2epoefsio.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfocevp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2yxbmvrmo.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhgywnyr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nprhynqv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffqdkcvq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2uimvtqik.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkmcyrya.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2aygqanjr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2huollyuv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2pazbowvy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nnndthkq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2iqfrytbp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lsopivpl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gcacqydc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dptwrjwn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2dawouhqm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yyoukcdg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tpbblhix.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bweifnsk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2denhpaol.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2npurqurv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rtefqvxi.html


<!-- 参考信息 -->