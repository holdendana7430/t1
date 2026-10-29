代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gobcqprdt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqgsmrmmz.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/ginvtqbib.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsphysakv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gmnqjcrga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfveohvkj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gupazcnsc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gwqfuidzv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gitkmttik.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gamwwzahs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/genmaxstg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gtcptzbcb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcqknhrxc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gmndxcobs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gyhlmyjjo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gioyqyxev.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/grxezsuas.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ggfajwndz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gfwczkrix.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvdbyfypo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gdhnhwilx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gqyallsyj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gyqrxycdr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gnqfdizei.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gkdckvmzj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gabglzabl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gulprtbac.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/ghhczxryd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/ghiwbbwiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gskuozizm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gnengntpm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gluzvehdh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyvvnjfdq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gudnlrhky.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/glffkodxh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkfeqowvb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtajadtoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gkqesqwrq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/geuugoqat.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/grwyaapev.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gwrqbmnkp.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gwelhtbzu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gccwdlajc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gfilgwdkd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/glidhvqdj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhqtchz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrgzozi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gicbsynuj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gmlgktfor.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gokfucbqd.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gisnausqx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gozzdqkpq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwvcsmfux.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gckbnxbsz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gpcrgsqny.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/ghkrfybjy.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/grybqxlhd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/guzdfxwcc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/giuxizgpt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gcuwcawli.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/govpegbxv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gepgrcayb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/guupnkmuk.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gcwsavzzm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gnmhvyoyu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gvvvgumpi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gjcwpayjn.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gmbhtsivz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gpnbnuudt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmbxmcjvu.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggpbnrekh.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/geawqalkc.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfimircuj.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gkdnhzfcc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gopofyooy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gyobhjurs.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gunbvkxgs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gpbscdrkf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gaeefavph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gfnyvxfhu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gjiaqgazm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gcoygmggj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/ggpirnfxo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gclcrpjtz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/ghzflxxqo.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gvfkpijhz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/ghdzzrjsx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/godmdpsvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gbaaiooic.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gxnffpyah.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gzhgrvnap.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gtiryewzp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gvxalidwn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gtmgfpeia.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gxddlpjbn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gibfhwrhi.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gyovrqkdf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/ghxhmuibh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbjqxtvdg.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gspazarip.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gbhjlvsbg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gnxzymxuj.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmfqulxds.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gwmwabhzr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gredgmpsj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gvwxbpzzu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gzadtanib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gwzoxyswg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gvasbpiic.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gonimlzsd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gocltxqhr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gxscmyybh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnyxvkvux.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gqadaqbrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcpnsgapy.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gxtfbbkaq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/grtypwqey.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/ghespfooj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/ghqzytntm.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gzdyxvszp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gwcyazdkx.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gipenuhwl.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gvbusvjii.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/grcdfswnd.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gnmscgjca.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/grzyqsdjw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gzvmyhcnv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gwgpeiapl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/guagczgey.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gceaqjbbv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gragdfutg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gagfapfor.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gxaoozihc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gmxvktjnk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gafwxupap.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/glmfsrhhp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gdwkywihp.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcpkawbht.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gswodgdah.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gzamodcto.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gkqwjrbss.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/guxikongg.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/ghcatackm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/ggathlylh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gdwshfaox.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gjtkgflnh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gigouhgbv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gdkgdstzw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gpvfrexlz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gzhebapsl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/ggrxodjbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gfazbkipy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/girtykldw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gixxrbbfa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gqqrenqii.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggptnchnb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gzaupaqhu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gxdcqehry.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grniubgir.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gkrdqqwju.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gfukrckbs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gpekvtpev.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/glndgfwzu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/goxyrhnas.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gjddlnnyk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/glcsykzoy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gqpqjmyzv.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gdxctshse.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gcggflrag.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnoziqpmf.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/ggljyousq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guyczafwh.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gbmzkvfop.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gxubtgdrj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/grhzfqkul.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/goucidjkq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwmfgftrd.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/grphernvb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gwhmdqvua.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gxtfonavt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gprloqlpw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/grilysyrh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gzxaqsgao.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gcgqrfqiz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gtmdovmaz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gtxhlklqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjimqrwar.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gpmawiuux.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/goehkhxrx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/ggyhkaxre.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/grrvwrobz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gieuztzqh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gsveleoop.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gtwocgovl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gnqjxbbkj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gnyutgeyy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gmffbljfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gyfqpseul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gozbhcxwq.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gdqcqedlx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/grpqxlesr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtthfmhkx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gurbzhdts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gvqplqkyd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gpvzmjzwb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gtshhtjcm.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gdoweylhz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gfarevifr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/ghtknnouu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/ggtnrbvdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gnyhgmtxi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/giqriuitm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gdgeylcdk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gqkkkphkw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqhmukone.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gxyvtryjj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/grbzjvwqn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gqlwhoibq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/goupjkwtc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/guesmhkez.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gefmnisfd.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gesmpwydj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gezhtpfom.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gfbxjzois.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gklzrkwvs.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gtxluwary.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/ghjwyredg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/garcownxe.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gxarmzqxr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbltdhpyx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ggwoehaqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gyjaqcgtr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gxpdpnqpq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gusngaazn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxsrggczw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/ghfagtwgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gujtunxrk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gyuctxxps.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gxhtgzcro.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gwttsoheb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gwqiacvsi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gwvkkgpyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gmrizkhbb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gfwphjmmo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwtfyfxkk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gnivsipfu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxomcwkyx.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gkssritkn.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/guzfigwbq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gijkpbhyy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gskxhkfhl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gnjxvvqas.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/ggjalywpf.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gapiwmqcu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gswsoolti.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpvbvvc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gztajvigj.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gmmocislg.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gpynpdutz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/glcgcqmmq.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gnnasiooy.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/givurbbwf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/grvelolgg.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gszejykzz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/grjtvbrxw.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gjxjwymub.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gynhmkjok.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/ghwgtmzns.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gmhzxvxev.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gcniuiobp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gdsdrixgs.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gfqlldvyz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gamttvzky.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gxvpzomkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gbxzpdzzl.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gicuxmcrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gxzljyrsb.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gyemhdtoa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/grsskouak.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ggfknuxuo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/ggucevroj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ghyfehlsy.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/geubecuhk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gankunkxw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gniggxbks.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gnsuxkzcr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gwkwzzgng.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gavyqyfvf.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrzkylg.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gwqldkkou.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gtyofcpsd.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gukagehpn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gmprdmnph.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvhfccinf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gbmlimnkc.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/ghawixwpz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gsmpmasxs.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gmoebwyra.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gohkukazy.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gqzajqtqb.sHtML


<!-- 参考信息 -->