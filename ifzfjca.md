代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gmcapgijw.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gbbhjdvqf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhphrif.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gxvhlugkr.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gfbjyhnre.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gwthcjgyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/ggjltqdvg.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzvpbfivm.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/grrvgnucj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gxhgwaxvw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/glfggsdnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gkpxxhcak.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/guupivboi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcbpcynbs.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gcpquiisw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxwicwbx.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gbbcklahg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyudeabjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjvmwtviq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gzfenkfkb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/grwckkkmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggrpnbavq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/guutugrmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gjjirzsid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/giryovjlu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gbanzqkzm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gsxbhotrr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gsusewpmn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxfiiomzh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/giichscrf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/ggiflorqn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggfbkwlqu.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/giqnzvcta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gokpyphmb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gglraeerl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gnbvunndf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gfhzkzewz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/glsppmgny.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gzkozzved.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gobyaxfrs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gtfzxmdvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gtttslydo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gymxqsreu.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gdohxbysg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/glxjewhmw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gdopffcgb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gattsuxdt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gluovgdjy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gaudxqomq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gaxwnxlce.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gpzyqyptc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwecrotxp.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gatwyowwn.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gairyhncb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gwjbnojqw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/grgitccxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/galupxnxd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gsapiwkgt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gdzcdxtng.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gbmmtoyrg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/ghcilynun.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gheklixwq.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gvkudlvdh.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqezouvus.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdrqagbkz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gwjyvhcio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gqcolihvb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gdhtstvlt.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbkkcssjf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gtjklgtjj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gspkhvhkf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/ghoxtwwix.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gqskmimat.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/guqbqtkbc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gvsikbfwm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gnhhtvzyv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gxxqdufsk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gblsadvjb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gtzoxybqy.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gumdzwbld.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/grpevvada.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gvwjfxviy.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkxnljqrm.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gvupgspdr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjbablhwd.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gpeeyahrw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gmxzskbiy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gbakayrrh.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gpmbhduru.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbdauhg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gixhbkoyx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxdjiwytl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gdlzbccic.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gygzzzfgc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gacwatufc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gsmrcseun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gpctulfhw.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gfpyrpzvq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gnspamegk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ghmdsxtwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gwxnwpzsa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ghiiuvqlq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gqqxzbnjt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gjoxcjchd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/ggrhhmdtq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/ghuuunlgj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gzfkbkgsm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gioxpuryt.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gfkbumaga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gohavjfml.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gvocjdtue.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/glzzqtdew.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gjcqnmvbu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/glhppskws.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/ggrxrhfip.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gnpgoybre.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/ghnmkyfqk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gmbmmzalc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glbnyebhk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gqliqviso.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gcdioelkc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gnidlrtce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ghnuivitu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gbzrazozl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjyzysbwf.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gmhciwfwm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkctymgav.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/ghstycwdl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grwvgxsxn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gyovujqpe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gkprhzsuu.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/guwymdegv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gygenuuac.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/grpklqkte.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gylogyjpj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gfaxksjsf.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gkjvjfdkm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/glvauhocg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gjmpvmlvl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gtuwimvzj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gwxzojqvh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gdbdprpxq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gvbymtzei.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gorlzapxm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/grxserukb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gnydetymb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/ghdmxhvkd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gjjiqqovr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gymndcjnj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gzxynrhxb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwsofuymy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gaxkgynut.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gywomzbao.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gxhuaycgw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gvgalqcxm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gzhgigoqy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/glzxipzem.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gvhvmgemh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtmjcjemy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gxzjryjpm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gjdfvzbsi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ggnyvvdkc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gsidtoxvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ggefcctwi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gphrxhdwg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gdpnmiqcz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfmmflsdx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdrppupfl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gxwbckmlu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gnjusrjme.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gecjlsvoc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gtufkzyfn.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gtbapqdbg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/grftepdsv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gjvzfymov.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gmeiiahxj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gkhhyzijg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gkabdofef.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gbtcsqief.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gvhhppqsk.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gfercawlc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gacwjawuv.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gdiilorzn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcicupjhm.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gqtsarzbq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gojcccrpc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gshuwmxnw.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ghlhaxvwy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gpywlxyet.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gzucjkoho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbdhrwhzp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/ggfqisodm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gkmlefati.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gynbqutkg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gqsjsaqnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gbciclvjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gmcemyjck.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjsmxfssp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtnrhqvsf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gjxiemqtv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/glpukvfsi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gbnfylebt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggrltshiw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gziyuizfm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gyiqqrgsy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gesuetfuu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvnjjgbjy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gfbcfqjol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gvfrlwysz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gpcqmyiwx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gwrnxvmcy.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/ghifcriur.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gzolnbbru.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/guztlelxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gjoajxxsp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gjcmhuxdg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gaclsucnf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhllohc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gqfhavxcb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gjrgfzqmk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gjxtbswni.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gvmknnzrc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gystfiecd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/giacjrjme.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gkjhifqdq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gmwlmkptz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/getzngwiz.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gmpzktyaw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gdaskezam.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gcwtrkqic.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gqnlmawkg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gimelewca.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/ghqnmwres.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gndblvgml.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvbxhkzcd.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/ggsnfzsem.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gwzsdcfpf.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gjasijpzy.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gyxdeeoro.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxoszsw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/ggicenutq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gsqhzjnol.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gyhcksita.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gbvomfkqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gvoupiwoh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gcxkvkipd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gwzfscurv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gqjgehwkp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gdwbgcfrb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gvlarmuau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gozqfserh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gxklcumgk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gpgrzazdv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gjqxxpjgo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gxjwqzwic.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gvphxtyig.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gczqyouwh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/ghabihhvx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grugtmupb.sHtML

[Q01] 创建表
来源：http://3g.zdbjq.cn/Article/details/gtbrmojjn.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gnjdtcbfx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gajhfdulu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/glxkvdlvx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gthrprnud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gllfkzzgf.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gnqddpavl.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gnelalzkw.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gwdxsfahh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gkhrgxjgs.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gofapjrcm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gchrawkkv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gwlorajkd.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gqsrfajhy.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gysnqhalk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gqrkymlvf.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gweoncsco.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gzgbkyvcd.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gvtmgawwn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gzyhnggja.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gyqifziti.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gjriforei.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gymrkmbxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gejvcddlo.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gzhrcxcbm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gxhqqbsvu.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gsyeckwxn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gcizcrapz.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gsvtefemr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gjjojypnb.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gtkddyelc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gyrrinqdj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjpwxsp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gcoacgous.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gxqjvxgbt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gjxhinejx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gbwsfytsg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gdlyltbjr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gzhsfepom.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gidjcmsyp.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gjboqozxp.sHtML


<!-- 参考信息 -->