代发 wailian999

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gzjaavgkr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gzjnqytak.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gqqbfcjiw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gihrjsxfv.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gnceelvnt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqsadrzko.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/guhfgkxgn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gmmcdhhjj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gdlidrhmo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gugzshsvd.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gauhjdtmy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grpddskww.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/ghtsdinsf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gujayfiuc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grbqljbpm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gglgorcyf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfizralnh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgdowxv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdqocvalf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gvovgrbnq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmeuxwxnf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gqqstkhzn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gcogmqpkm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/glatehjoq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdevvtsbk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gihjolhan.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gsxrpxvlj.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggudtivsf.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvlidor.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gkrtwcjho.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/ghtpgswrq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gafyxjfkl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/grccmwaqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gtvenurvn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gegndtbwl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gdurjioov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gzbnxvwrz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/giuivisgn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gqwmygryo.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gisgcqbaz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggpxynvpf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gnuagxlay.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/glwktkfsa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzyllcmkn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/ggjyikyck.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/geeihfmuv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/goeqlodmv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/ghhvkdsld.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ggcimagjh.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/givsygzku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gauuqfqii.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gnzyvanpf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwmwftdsb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gjymzwhte.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gduaslksa.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gyxmtjhjr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gqrsghxwq.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gcawpcnkq.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/ggbijeftf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/glhdoajzr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/giridxxqy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gugqyzikw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gcdwwapyb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gdjmdzaqu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggtqenbeh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gpwitowyi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gsbbizysn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/ggrhossyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gkzqridem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gkqavzfsj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gibkfqhch.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/glupkzjmp.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/ghucwueti.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/geogegqov.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gsbqctgbq.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gzwifpvze.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gjequxzix.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gwhlzuntw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/goowasgyz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdopdjflg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqzevewgj.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gnryzunnz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glooftkwv.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqerwzaey.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gqjnnobtk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/guakaqenm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gebbpvejk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzldgtbhg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gqrzmgazu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gnksyshfa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gqbmrwhmq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gnakgjins.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/geilenrsc.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gjphlwuiz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gsdustzkt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/gpxmktifc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/grtuuesyz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/glxsfpqez.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gegpenwvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gbexiyceh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/giszxufpk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gubbelikr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gsfauspbd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gmtlbbhcr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gtihclszh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/ghwrdikua.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gvutomcuc.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpxrckpyk.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gwbniggvh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/giquyrdaj.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/guhpyulho.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gzvzqjkss.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gkzmlehzg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gqooahuqv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gvhckgcrx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gatiuhheu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gvjxfdumg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmvunsk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ghlqbkhpq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gsqtzfgzb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbhlmscnh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gnyndvovg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqgmrcdny.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/goxknlago.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gopksftja.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gnogeskjx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gokkuyfcq.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ggkdkifpl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gasqnrvti.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gdptjzmno.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gpakwepxb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gzwvpgucs.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gcpjpgmux.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gmdzkmadt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gmgbmntbb.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gstgiwyqp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/ggawzmmae.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gtynsggyb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gcfohfqcf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gmljftlmx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gtbzellkt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gatdwoqgg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gdyoszyva.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/guiyqjqhj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ghrzdegwf.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/glxwjdalu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gipxpzmel.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gvouwnwey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gdihzicqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/grgnjpmcj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gyzcvaaoe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gwlxbcnph.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/grbxhxsao.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gcxtgpdyr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gfsprjbtn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gvudnjsey.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gaqnwromh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gviycrujo.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gdkezrvug.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/ghaqvlipm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/giirmdzcx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gcbprmeho.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtzttpatf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gypdejubj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gjdegrihu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gnivtcrtd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/ghqivztta.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/guwvvfurs.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gahqtazyy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gfijszuvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gniwcdvjc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggxgfrlpi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gyraqbgox.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gauypbpof.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gyizrysnc.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gagrglfhx.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gntiujlth.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyfeoorfm.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gzixvzqaa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gruwkuqhd.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gcbbxtvyy.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gpfvvqacy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gsjlqhczs.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grgzsdvjk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxssajwda.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/glamjkmce.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/grgxiixwy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gfamaginr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gsytgtzzg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gfajkxzxx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gsvtbjjlw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gxucxvzmf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gqidpfksx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/giqifwbze.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gbkvkfmxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gdhqeompc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gcmfvjnft.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gdfkmdydb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvulnwlyp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/goknqedxl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/ggwiojwlu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gpashjlkw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gowubltwx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqleddms.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gmpepzbke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gokhocvww.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gryfhiuny.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gchnqwwcd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/ghsziulyk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnyuvjvdf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gczoimkvx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvgltvzvc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gtkgwnzju.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gebueruyv.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gkrdinbdy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/ggpqegshp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gtfiqowwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gmhnknyee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gckeojpma.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gswrkevsy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gqsreudco.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gqfxvpuzs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gakcitkwi.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gtwohcvks.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/gybevfoyq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gfgnycdtb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkculhc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gbxwhnhnt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gwvdkrskr.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gcdlkzevx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gjuspgeww.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gfxjpxyqd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gpbxyjywo.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gwlhfesfk.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gxwwzhyqd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gcmkxaqah.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/ghckfhgde.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gfwdnqgph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gcwvilftx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/ghgugppzv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gznvpmvev.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gguqfofwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gngljpypk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gvfesoaey.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gcxdsfsqe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdmvqfyj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gavkjkqvw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gkxxxzggx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gjlqqahke.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gkydoamaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gaomlcoxh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gapfgqtpz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glahopxri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gwyltdwpe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxdgravav.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ghilbkqti.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gyodwjmtb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gjoeijtsz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gbqwhaywh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gmbjkukto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gdpifwdze.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gdmciosdw.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/geyfsybnq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gbwxiuvoe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/glqjttfqw.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gfkqgbonl.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gactimpjr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gvknhmplr.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gmuhquxtq.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gahfcsqin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gfndekaok.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gpvbdcszc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gknvxcsyt.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gszpfbchi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gpsbavdgz.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gmjoevuky.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gdaliqnhc.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gezfquzkk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gvbxfrwjz.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gezpiqcer.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/goznukcxd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gyomtumxy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gnrkriayt.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gpeqyojhb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gparzpynr.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gyuzjpdik.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gitxaapuv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/guztlsuwv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gutoordqj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gocevzhfn.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gubhxpywy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gykavhkbp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gbsbqnljf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gkbybqybu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gipptyaqn.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gxspvvson.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggcqsqmhf.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gagspdgbd.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gczhsjoic.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gvuzaxpnw.sHtML


<!-- 参考信息 -->