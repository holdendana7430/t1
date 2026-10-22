代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vtklbrru.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ptqpntnb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zmprpmpz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cxypnptq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tomwbcji.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xulxziau.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2efizqnwq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gcrbppsq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2mfsisgav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cebiknxm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gkvudxnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrqirmba.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jwjagpbs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2anlbuacq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zfuazlxc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xctgowxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdeiyv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2agwlfbbc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahjdixau.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dugivoab.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzyzncrw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zekqvwwh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mjwhfyno.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qhpfoeek.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2emkvihqf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pfcfhghk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gxebtmja.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnnpvspf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2agfiorzh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vhygdgvx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ffbzyjxo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2howqcriu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vxsxrato.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gvhjwztp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lsznvqcc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pxjvznnm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kwdnjeqy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lvzfazej.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2iuaizyfp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2uqnagwvk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2luyclume.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2chfxcyge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cxxmqndr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oaqhhypy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdvkddu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ewpqlrdh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iukfrjmq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2udssiwnl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2djduxkmx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tdgazirl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ocpghfbp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldlmoecp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjbvprra.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2byxgiziv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uidhxunx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sxrzlvag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ipjbwrtr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmjmizri.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2sgicvjwu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gchnbrxf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bvgwztmv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zsxauevk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2plktvrfe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tosxnudu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ndmaegbf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tszssrxn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2gchdzlwr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ukzxuftr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2uecfinzp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhaguru.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ooojiipt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tidjmzie.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2foulgrra.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qhrhkmpy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lxmbwyyi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bysknbzc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2popcjovc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2urenruvc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xhedkebr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2evgpvqho.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kmgpdgsw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cssjkkun.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rdbfumej.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tzjgptcc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ntfmscbo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2botoaepk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ljkaduoe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kpwabihk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2yywaouiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2khvpqafe.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kegsxcvx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kyaghqzl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jjlbqulz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2majkulhd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2enpmsnvw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbnjtjam.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2asaxiynq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kjplgokl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhjuuwy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xxgzbrky.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wcsslhrg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2qskiibue.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxccsgbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kscawxzw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2abxuqknx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lijlfwwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2urspsrlg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yfzecflx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ivssrpxu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ottjlhez.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xjszagnl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dimvnodp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2waajzbro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ilfmxhsq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nktwnhan.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kwrofeov.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jsuyvuul.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwidihc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ccwufwxq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ffbcovac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmfcygva.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bgfbxnoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsnixltp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fuuhzrsx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tlqmkxak.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdhvmmxc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bevqomut.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gzjsxblu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2rgzmhqst.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rfgznyrt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2matuekgl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2swukmgiy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2caozkigs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vtyfsivt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2iysgrakq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nqcqvtnw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hbguzbem.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2seepewbw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ladvtuhy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ceghpwih.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2feqgclaq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ffggsfjr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zmhqnofd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dczeinog.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mtfncpkj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sbfkrxgd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvolzgru.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hgyfkejw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qvugeezy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vczcnpng.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rokwvrfs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zlvjbewb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dwrpmyeg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ujmlaxks.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fffombbp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jnzjcwuw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2spupxzxt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uxsppvde.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msffgehx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yywcuvrq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uucudpsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sahurisr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tofcxjvn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nlomwumy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aidjdbft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2altovlxq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aghjyedx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqbedwpe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rwnusgdx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2lijtgyfw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lstgngay.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ylbuylzb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mzdvpgwk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2koklmzgv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2iussanwq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bgdzemuu.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2rjnufrwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kitxxuvp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwbmauuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kspzwsfq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ppgnejtg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2azgxqwny.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hxhmimzb.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bsrbtios.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ukzezsck.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cxjloive.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jbnuxfyu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zwshgctm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ueezonxm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uqnweuql.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dcawglly.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2haibolyz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2pkeuqxln.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2jhzaucvq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txsjfqgl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tkxvzlyv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jrdxlajl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nqbmctif.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkxlraxd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xeedovgs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2lmmgygng.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lsaaclbk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bksokfvk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2kdiyqwek.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2szeyyupx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2yfvwdsgh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ydnrwkdn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mfialjty.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2fpqkfybu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cynqpbkh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iqhahsea.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ldcmsfyd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ramoihrx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cppojjyf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rcnewpyk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vdsvxgsa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pdtnebvh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cviazaey.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vruluutt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kkropxtv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrapggff.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tnezserw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2phjqwhfq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ndfpotrp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2fvlvfcfn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bdijmnzj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bopwivcg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2valyfnls.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pduqltjr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtocjfag.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtwfphxc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zeaqmuyo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2surzkqni.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2emywayzo.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qmibxqdi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2uriutyvl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2uxnletzx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bzgesbsi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2unrajury.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qztfehfq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aovmaeog.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ivcguftb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kjmiluly.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2enkjjkoa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ebtlqdvc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fiupeqdw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tqapwksn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fmodstgr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hcmjnebu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nybqfhoz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nnsbjjfb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2njqvhjsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkfjdcmp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2mogutcxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfapsmeu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ahmhkzop.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dwliitwd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hftlawzr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nctfzobf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2yqnagcjo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2cealwevv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tgyqmsfq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zkccansr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2awbwhvqo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xexpfbki.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ywafpbyt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2hcqghpro.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dlnpmihn.html

);
来源：http://www.52xcode.cn/Article/details/gt2ntafgpei.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2uepseisz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nhkvyujy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfdebdcz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lfdwahzy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2acjpouta.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2laqxugzt.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wmvwulfg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2mpsoyfld.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cvcqwnnz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dzbdhefo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2uixlelat.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vwacqvhk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ssggjanj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gvzojnre.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2lwvvttij.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xywvsjwl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2agbjlhel.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2miahzpsb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zuvmpqmw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jczrftfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ofngbndk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2baeotvxt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hirdetjo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vmittwzl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2blrkkgav.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zqdrrchm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wevgvolb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttiwgbuo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2depkavnd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igmhmbhp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2tlnakcfw.html


<!-- 参考信息 -->