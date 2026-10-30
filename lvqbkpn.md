代发 wailian999

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwsqsctow.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjpvtcbxn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gsmhsorky.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gunsdegqo.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gddyjofjd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gvatrqwux.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gyxesaetm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gojqvbjrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gyxpfoutb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtelpnwsc.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/githhwupm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwqawzrjg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gyjxisuww.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqoqygwrd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gfpmztemv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggxvpamkt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gtvnptcou.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsjtddevn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/giqvglqnz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gbhaalqrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmlvzxlvp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/glrjzznqy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxevxaynk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gdbbcnanv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gukntcdky.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gtzwxgnll.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gfhpaoeja.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gjnhgoogw.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gazmeoiqf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gywmejkqc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/glaypaddb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gtmrtrood.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gpsumpghu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfplnslck.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gcmvymfzl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/glrlwopex.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gktbvqfzq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gpubasxmi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gbzfkmtrq.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gocinsqze.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gcczkwczv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gkukyrwbh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gzuxuxmez.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gyvafvhnk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmiaqhekk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ghlietyoy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gbgtrrkqh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnjbjayhg.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gfnplecey.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/glxqumzls.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gpjtmsjyp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gcfkxtevj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gcdkagxce.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gnmwkyuer.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gatenqgob.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gtaftqons.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gvqoaujtw.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/geijzzhbx.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/ggoxdwafk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gglqwdexl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gugrrflht.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwlbybacw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gybuoviis.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gcofiilbm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/goykxtipw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gdvxbfofy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gmsagdmpr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gvemnjqvf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gempfmeec.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggilmzoln.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/glrusgptr.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gvkoaxgeq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gussgaovw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gkcuzpkqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gnokwkzkb.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/giobdjxtt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjuwptldv.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gfywxrzpj.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqaqacthn.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbjmxuqhf.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gijmmlcoo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcxbwqbbm.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gyvuylmjl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfrzhenjm.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gyqylzsta.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gnjzfaiyz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gxpseagar.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gagpdvvqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gvpyghzgb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gxbuxtppy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gumefafdt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/glyidwflv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/galaqezwe.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gkaebqkcn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gdshncwfr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gyzxjsgqw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/ggihqknrj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gaiahlsds.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gnsmxfdqs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gaglmpegq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gbxiaruks.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gfhreeixl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/ghffziftw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gnbylmdkz.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gmrciiqqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gjrdoxglq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/goigjmzhp.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/guzkotanu.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gppymtvcz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gjzwkyixb.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gryhrbwlg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gahhetznk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/ggozahcqg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/godguquwi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnfiizxsw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/ggzuojkjj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gqaiuziuk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/guuwolhwx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gfsfrfkks.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnnhwsvql.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcekblotk.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gbkfyqnqp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gogpigorz.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gzyfrhwrm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gbnrekjjl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gikeymiih.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gzrloqfrg.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdhvxwxyp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnxvurja.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gqyfhecgo.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gvdhkdhmw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/ggsjfpiqw.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gagffrsla.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gfwyacnch.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gbathuhme.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gmczkfano.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gcziwpwbw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gledvolqi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gybvpiiny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gcpceckai.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gxauvvbpg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gpcsufoad.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gopuljjqs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/glkojpoos.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/grvwwyrft.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gkrdcrpnj.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ggwyfnexy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gzystarnq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gykiudtvr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gxteiloxi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gxcqmgbqf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/ggsrlexew.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gchhrcjso.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkuhzzvin.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/giircliwm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gawiuotyt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/geaopxwkp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/grwufqyie.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gzgpuurvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gyddeeazo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gcazhojga.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gnpcidpus.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gmtvllqam.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/glmdqmgnh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/goypegsar.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gtenlrgvz.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtpzpuzio.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/ghsdnuwcc.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gfpzlqsit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gjnjenfnv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gkkpvsxaq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/grxyhvmhm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gkqtvatgq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gecntplnn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gnikwfgmf.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/glbndkmng.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/gtcjpkstz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfyggsrtf.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/govoeiebb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gigzspmxq.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/giltteiza.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gpdufalqf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/ggolcfvga.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gipjeivxj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gybuxefxo.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gjfumhpgk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpfsjfj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gdtqghmts.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gxjmuglhl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/ghlazcxiz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/ggdwvbeve.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/genekvkoe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/geruqvofw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gclsveymh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gosborbyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gutuermqb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gxwvdhqgx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gngbnabmi.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gjwoyoqvd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gqmhhrwiy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/giyvulyec.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmemqspz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkgsgfexj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gzlyorush.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gpusequfy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gtojflakw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/giyrzceid.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gtiwuafua.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gymsdtilk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdoegdarm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/grzjbodpt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/glofkdamo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gmlvricew.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/goxytfcct.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzngdaxtc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gltadodeu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/ghsxpmite.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gxyzobkof.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/glcsqispl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gylrrqood.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/geetidbyc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/grmqdrtlx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gypyagoyk.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gsqcxqozl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/glzcdtavs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gshbiuuso.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gkeznwdvj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gycogaemq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gejbrbrzg.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gfkoyiqfe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyqmfcgbk.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/goxdxxpul.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gynwlfuif.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gncxqbpin.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gsajqmxrt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gfybzepog.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gdnpsjgaj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtmatvbol.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gblfcgmoq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gxlqhxbbf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gsthmlqwp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/golrcizan.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gnwhypxey.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/glgzqkrkm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gxstfzcni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/ghkejkpnw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gpapysxvd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gntnfolwk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gsuneqcvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/glymdfjrv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gnjfunqcp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gvrgsvqpo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaortvnda.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gqznrnncv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjixravgh.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gppnypxhr.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gvvtlrtvk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gjpvvqqqx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/govsnrlmc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gispdhzjs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gcphvaikl.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/glrhiehuk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gwpafwtkg.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gxrzfpjji.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gzqtlftvk.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gmwildgvk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gsqmwuifs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmctoskji.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/ghdtyerrt.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/goxvwgzib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghlxmpwyq.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gylmjbuiz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gjnhgdiiq.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gfizaubli.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/ggkyynoob.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gzugfrtnk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/giwiaxfxl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gergvmzgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gfxhfriqo.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gbopezwed.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gmxdssdiw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gwxlfkktn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gdhpakvka.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gwtfygwhs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gahbkmedr.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/ggbeabkdn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gvvzbmwvr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gbqcibibr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gctagoabw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/ghqsihqrw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/glgslyxfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gyyokpkfc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gzxnfqwwx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gwhhiqlhj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gsivdfyfb.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gsbytaevz.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkxwcxcwv.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gmpcrsjkh.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/garrtedbm.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gqjfqsxtk.sHtML


<!-- 参考信息 -->