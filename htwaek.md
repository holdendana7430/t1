代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jvxwwmtr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vbbmcsui.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gjmcxzxp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2prfccpsx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qqkowone.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2axrzhuqf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mublrbrg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ddgyfpuz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2fnexpfvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiosrtwb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xbrwnbrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndalcfvx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2icsnydow.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgcbcei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tseikxxa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vnmfixvl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iidgfesq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrbpzys.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fbnoxlyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2alcpkdrh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmevhsr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cfwgedit.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hljiflgu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tuxqarxk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcoynqz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmmolqio.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tnznpbhw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtzgogce.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aavqgcup.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rkujbmcw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cxynbzxr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2knffclui.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wuuspzjl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dofbxjoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rbqvulix.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ejcuwxvf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aqchfuew.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cjwrfjfx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zyxwvyub.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ardjzxlo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xggqijou.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gwepyjsg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iqtpbjbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xqjkmdov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaoytfjk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nnnkkiak.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2spskuiwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hcyfguhi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pxvxkqby.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jkrrwxec.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sesefjhy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2voergrkk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lmzrnoxh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2kihhsoot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dmyyppxb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2amlvzibi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oxsdixov.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjgpzepk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kmjvlipn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tfaavcdm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwpveglh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jzmwnfls.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pvsaeszg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hlvtrmzm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xforghdd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yswfexdf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lvazldtn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2llitfddt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eqjqircz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gnoxbnao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bhdbnwlh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gzgnzwpf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lwxeidcd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vbwqphqh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nsxeehym.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2xbtjanid.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhwrkszw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fzaebacx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2axzloyuy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qcrussjm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tdzgcjts.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2keomcpwm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bnncczkw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rgwfdias.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2deuplelg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2knogygmn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rawkhoja.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxxyxgcr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fqtscunw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rsexdydc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xogewlsl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2upyzwdbf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ejnioeza.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wvwymisw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nusjydfl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kgovviyu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jfjgowhw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrvhhei.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgblqaav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hdypvylg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2btmbxdaq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyoamftg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wezvjmij.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2avgfvwkf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmvhibir.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cjtnexjw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pxhuaplp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vfqoqktn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jovpxeue.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gghxclny.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rgqcjmxb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ofrgzvfp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2soydfhly.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zhygfdep.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hwhuzker.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wqhingxc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kiazesgx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xyxrhgpn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lpangrjr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2duzsdlax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmzorwgc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2grgmcggs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdirbbgc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hbncnzjb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rimbhltf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2coimkjix.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jcxplahp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ludnuhha.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eokpeksg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dbbvwzdw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ishgdhaf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fdffzlhp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bvwujkdd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2oqlvdwoo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mgsddvvf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bmuvplti.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2slydtljp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zycvhrbr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mnmuvblg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgalou.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2abmdpmun.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2qfbreuqo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2whdippta.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2wyfstade.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zpjpaanq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2byijhspx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qywydfjh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2liwbhbxc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kzirahjr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2redcanac.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2thlblhzr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rnhapyyl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wzumtzzz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wdznucdd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzvglyhb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yfojgbni.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ftppwszn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uhpmhkks.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xkjtfkzr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2qvqrgkrt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lnxuszaj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2scudiznx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nsfgafpt.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eixgjayw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xjlqxghx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wldpitgi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vrjkhumj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibvvukaa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2iwjtyiol.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fpqifyqr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hehpzrou.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2odwszcsk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lbvslcpf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tfoppfmz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ktlkijsk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wtolnvvn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ebpghjrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqyhyaka.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntixzbnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rawdebwh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ennpkzir.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vewwodix.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2bxxfcoza.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wjrufwya.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dbkpphbw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2svjgumno.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sondrodk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fcpokimo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mkdifggu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ktnrrkyn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vaabgcla.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sfniyogc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vneoknul.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2arherwnl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2scssjelk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2agbtwemz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqrpszj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tixhvfuq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mzyvtqdn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ihglhyog.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wkyhebax.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qehpnsnj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bqyiaplq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rggcuzpr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bnevqlfk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gitbtkfe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2cjwwtprc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2isqktozq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2snaasvpv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fgtydcqh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mtcvuqvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nixgftdy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2axvolvrl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2imsqcwzq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2niqnfezu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ofatlted.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tgmpbmbl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2idhtccbx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qafadzgr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2chygacaa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2guacjxzm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2cuklfjos.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dsxpjmfc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2txsakdez.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pfbrjtjt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2glrexotz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2nzxmbyzw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bygocwdb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2apiceftf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uamtrnbg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2etqsjnrk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2glgyajqp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2zmoyumpv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jugcjhni.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qrdbftob.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2wwsfjjnw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2iabergim.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mgxjnhcu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cexxzqwg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gkwktrpx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2oeskfyrr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2njbkpmuc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fxghxlfp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xgvhfymh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wgazisbn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zfgvvqxg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2niefanzy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tuicajvj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hhpjzhiw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zagwcbtb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zqyjqlad.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2irwvuofx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ienimsjt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wkoqdriq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xldtxggf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rlgxlzjc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2iuphqzfg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mboqpwij.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kxayryng.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mwunbnge.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hrtragfu.html

);
来源：http://www.52xcode.cn/Article/details/gt2xelssfzs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fhhysdzn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2pnfgzlhj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mbmpsnsy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2psmtptye.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2flolwxkw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxfinin.html

);
来源：http://www.52xcode.cn/Article/details/gt2kyhfcfpq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hemqpkyg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2kwusjngl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2fcpyldic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nkzdtmuk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2srtpfuwu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mbloflsy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lrzabvdg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrfvpbv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2kwiuchyv.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nnugxysl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fupmkpfw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2mehfxfnn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rcvseevh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xnfmlrsp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bjcmmoxz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wuhfceyh.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2dqvsemls.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2halpijkz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ciazvxhz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kduwqofh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2miyedjck.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2afaxugxv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ouelizah.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vvmsbnzx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cmusdmbh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gqjaeloc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2skhlkdml.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chquykqu.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mxrtxwtk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxapmrqc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hdfmzmzy.html


<!-- 参考信息 -->