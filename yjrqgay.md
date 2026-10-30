代发 wailian999

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gmtqvnamg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gcylswqlf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gdaibabmx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gvsomdfcj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gfdqlnzug.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfjoaajuw.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/geoacephz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gonpdaihk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gibuxmppj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gepgwfcyg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/ggijikozb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gyjfkvgsq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gwylnkhpk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmdrlfivk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gktorcfgi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gwtlkgizv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gbjbklinp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gffntbyeu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gnelmgneu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gvylfegsm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gupvuwcje.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gsovmvtdv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gauzzycoo.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gcpjrqvkr.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzmukpdsa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gacwibmfx.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gvrgpwcoy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/ggivgxsau.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/grnuetvip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/grqxtgovo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/grqlocuyz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gjecpiivv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/guntwesom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/grlritbio.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/glhxgjfnv.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gdyaxfgsq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grfnueoop.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxlrdhfd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glupsupbl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gjdsmqafl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxwyuxnqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gcrlmqfxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gaejkhguz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmexwrwcw.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gbvgnegci.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gtxnxkvsm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/giuqfgbws.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gscdfgrey.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gkftfxdrr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/grpvpcryy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gikmbzgaq.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gnnuqtnsn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gaqjhurpg.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gtugwpxia.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gvohtejyc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzcnuxgzs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gaswifxje.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gddvjyfdk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/glrdoyhor.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gfmhtjxut.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gtlkbfvdb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/geyuovvuv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gthlwotsv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gmmtixkgg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gdqirwmta.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gyxeqnaxm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gsegrcvrg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gdwhznnug.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gjwyzxxcm.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/ggjqqjnjy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gamlmzmbb.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gxjybpiqp.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gzbpelokj.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gehzducuc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/growgbper.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gfugldkxt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwbkyrrid.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghmtmjjmh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gkdqlzitj.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gdmielvae.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjfsnbqfy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gglkdhebe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gfnuqadup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gmjqrsgih.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gyjuhwhmk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gilmjegwg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gznwhhxlz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnqjuxvil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gdylrccbx.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gwjbxzchr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gljpzymuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/giklqmyie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/grjsmwxnc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gbgcpxrff.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gssfvpsqt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gviqwppll.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gdxswkavl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gksmhtqux.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gjoosedwh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gekitxzdx.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gllfasljy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gososmtdv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghszawsbv.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gocaxukgj.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gxlrnvbwo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gbejyztzg.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxprsrify.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gdlhmqutc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/ggvauvcud.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gqwylxuca.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/guaisdcxm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gfsxhxljj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/glgnkneuw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gctyrfkjl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ggkiojrrk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/glkblurhi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjpjbemsc.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gsvjnewcx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjtekhywr.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/glilrkxgq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gcanncjfk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gyrkxoomo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gfymhmxqw.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gzrfkgngu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gewjxovrd.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gfaicplkk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/giufwuspf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gokhknarg.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gfwhonwrs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gmtgnvede.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gabftpzsk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/goflxgjvj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/glfcatomy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gzsteuprv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/giuvltclw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gsxukurmz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gfdorukoi.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gerxagjcp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/geiprivma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gykywxtrc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gyjcyruuw.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gjwwrscye.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gcsyvlbdr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/ghewlmlbp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ghcdyuixu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdovbyyjp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gbyuqsrrx.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gbwsnmknr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gsqfqvmzc.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gdowbdnhy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gfhawffso.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gxnzvskdi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gfzznkkmv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gadsgvmsp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gjviudiwa.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gxoionrps.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gyoujdkzw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/grosqqowl.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggxubymbn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gwgoobhub.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/glbzpzigg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gpyreqsyd.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/goqejcune.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gqucudedb.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/ginicjbmh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gxovbohch.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gmjbwacll.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gurttfita.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/glzwtgkgo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gqwoolfib.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gkygbvzlu.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gzmytkdqz.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gubrrpphg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gceykciun.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/glxiljaes.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdxzeikt.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/grramtxbf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gexptqfpj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/glgjonoks.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gjlnkbiov.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gtjssrfon.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/greaigkgk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gssqorxyg.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gjdiebzvt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gpmwwrfta.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gmvpajxxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gnifbsphi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gunmphszs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gczrtresw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/glfosnrce.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gcezpfrhx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gjxoilprh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnokwklur.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gndpnlvlb.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gsecuxfzb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/glanfcqhb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gppthvwzi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gikjadahe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gobixwvwu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gslrstgps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gzlsdonkc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gesmuncrz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gwmrxewrg.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gtiymobhd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/ggjhimewb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbcngyrcz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gebhjyhjo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gjxnehxhp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwihnpntt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gywziplvq.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/ggvimyvqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gevmbudqf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gocxisahx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gdrdrqmdn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gatyihlkc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtwiacfxm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ganjfxtem.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gvjrzavvn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/ghxxeetdr.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gxhnkejan.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gnicbhjwj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gnaervhli.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gsobitkvb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcbymhisg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gkurhqlub.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gcigjknfg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfupjfsff.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gamabiiei.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gefkcbczp.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/genfyazow.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gyrjzzmkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gxjwzndsg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gvcsovgxa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxcuovvli.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfoipidvf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gkhedmurp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/galasnxsg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gijitqjrb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/giqzqfyue.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gvrhnwujf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gushghitx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gschaeyit.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gvgotqvmv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/giuaxludv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gepkrdnog.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gzqiflvsk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/ghfcwleef.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gdqqvnnoc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goqygyhtj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gixmnvotb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvvpkxloh.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/ggqqskqla.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/glizwztnc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/guxxfmiio.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghxbcrapp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gsbtwuqct.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/ghlifxmyk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gszujhpwo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/ghlarsuxi.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gvqmtlfjc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gwsrxjuzg.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gxosovlhd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gtldrkvvz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gobnxqyhv.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gtywqgblw.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gskfkpicm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gbavnfukq.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gkrkdmels.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/grkamoefw.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/ghzloyhai.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/glwdsgxfh.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/goplzyuvm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/geshnrbyg.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gdfxdzqtb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gueujurwm.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ggydsvmym.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gnlnxjrig.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/ggkwoitye.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gtmqcafih.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/goymormdu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gpbvthgbl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/grknutflu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/ghnrtabyl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/geckqsemp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gyyezivbl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gelqxqgwj.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gbyrarzri.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gvrkgjruz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gtcvtwhoq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gqlgphijt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gmiawcjkx.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gpklvjvvp.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gaovhajve.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gazhbarqn.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsstssaqs.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gdwtuccqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gunteuidr.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gbfejcuqt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gqjkewtli.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gfgqtcwrg.sHtML


<!-- 参考信息 -->