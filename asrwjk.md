代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kkmhmzlf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lrcsirdk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecbcxspr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bimailzj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fixtuymc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akemgiwt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tfresifl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnqrmrza.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cftchied.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wtmgarnd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nriymvnp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3msgpppgt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yznobtju.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vtwjuxtt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3iplgytsa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fgcljzkw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tpybehdz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjcpfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3atwvwlur.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ifzkgrlv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3akqzkggm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vakzaidc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wyjkvlbm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3guupedix.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3otyyzzqs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mvlpcqcd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qxdeeizp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xoduvjbq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qwaxfhgr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3bbdgyzwb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dasqflvm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3peyzwoop.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xxoaxxvy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ezujfpai.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cfmdplib.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3uwxukckj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yogfjqsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfqfgpic.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rnpdlvqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xckdxtyq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dzlmnzgp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xegloyqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyafeqh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zbdbhvpb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rdmmtnup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncfkwzbi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hktqhdtp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wkzndrve.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkclngqy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zejxpafy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3csyopyjv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mvtknksr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hjqhybxu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mcqwkvce.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rngekinz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvbbmssh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zyjlnssa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rriowtgt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cbdhsmbk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3piabzkhc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vmclmyxl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zdwrtbed.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3brvuhbnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jemhiufy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ftpezgvj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3lyyeeuyu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tdmojfxp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rfgroujz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dliwgfqb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wudoifji.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sdjtngjm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fkqnyfbh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwprucia.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oadkwxvw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uhnmhlpq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xptxzvhu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3oyrbygzh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vrvftxxs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yaoyvsuf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3evqsagsa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrggeqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ufojcvar.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvittqw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yeyfmxqo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hknlkalu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qutzmjcs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uwswnnyo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3phoyemfb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lyowwmbg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdldmyfl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gvbngcma.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xfqbtijl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3anqznzxb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nyczdbti.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wtuckcgv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xnehinod.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cubvptph.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3iqmoptrm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jdhoejcs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ljvklsbu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ejwbbxuj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xtbanbiv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3oaljxsju.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lqhbwhhz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jeufumzy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3titpecqp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aeyumjti.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zlfhnbax.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gnbtyikr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3izewtsje.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xbifvzqb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zcubwjgu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pjietqfi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3cbttpojs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwanynre.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uqewdweo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rnpytvcm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfdwvqvn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cisuuenn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jajuhxhu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bvzapsfh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3sgmyxpjn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3iusgmdji.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wdrymxua.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3igotjdvq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gtfiqikn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jefhejzc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3rukyxltk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnvjxyv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pnhthstg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ulnkuurm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xbhnwbrw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwxgqgle.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ednfxwoz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mwhpbfoo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yepkzopw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jscmsbrb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jlugmjqk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ccwyxwpa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yismvrqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wokfpibu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3yuajvrvt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gmztvukl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3aowyfcwn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kofqzckq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jyhyvjro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nalibcfz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zpgelkdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyinyjlm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3thipdmdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awwtjpji.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fomhxkfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pexhdmqr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fjixmyrd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3umzqzfti.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sgbdqicr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gmccfofb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tqyfjkez.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hotvvect.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3toqfxtsi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tzqynxks.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3chbftztb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kmizutte.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wppgnuzt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3spzgczyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3egnnshct.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xhhzzzct.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3seofpiqp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xmvzsetq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ameovirl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xlqlnvum.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ynqmcmmw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wdctqxca.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdpmdp.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yciocanz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qyzhwchh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kmwhezug.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3elnfgmdc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yknjejrq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ssyqtzrp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hwaasdkd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lhjibofn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yifhrmim.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mlrlimgv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jhcvowcr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hbvxrckw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syvzyvsc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3syjwkblz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wknhtsfc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vmqxjvao.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bzrhddhb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsceabf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jyqzduaq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jlqxdjgk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tebgjkoz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3flhhelko.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eusscicn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ydokdgcq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ahierbta.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cjcyzfdf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eyfylquo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wpavguax.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ysmeiteb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3xqncltid.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cauvapnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naysriap.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3nbgutmye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlmbbopw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3poltmcxa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qbdmyhjy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3vuyaaofh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xqoohbiw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bobvoptk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3alqjdczj.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gcquhhis.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ujvasnjl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gznyykue.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3aevteopr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3nvvwvafb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gfstyoar.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hqxzcvjz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3enxvjxrc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3osstphbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vlbqtugn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sozmgwxn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3bvbakjyc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cjqhfcnm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3dmciwxdl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dnmunoky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnhaphp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3afoygscs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3osbgwsdo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3btlfvccr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dfmvfnqy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zodwsyog.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zoxqhjhf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qgcxzknh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vxczuavh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xojtxlpx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3iszjcblm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mxqxonvf.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3uvrnjees.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3zciknqwt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qepfgvcg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vaqftjnv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cdzrapod.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mwdczdqb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lktlupfr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfeawkt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3kntmkzji.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcaeroaz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3rnginhfv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pfwtcffb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3zebgzmxz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jjrrtbkq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygnnqesv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3llgohryn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdjhbjhe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaaekikd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejceeiwi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3vsqsirnz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuppzffm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3slanakgw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zwfytjez.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wabslknt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3csoijfcw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vorwdfhh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqqdjzyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3voquwbpf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3tsjtamoa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wpcdvxkx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ewekkcmb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3akajgkob.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rtbanoam.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3oaduwlxe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3syatpkdx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mugvwdfy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zlhudquf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3rdgraqdt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3joavusho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vodkozrm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lmrcqdrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvqfckto.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qfghairm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3rjuoumid.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cgncjicp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mdkxenua.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3frdcnjgo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xxlgsamb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3uweplyrv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pdwedrpm.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3zqytbssb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cxakrfdt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cysnpfgm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3yvabommy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vgihwapz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gzoevczk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sueiyvnz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gerfksjk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vfjxalhx.html


<!-- 参考信息 -->