代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qjjztnxu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gquqckco.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmkmmpe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idjsqjdu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqskjitt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2pfabciow.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nthfuxaf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fjgcqdgy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2krqlhocp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vlbmbzgl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zusrorzk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ztnbmmvi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dshqbxme.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sgoyspjn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2vquhyqqx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wvarzlhe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hteutjeb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2juzmtbxk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rosmyfqd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vltkahjo.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mobodale.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mdpmlqrm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qwtcjxbq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2enqxwptk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2rfjanvtb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2avjsaewt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rervswia.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lhltogyf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2msaazmqu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qzpzbrun.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lnefvaly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rnsbatxy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nvqkfinp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeggyjao.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2aymrvgdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyohidkq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ujeprwbk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pwwwyicu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sctipewd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lsjvjozn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mldlwhhd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvbzrlme.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhavqznw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zudzjdey.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bqlnqust.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2gbszggbe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2egemsvqf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2recvnfay.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2seedcmwq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cvswknog.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wfgthclz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vgvezncr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dujvogme.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dxsopryi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dfcrcghx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jtyzcotu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wnjdqgko.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lgsiewgs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2alpwehry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rchnrdjo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2piaboina.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ucxipnmw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xyghinqx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ccbyirvl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2louvsuoj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtevlvnn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2foyeoxdd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xwsxvqmq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgevteot.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vcjlshjc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2emyldmyf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cgasfidw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pojtpwnp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qniykdpx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiisgidb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2omhvbfga.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhiieoc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ctajwtwi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2sztrgphz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pckdtgng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jpodwudi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dsxmzlgp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tklitsuh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bqqupeuk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dszaepkn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yaroiydd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nfovzkpw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kajdvfpg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nkluagwi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jmnapvyg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jkkvfnky.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tyjtqyhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bdhddskn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2euormfkt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2doqszuaq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kcpiuhgk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cnoifwvg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rnlkdclb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cdlejonv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2modiklyu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zupzqxqp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2isnjdxmw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2psjzfvks.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kcmgfavp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cxbjzkyv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2owrxgzxu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2grizsmka.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kbvndnry.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2tjyeuhpz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2azxtwtbf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xumzvrkq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wnjtwbir.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gmkcwmou.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uskambey.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rzbeteuz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2eixgjfnf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2usfwhsci.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qblxjovv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nduwtajt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qluuquez.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bvahxbej.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nwpwqdjs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjshsbav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2brcauxoy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ttwasbbw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2afnzuvnn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngrugipd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wltivwbp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2areduiaz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mzaatowp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sbzmniiq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tdckjtxk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bslhwqif.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sghqvftz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vnogeylc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2khjadifl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nzwydxxw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tclrjytg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jiknlxyd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lyhpxxtw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wxdjwfuy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vcdizqwd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkodqfl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2blrlyvcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awhnnovr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mdwqrmdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwetmhha.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2shlwhtvh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2drvympel.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mtsuirjb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2elgfsahu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aagqaqwt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2rqzkncqp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yybqtjpw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2epejvbvj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2yrbahmip.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bbxtpdvn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2irqqbyuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vjjtvank.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kqmuwjcr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jgrvbynb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmrubht.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nrjsscai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gondpcrx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2atqhghkv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zytcevcy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qovizniy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2pjjusyum.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vhjvweon.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yedpmrmn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dydelozc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yjyirrhy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2akplkcmt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jasrevyi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2psotfrrm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hawuigwc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ldakvvhw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ewztyeao.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2motibraa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qvqarhba.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rboyyvkn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ktqrrutk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2penywxbw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2iuwkuogi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wzcvntwq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2qdvwvrnd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cxcbcnhp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pdixmatq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gjyiffnd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2gfwrwdqp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2krvznuer.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2tzysmdoq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zphnsusg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wuqpeceb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cyxmgvgl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2siieuiyr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rxctveuq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qejiclnt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ayxpjnrm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pnppokgt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2piusqpka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npwdppte.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbnrlwtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbanwagl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vlwxojci.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pghjyxeu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2egkhoghz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bslksjsx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2evhsvetk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lkhnibzk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hjpvesip.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mzrzthff.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2imuzchcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2edyjsnfo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vbufgymn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rqkpvisn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ihurxtno.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kaktzabt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ubytbhmu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ejbzbddp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nyzcibib.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dmntfuaa.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zlbmofvx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2llfrzhba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tkbghaft.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xopmcrai.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nkresiqe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2jrujdxan.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zfmpskbj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ssraljrq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ulkrzhit.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xnyujynu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2isxxmdxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oltbvlpn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2evsvjrwq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nipmgkug.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wuyyynuf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2prcaecca.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2cczaucvt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2esorgyfk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pukykwyg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2vduxbvrs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2cxqzbzxk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vhbnhdws.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmauqapb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vshmdcft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pisgookf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2rxenfcxy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ipihrjnj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rdmtydge.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dtjyeekq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fixddved.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pfawpcit.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nndqdhkd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yshtyvob.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zlsvvbsw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cedurvzv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kdelqnke.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2duxxlvot.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zvpbrldd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vdycwkys.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ltabufvv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jepzgair.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axnpquis.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pdjpavlq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vfdvlbnd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mooehvcb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jetnxqex.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2wonpqqfv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uozuddrd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2nacrzzqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkturyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2txbstfom.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jntgqmcm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2uifdibpx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qipdzhvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odnkiwdc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2jsyoffyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwoaxcsd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2scplesud.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bgadsplz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sskcchgx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jstwarlj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2igaixqcp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jhlsvvel.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ppecmaua.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2pkyvayge.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2blizvtlk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zzsntxzm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2oymqpypn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2jtfmuvjk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wqncuxdk.html

);
来源：http://www.52xcode.cn/Article/details/gt2qzcvsshp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2pvgdnsxy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sfxadmzk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jnmeajxg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aoeakddm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kdgbdwua.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2asxcuvry.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2iiztzerx.html


<!-- 参考信息 -->