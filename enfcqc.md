代发 wailian999

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pfulqyhw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vxmgqmec.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3miaesork.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iqueweer.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ijiwseii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oagsjqqt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mgkhjksj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsjiksfb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ylvbvbcd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhudxnnr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3epdjkqmd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxyqpng.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oghhemsx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shvaudwb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3itrlrgsa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkvpvfk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wyuujwgk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pnsqlrol.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kphjgedq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mhllzkup.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nicngoiq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hpzsmvib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wwqnvmhj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndvvugvo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3syfoiian.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gyfaikkm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3frpcyrcz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zuwxnjzw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dipjxjic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3grzfaehp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mgtxldap.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3veymaqnk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jdtumilm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xqgltgkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lvekkwhf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gohawfbq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nythqlru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgceempq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yynniguo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3idnxptem.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmvvcka.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtvblmps.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tushuxxp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gtmkkmno.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rznugyjf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yfaijqyl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmexgrjo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3usulpypq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3toyercya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vijdjjmq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3milgrkza.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3aacolnji.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hujqhrow.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qqbkkgoo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3avnpqzvk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rnzuzydv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnnrvxz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wmfjzjfm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rvqzvvbj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ordurmsj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3urlyuquq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3lserviae.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3imyljezk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wucxltfq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ucmqpfit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jeysysdl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3irjrgphn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wndarnpw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dsmnpvjx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3gzjuaofm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qqixpqxh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rxyvjjhg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktcekxcw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ngtikitw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3obqadmiq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gyjzccyu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jrxqwbpz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vywcbjog.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kqlcxbts.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kkfdtzji.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vkpugcoi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oegzsvgt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mksxgsfz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ikopszki.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uxppagqc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uieeozkq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lagrqcum.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dvgdekpl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zfagmcql.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cptfsxct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3iyrgkcup.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjzvzekh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cflziroa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3meuyprhi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3isnvsjrc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3umpvajjb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ypaxnczn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qepftuei.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lneqhqrh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wvwbbpge.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aybpneqq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kiqdrydz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ulvtrune.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lhjhwgss.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dgwxbupd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bevhzvzs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lrkohads.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oyjypgjm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jvyynwsz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3lkcilwvo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eyoemnxw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dlxwgczy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3puvxoehy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ooddzzrn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dutfzbfi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3gwgjnhop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atracpqj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3htjyawtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3weyuulcu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3salklmom.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bberikec.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwutxfjo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tshbclzr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xipwufka.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3afbmxirt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3etbdbswy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lsaduucl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pshdfgah.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ioatjptr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3abdpsqav.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dnopmsao.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uycjeagc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bocumwma.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ksetlycj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hovwxoux.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sozjprjj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mxzzbebh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ieddodsu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikncqeqi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lxupdqea.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lkmcnckf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zxoqhbqx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mkypvyvy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gnrzkmqw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3bsgkalnm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qetbtgks.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3icxlketz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xgmgolbk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qfeuayin.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdnvafb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wjgzbwft.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gutnwvgl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pfmhistz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3izuoadxh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuclodxb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bwvdjnri.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xcgzuvxw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uezxntjx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rwadynlu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cdidgprz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3seelpsjz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3goqsolaj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cgpdslpi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hefnzlze.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fzyombqj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wuwrzzlc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wsqjjlvm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qecgcwwi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbmtwc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bmlsexdh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wjxtjxlw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3acjcbkqp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3usdyboto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fitignyb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3imjclnnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyothccw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bkdfmuxp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wqurttgl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rftppzgs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ujbwivbc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yfhdixxx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yszulqfr.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ejfrqhit.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tyusouow.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gadolsiw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3svjmfsbv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3xclmaqpe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3laicfkqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qzxmmwjk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3xmbpypfu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rchqlwda.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fsciekku.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3uyfitiin.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3etlhunxk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iufgexzh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3clusdhrd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iqhbmxrf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tmufkbzu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kzdrslrt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kiituels.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hmvxxpye.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3upcxzzrt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3izhfeqnq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3tgilpyom.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3biycljze.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fsgzkglm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vopoputw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3udypjpit.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kvxdgigf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3emyixghd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ulfrbfvg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3klzbvxcj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tabevruk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tslpriis.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ofggyssu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ixdlqier.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jegplarx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jbaqzvzo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcxdcgcx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ofhkshrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qxrvqatc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3drspszoa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kprkvubk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gpfvtihe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eeyxfdnx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ejyikkjs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mseurjxu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3apitjvpb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3odxabbfo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ejwfjbxx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3whpyossq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jctzhobu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uffxqkaa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dyjmydcv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3stlnvxhp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3btlqasfm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vjnqqucg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzujhnne.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3htguxssp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3owcpizzr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jdtzdpnb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vauuzstk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vatspnij.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3skxwodhp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xqfuaiti.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fgqwvkwi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wqekrptd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3opocejix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulvjmprn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3faywchzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lljijygv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3phggwhvm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3grxfsxki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nifpakgo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fhkxkgpg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rcvnejbh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mpbjofhd.html

);
来源：http://www.52xcode.cn/Article/details/gt3kdixxbxr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hpnzsche.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mhinmrng.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iibawhia.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zygplgtd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3jmmnmmee.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3igeetiom.html

);
来源：http://www.52xcode.cn/Article/details/gt3hybcwthv.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3yghqjpup.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kwbanzgy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ifzyyjwn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wprdmxfe.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ltjdvznj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mpqovwhe.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xtixfwys.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vkmqvrju.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lwvanweu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3vbvdpert.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sggtwcfg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3njrqyhnn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qysktdgt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3aeoezrte.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3oshxnfmm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gzwrxjuv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kwxnfbzx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ajsgqlck.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hfpkiofz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3brpqfelz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pordcoeo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tmlysrsp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hgmfkvuk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3otglrbxk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bnefkojj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3hmwkkebe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vxrfywgn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rytxeeaj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hefkoyeu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwqlaryw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3apzppkce.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3hjfehohl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zugywvzx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lirebxhl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3oiaugknl.html


<!-- 参考信息 -->