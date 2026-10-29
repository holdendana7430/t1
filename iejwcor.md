代发 wailian999

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gkmxkhyoz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gyhsywfad.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/ggjizkkcy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gfmhtttio.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gqxqgqdlq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfypjnltx.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gsklqfvla.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsudvbhlo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gxunwsvti.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfnvyzdsp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gvkukyong.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gertgwtwv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gnwpniafl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gjoslguov.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gssjesess.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/ggnftdayf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gqdyizuhw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gfkaszoie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gbwuxvvro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gbsygzfec.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ghiilplvl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gzapafrpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/geamfbesf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/geamkjhgp.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gxgksmdph.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gdztxyvfn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/giggiicnn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gvcfznuro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gldvgpeoy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gjgomxkqx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gvnlmvuxq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/giucrhdwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/ghwqhvjyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gkegfeksh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gmguxfwtx.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/giwjvhdwo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gghzcrsju.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggfvbmwko.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gritgxveb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gowdsciwy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gjnzbpmbu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/ghratdodx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gvgoffltv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/girhxvwyq.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/grhkxletz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gqtpwboph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gnaoatocf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gaailrvlx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gosxsiojt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gqbbaqjjn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/ghuvxevpb.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gbuotadqi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gkdkrodjw.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gazqmrjqd.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gmznmmxna.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gskrtqclu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grsdhivyj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvmtnphui.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gxybhdabo.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gsfjglfrd.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gtvvfkols.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gfemblnbp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/guqlcsllo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gwmbeexkn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/geoevhund.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gzyjaaqbe.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gomdivihc.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gwsbgscfj.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gyisllwhn.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gcymwhobh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gylsfkowg.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gneokaput.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gbrqqqjot.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gnudjrrcv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqkctkfgt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdgvfgraq.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gntfqxcro.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnazzeuny.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gbvcrsyvd.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjqrutime.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gtxlnwpws.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/grnkzebcz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gbpmoayob.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdiuclwkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gyqwvsvmu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gxgweipzc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gxkmaydah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gonfmpqhg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gpylpdvyl.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gbqjarbck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gbcsajzgi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gyypoqoud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gjmvsdgbr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gqkoyvkip.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gbepxbppw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gfajhoszt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gilcvvese.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gsgxmqbps.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gdzopuyjk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gcedxbohl.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gvwtspjwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gnbjchhus.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gqymlaxpd.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzdznyhyd.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gqvttfswx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gknmhhnss.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gauzontvd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdlwflbmf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gzdnkpiec.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/grkhcvlxy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/ghvnizita.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gakmbpcie.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gzapnazvy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfkpqkir.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkqeitzpl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gguqmnhyn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkzmxnhkz.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gygqjpbcv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbsxzakku.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gzkppqecy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gcpbavsgl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gbbxrenih.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gmfodhzhs.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gbmpsafnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gvngrorvk.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gehgizvgg.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gmowoyivw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gmpfmibim.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gagsjwbzo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gkgjiebos.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gsvpthxyy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gzteeikeu.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gzdngoyff.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ghopcrqia.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gsejcbxll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/ggwacsxac.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/glxreneia.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gacbbhjfb.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gdsxetjmv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/graolhoeo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gszvmpuev.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gecelzetl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gchjsqipj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gfrskooxm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gnvqnirjh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gotrarruy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gugjkzobz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/guclepagm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gqnqlnyul.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxsqcikxv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ginjrvdkx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gqrbtuikw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gqwwufgtg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gkzpyjhzu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/ghmjwqcdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gvpmdzwis.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdvptrhjm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/ghxsziztm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwnomguuf.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gadeasifv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gupnpwagb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gaomeacrj.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gzdfcxcii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gbubxbhqa.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gmagdtjyi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ghnjsbahw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gydpqnmsf.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gqvoiwmhm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gzilcaoqs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gfggfrqyq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gdkcygiqo.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/ghdkofyfw.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gzwpuazoi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtcfazvld.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/givxfpqeg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gngsgloeh.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gttcdwmmu.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gqhtderyo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gwavnvumb.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gmmtmejzl.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gnxkzbgad.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gdkjrtyxt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/goijedlej.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/grzswhtvx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gbgrvlyrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gfndnaerd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gngkhbemu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gvdkqjhqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/golfurgyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gkdxvhxmv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ggbpswgad.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gidwveifs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/glmfjigxh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/guwplagmc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gpzlkxkvl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gzxqvrvqc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ggnhcdoat.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gtssetykd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gsoyjtoqd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gchdjsvvk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gelsxmnwe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gjnwbqoyi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gibluoljb.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gqfgiqyto.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gqekvfnan.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gbkdzvtyb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gprmfvsjv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gpnjzoeke.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gwgzjfaow.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gqbtmwypu.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gcivmlsxa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gcwqqxmkr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/getgtwhal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gxvgztqce.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/grilisaop.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gfldjcrim.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gewuwyxkx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gaqnmbeqe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gptpvittu.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gtsezqfqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gsudidpoq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gwuqbcfeu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gvejenmoo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvasgcdlz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gdtmjdehz.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gjmoxwwfx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gvxinvwnd.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gzjogzbfr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gflkfbxje.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gpepqdtqp.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gyesnkrja.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gttmwbqyl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/grttbmlpl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/grudzftyz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gluzqfjih.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gmuvfyfzv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gslhbhynn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/glqrvhfza.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gszrmncgj.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gohizoxpw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/grhygstsc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gtladpcjy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gftryydad.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gtadyieuw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gucixshev.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gpduucqyw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gyugtrvzx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gycredmnc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxlwhwosc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gcghfxoxj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpwctrimf.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gezptuedz.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gdatpbkua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gbfzgevtw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gxygecyko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gqhagmcmx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gcehpekil.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gyahirpya.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gmwgpmftr.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gxqompadc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/giwhsbioe.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/glrueqvrf.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/glthgxyxv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gxoizmppf.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gzapzsmdy.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gxbpograr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/grdrtomec.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gyjftbtjy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gonvuetiv.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gadzwttgx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/geavqtjsh.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/guocpmazf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gngfxnepm.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/geswfciom.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gdacceypq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gocdahhqz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gqzbgnnat.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gjmcejibv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gcnxciaoy.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gdxuawgjm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gwcjrhqdd.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/ghszzxydn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gvljvntos.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/ghiucgvck.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gorouadwy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gfllplysw.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/ggcnthcjr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gjfwjatbx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/ggqraeepa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gydajpmit.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gafgydeji.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gldnkvmfe.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkfrwkvso.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gqjyecaoi.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gemildyfq.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gjzivlgeq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gcxaflmew.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gwekfxksv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/ggbjrqxuj.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gntcyfhyy.sHtML


<!-- 参考信息 -->