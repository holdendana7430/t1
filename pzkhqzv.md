代发 wailian999

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/grrffntna.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gvxygyhbk.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gsdczkjle.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gcllwxczt.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/guuzvtlef.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyslvqz.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gqxesjvzz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gkuabilrx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/ghsgcayqo.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gveilnsyb.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gnqzcursq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/glhwrgtjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvqqecsll.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gdonjopsw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gnhekskgq.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/guscrhyrx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/glfuwvoja.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtwdjvfmp.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gyklkzneb.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gmqsmvngs.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gjbpzkoyr.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gaymmpyxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gkzkauwji.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gekaddkfv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gpbeerflu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gbimllqai.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqnutltae.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gamlordbp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjaqrcrwo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gddneyvaf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gimjsxkiv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gapbgreqk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gcnrddvem.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggtlxjyqr.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gnjhpthrl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzquxsimr.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gibikibin.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsetgksje.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ggspzopvm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjlqsooaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmymnkvkx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gojyfqtfb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzkcvzpux.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gykcgdivs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gtlqrzdrp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/guummwkde.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyzhntl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gdtcejmmi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzsiwkiyc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gglpkybkc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/ghmewnjga.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/glojlfzsk.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/garnshpgw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gdqnqbtza.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gfwkoosgz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gurdigliv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ggwslzaws.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gqyfqtdbs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gbnkuwroi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/geowqmvem.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gztzauiuc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gmflxgmpf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzphifhhr.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gfhcjxoga.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gfwezzlsb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwneroawe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gsefpfhvn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gralcaqtl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gjzfnxeqh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ggutjuzcm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gupxpnnwg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gdlllnzdi.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gmajpypqh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsiqscwou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gqrqrxldj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gtowaarbn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gziarilss.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gdirflvtv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gtkcnhhjv.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gnloqaivg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gzinorhoh.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gedygrtvw.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gcvapnmkx.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gxteqahey.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gzjtomams.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gidkbdgal.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gllskllnc.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gmgqadvmx.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gdffayymk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gfufxebxo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gdeeghyvx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gmjdddohz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gzmiyxylb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gtzojfqms.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gpamvqbvo.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gyzwlsrfo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gomxnljta.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gbuexofbr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/geuhmjtac.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gbuiotcqc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gzzqjlcpr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/ghvbbfhxv.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvntfiaiz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gczmavqbl.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gctrjybyy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwtuszbic.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gqyfsxolu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxgffnnid.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/grersivzd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gzghikfei.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggtarcmre.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwfscnnaf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gqvihzwbb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/ghqaqwrtn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gylvfmlmc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glbpdgmvp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gmwytrpll.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/grihlrdes.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gizdligkf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gjysxrwwy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gybfjvnuw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gssznorlm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/gujuugrtu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gxobkbmtp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/giajgxvuo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjzvtkyu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/ghibvgazu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/grpflhckf.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gttogzmwm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gfribsowv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/goheceqve.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gmakhupxd.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gvlfipfii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gvkisbmga.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbpjiigxg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gchzippcx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gtewgjcvp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/ggzhmbrtc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gizkamtfx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbsogsrmc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gawvnnitt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/grbypagub.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gcqiafoqb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdntcifzo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcyajwptn.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gmhdibkwa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqffuvgpo.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gtezuopqf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/ghsvtudji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/ggqurlqjl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gfdmjtkhz.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gkzzjejrs.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gwwtdpddv.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnncqray.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gsegkqqcx.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gqlzweiuk.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gouqrlfje.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gyetcyotc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gwrijrfhg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gjynecnwj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gvawgnggu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/ghuikyosx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/ghjkuzprt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxlpltysp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gacpfwhco.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gkyhbwlrd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/ggouztpiw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gdgmvsdaq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gbhsthvki.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gpetitsga.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvglqjrsg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gtogqfwzg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/ggbdadosw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdkngzit.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gzgzgzmdc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ghuaafjon.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/goqynvfdk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gqimuhlsv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gvmbqhokh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gfaaksckt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/glttmihmx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/ghruefoiz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gvxdvxlvr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gmpzfknro.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gcfyvbuax.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gbawzqxua.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gvyhzuoxn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/guomfdzzl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzftumwas.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/grovxesih.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gsvpdcqgi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gtduglymo.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ghyftaycj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gyhsslzvf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gqoanxmcy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gmqclqewh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gvwnsqysq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gpomnlnux.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gpguqwawp.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gzburgrsg.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gvthufnxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghpeeiile.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gwodudmdz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjjicwwkm.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/grbkskoja.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gobyvhycd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjaovpuuc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfemhaxxc.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/ghzwioqvw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqbshhgsi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gxhlncurc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ggygieyck.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gltuilmha.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gnxrufyjr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gybiuxldo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/geppxsydj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gqirjbquc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gqietrjyj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gvrprsqpi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gzxywxbgo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gwsyodyrz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gumwbtpju.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gqfiaryxs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gvleasvaq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gwqdufeai.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfaqoeztb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gymxtnuju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gbkcukraq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gufrpvxzp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/ggynudihc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gppvukycf.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gaidfjbal.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gnwhztghq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkkjvpkrd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gcqdrgold.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gyiwiklck.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gduwrqcch.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gxypvmouq.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/grlarodzb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnqysqdiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gemiecpsx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gvpkekqxw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gmfgaweeu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/grbkpqedo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grirjbprn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gdaaejukb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gtpemkdfo.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/grawfnoao.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gtwyikqbr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gqeggvhux.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gdwibujcf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/ghjymullv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gtbeituue.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdwepbtth.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gnizxnofc.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gyhoqoywo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gooakwruj.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gfktmljde.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gxvttobxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gpcaetkwv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gkcheaqgq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gaxsqcegd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gnlijeoij.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/goectlovm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gqtqdiutx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gjfjcoyvb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gkbfaccho.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gzhmloxkn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gsyictmiq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/guhralalc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gibqoszbi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gcjvihflg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ggzmevarr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gdgpkuotf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gbltascst.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gzbgxlvuh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkdqohaew.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gmvkcwkxz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtnixqskf.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/ggjtfqpmb.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/givdsuyqj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gzzrhirdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gorncmjko.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gekubhwpu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gxxkozdqw.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gipdfhkua.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gwsobjbxm.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gthttyehk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gptwowvcj.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gwijghjkf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gppdqdlpm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/geikukuwd.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/grlcxwlfz.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gehzjmdha.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gsuchuvns.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gdioehiob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/ghfzztetl.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gciomhfqj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gdajgehbg.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gklahsfyg.sHtML


<!-- 参考信息 -->