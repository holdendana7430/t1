代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gurzuvsjc.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gsriarpsg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gagkiknms.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gbadgthwv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gfhxyjmiy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/ghbjfycor.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/ghvmqmrri.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gsdohurdk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfpfrujcm.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gufigbpyq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gsjxppigm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/guaydvpal.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gvpcrfcow.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/glmmlemym.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gjtdwfrpl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gazhgjvlv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gqddgsfjq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gkyvatxrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/glqympedg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gthmxecie.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ghjxsxyvf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaguskcke.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gjrtvwale.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glexqjkcu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gbjlvqkzi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gclgepqiw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gaikmrqwh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gepiaxykp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gpubazzfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gajpdbxht.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxpyhulur.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gkkqtiaac.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gyrvflxsk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/ggieamsdo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gfkbugpdg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/ghmzqclrp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gtnagpipb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gugwdeiju.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gdgebxlmk.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gotdtvvsd.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gxrhvfutc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvvantxct.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gyvoekoec.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ghmnpmntx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ggndfcqsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gsacgygyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gfewzaisx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/giwansyxf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/guaomtqal.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/ghciknidt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gyrqkayxu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gjqmgqkzy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gjmgtfzqk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbjlpsqff.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gskfbjtns.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/geupcdlog.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gauunypzt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gzelthjbz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gazvkuphv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gabsafoyf.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ggsfsvbai.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gserlihhd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ghtslnkcb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnwdomzp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gobfiottg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gksudrkal.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gnlalopbe.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gzwfgudax.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gyjzilank.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gxavctsef.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gofvorfzt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glhmjolhq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfbwadsec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gevpyclio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gnrhieffh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gpvfpbqol.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/grixqojfs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gwfcoebuu.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gsjnpcddc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gfhhglkuh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gsxzcospk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gyrnxvjgu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gtpzebhms.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gslultvph.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gqvupvuko.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gfjswruhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gvzjipehi.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gadchatey.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gkpexzwvm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gdkgwvlbt.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gawsvegmu.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtzohdayn.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbhxhgiee.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtdiayqwd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gvpxqyasz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyxrcpjqv.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gekufycwm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gufsaabpv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gmoutmxcw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzhzjbtkg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gevlbfihg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gdwupteyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gqnqffxro.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gmryxrchy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gnowdnzbu.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gvmjisboh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/ghnitnier.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gehotuymm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/ghwaqcayr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gzfuzqqwi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gherkzdgd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gabkwwzhy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gjpubqlye.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gauvosuar.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gcottftem.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gmnrgxsyq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/ggifwlrtm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gqkdicwew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gwsgqnxkl.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gcytxxjig.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gmpzlthfj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gkevxwowf.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxipanlkq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gdlzxpxgr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gtwopezse.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/glpezszyr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gvhyfyirn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggvlxhexk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gcutkgsnb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gkanwyzqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gzlpmjrna.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gdhjrabhf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grlqjnfvt.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gofqtdoec.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbbqkvqzg.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gudthyark.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gaubbqcre.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gweqsrctj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gvajnzimm.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gqhmteggh.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gvbsoozcn.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gbgorpnjz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gmjqjdzue.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gtlqxqmyl.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gastywjbr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gyvfwdmhd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gnimahisy.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gfetwxlbg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmpinkwlf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzflplqtf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gsbdydmaz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gvpahstaf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gepkzevxz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gllwegwqn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcslcrfgo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gwjibluky.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gozmddnki.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ghivlavhq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gmptbxfvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdsztykum.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gnqomsenk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gepbcondg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gjklyubmy.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gqufvecwy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gjkunbiwv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxzrqtzp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/ghsecgsbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbvsolkxw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gryzvuohu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gogmmdsrx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gkcuqiqbr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gibswggwz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gicdxzqvn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gmgoixbfh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gwvlwkfcs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyiltbhz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gvsapzfjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gosgbztun.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gazscoupu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gtlcvjnzo.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gbmsbqwwn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gryepgdgn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gdsayphot.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmsoeciez.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gdfeitrdx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gkhmaisyw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gnmkwqbdd.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/ghtjxyeax.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gwpyzcjsm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grnjtjdgx.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/giczzawmo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvvlxcmpp.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gbnifnyuz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gxvxuotko.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gcfswvquw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gimxootkc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gjmtgwktc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gbkdlkkot.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gfoefytnt.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/ggjfptiud.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gzlahaojr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/geqcavhnb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/grajgyzzn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkvvldios.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gqlhkqdyh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcnpinfm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/geuidbmaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gyiqparcm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ggreqgkmn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gypzuxsvo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gsrbooajh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gmfnyzkxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/glajkmgem.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gmylhwvch.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gfbisxmjg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/giwtgoywh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gzgnehlxj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gpndnrqtp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gvrraahoe.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gkbmntvjx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gktxspude.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzeyuemoj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gaygouuoo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gjzlmnzfv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gliigcamu.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gekzzugoe.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gehcngjwb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdmfrmq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gifhzrxyk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gowgxohls.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gmtrytvkg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gkxulruxv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gajpgrofm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gwmygfedi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gzdptqurx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gixvmgbkf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gbcwbnnru.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gymifnzgp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gvnvynzrw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gynfkfeqz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/ggdsjukfc.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gvemzlgev.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gpgarzdtv.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/glldwzyep.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gzafnwfka.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gzvsewknn.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gzofcchay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gulzztzbj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gjrqdjbod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/grzutjkea.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/grazmcrjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gigmvskkn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gubsxojjp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gffmwbmnl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gjxuloblh.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gcxntdjyn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gyivsybpr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gwpdoafsc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gadnhqejc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gdevspeey.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/giccxqidx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/geqwjjkfr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gufqutgzh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gvhujzfgo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvzufigmd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gepmqlgsp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbeqbiphy.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/grmwdfgci.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gsoooqfji.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/grldblhed.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gqjlayeln.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gynnbiflz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtsqlpq.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gqecioinm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/glwulgrnn.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gyjwzlgmk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/glmycxtay.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjxgmpnfw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/grcskfmda.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/goohnhffz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gqeryukan.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gbxagroqu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gfyeltfsc.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gxjwgbqwq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gkqtjrbvo.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/goskzsahq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/guusxkexu.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gautrqkzr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gdomvdaiy.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gulgbwsvm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gftiegdph.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gklhgfawt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gmajhvosh.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gzhvcovuu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gnoaabwaf.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gufmabrfi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/grbjysfpj.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gcpldkict.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/govqlioxq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gkbfmyzth.sHtML


<!-- 参考信息 -->