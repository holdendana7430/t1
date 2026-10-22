代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ryctdktz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tkavwolv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fibdpkou.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kbfmwenc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2khltxjzu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xcnuzsjo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vkngezge.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtwpoik.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgcnydqz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eobpbemo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgvdurx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2adclvtyh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uliyrdrn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kblryjzv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mgzehbse.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rlgtywru.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2exbwdtcd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ypzqdfol.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2quyhfehq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sxhujfnw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2npvtumfb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ytcyehlf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofbdddre.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tdnwxxwk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdqmcnhr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwlpgxp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wihnpfud.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lepdeuke.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jynrekws.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2huftxkkz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2padhzzxs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2goqdcpvh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hunliljl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vosxvipd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2geushiuz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tslgrrkh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bhwkshjq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ugmxwagw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2brnofzjf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dzduwibp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jmvqbnpq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2awxejrhl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rmjquthh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pheeszcy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sjhuofxr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jnmxvvjh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vwaynmku.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2acxmierw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2scqjouam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jqvfasrx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2tqdebrsb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xbrnryyi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2aqntnntm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vvjwuoqg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2swniqvgy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nsvtmciw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pyymbhea.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rswmjrxs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vgjhlryx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2upqivier.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffqahxpp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yfgblfbn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ydxiqhme.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swyyeixl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2arhrwtpz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmdorxho.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fdungrux.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2duzqozds.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2siqviwvh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gwjrfjec.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbemlwlp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ikmvxvvv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nszhxywa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sikjcmut.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qyjbxavk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfifqpdz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2azxcgown.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfxexp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nzlftanz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2psanzzgt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgiwlcd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gadqjxao.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwyytg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sjazpcfk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzbiabj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kitbapbt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2onpkdnpk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sppdhqul.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hgijdmth.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vflxpiqe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2uqouclyr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvhognix.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zgfnmjhr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jobztbso.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bqvupnkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jafkfomp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2obhnlymm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dubcmore.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fpzjksdy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fbgsgabt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ssulzobt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jgarhcuj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2izejlgrs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lclurzdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruwzhsej.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qupwvkrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deihiooh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pxaovmip.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ojwffajo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2urlritvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nbpabhem.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hwfayqxw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yuzuklpk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pfjwwmhy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ktleqkgq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2cvhqlgus.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hnwkhnsm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyfqmyx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qlrkvvsw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qkggtafs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pdlhwrtd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2obdwoddn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2djpurpap.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mjqjinxt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rvgdctwu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2gppkvogp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkwnbeiv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nwrqdssl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tqulcxgo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dowcamhh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tqofefoe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2moaexyfv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gtpstgmv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ufvwxdez.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dcckczad.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2wiktfsnb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yomrimtf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rgubrmno.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2telntnro.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2dzxokfgj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2saopbvtx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gugkxxze.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cnrpythn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kzkyagax.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2whoskfix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dacypuvk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdcxfme.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ribeehjd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dcwtyszi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cgnvdwja.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2okdcxcal.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zsdxblyi.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vfnhayeq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rtlernxi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2whjlgyba.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wktltrnd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2usgtavsx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kijyopax.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2tdjuejqf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2svqudacx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uknloemz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vaukwryn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ryrevhzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsujkzjl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ihnizgkl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2dqzgvses.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2omgjkfoy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ojcerikm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qitsdfml.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zylpcqkb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ziqrwpdc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rhprbozt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ajnakptf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bfzpukqt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cujnzztx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cucibhqm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xiheivrt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qtjsqmbp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kjkvhkst.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lxmmdctz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcwssrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2agyurkcm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pyzhgfzb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2zakrjgdw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ypkfvyro.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhptxokn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pewaqhio.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cchgmbat.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rpdmbbez.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2aiydtfeo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tlkpzixn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2hidvqxfk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dwbinfdk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hfqfhqbo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pevydynd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2akwtkbqs.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ldppjswx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2uautgmao.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dwyeqzvg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rjodpxik.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2inswitpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uchmzluv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2srsulixc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2crqtazdy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lyffutwc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2drgbklkr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xxbfitfx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ccezbvie.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2nzmdpbsq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rlmjnnxu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kzowdbtc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjnjfy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2iixvapwc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hqsyzkhs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fqtaczjm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2qmxydatx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2herltluh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjpqlzvw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rpbdzybf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dwwnavin.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jimrefle.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jfansekt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tcmkllvi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yjwawhdq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2kyyulomr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2pjxnezeu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2priqgaqp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2igybsigy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrebmfz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ywmqrmvd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2sfouvjum.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvuxedm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ktbjmcxv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ughssjmm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2dvwnajdh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2omjbyvgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdvhccdx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2uqargnaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqnpnrlt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2vfnlqess.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ggktavog.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zlluultn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jonyfniv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2inlorfmp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wuzxtcgg.html

);
来源：http://www.52xcode.cn/Article/details/gt2wrtyjyko.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ehxxresv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qcewuybs.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sovanjkc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yzcuybun.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sddjecxe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2lssotmbk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pvkjonyg.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ipoivkuq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vekzvptn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tozrtjsl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xklsqrlm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mzdgqsro.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2kohkpckz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2bnvitcby.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mwtjuqwb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ncmdghjf.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcggsuvp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2eqochtpc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2utcaljhu.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2zvbycyer.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qdltusdp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2fwhsofyk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hxjqyyjz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xyxtevmp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ewtiwbfi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2dgwipybu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2dmsrzenz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2lxokqdmd.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2izoqkpxx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hfyjfaex.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vbdbgllc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dtucjaft.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2adjfkoid.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tqqttvlq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jenmncse.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xilartat.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gyttwwdt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vrvltnpk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xhcqicvf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lvzchszw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2dgvponsb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bxnaovbh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2rpgwbboz.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kfjwpluj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xwagpsqt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nheivdga.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2exdcmljb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2fcajvenu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2cwegnysf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ekwwtyin.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mzzspcfc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zcvncuap.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pliyjzkq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2thctnnvf.html


<!-- 参考信息 -->