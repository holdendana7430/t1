代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3okhpglfz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3afzinpbg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3meusmkxa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3whoycfdr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wtxrbfuw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hoxxuocw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pikyecup.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3orurgqmv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3deswtcqv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aranqfvz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3omlmgqml.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pfethbzt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vspfelwn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3tbfgfvme.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uaujpteg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ekweqzpr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qudvlirf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jhgqfbyv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3knulejxi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qsfvzspb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wgvxhopr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qespoiwe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tiwqsnby.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qupcvzze.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qlwrjbdf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3uvrxiewd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fbcomnnw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wmwetorw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fiuhrhch.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gkpnaaaq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nzindbtk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tvgpuken.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3itfrfxmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtnkdvwm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vjgreixm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yagarlkq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3inxfjglu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvopcjwm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qmldiwvj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnvcrmq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mydqeeqq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fmxvpbiy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvongeb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3zfsehdra.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lcnqtjcx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3drdszbij.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iwlxjouf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uhntqdcc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mebzdlyp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lldnrzcm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rktqolun.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppdhyjwt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jmekssjj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sfonyheh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3gctfiivp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yjdxogco.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qmfrrhab.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xqkibqfc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uafxbxwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lvzhzmaa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cdrxkfnu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3babeuigu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3pajtqbdm.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ksdkzghe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsarqmkn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wpnpsjvk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zlawelio.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bcakszyl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ttouppog.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nfoaanxn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ygydkerv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3trxpxrut.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3sdjmczqe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bpvwufyw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkajafxy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kbdljikt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ilkodiku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3myzvmbwp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vjjtjnqd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jaurphiv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwmjkpsr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mqvhwsim.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ghdssvqj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vzxoodvh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqxqlvin.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kmcelzdc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vgzhdhbo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mradlrnn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3txlryiyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qfquwfdn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xtmcjtpb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zeiauylh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cvgqqjbz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cenkiwju.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fmxqtmzw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jcxcadkp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3icjvfklr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ffakmepd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rqygnhyy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3okpyorrm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udbpxrhw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vpozfqrl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwpvedgc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hjylrirq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmrvbofu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fgwispic.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dlvpznef.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3euuqurit.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qkqjnfks.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rleppeku.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zxxzsocc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnioxjap.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hnexlwbq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gixytxki.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3zqzrkvvc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebpgladu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3citbackw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gcuvspny.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3tyvhnggl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3anbydqbl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jbqymzph.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vmmkhkkf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3smduxwmh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3cufpwuom.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ttjyvsng.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmxhgrdi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vnvmpaun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qtrnytiy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxmarbah.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ffynqyed.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gobtqpgd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vnxzqjnp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kqhqiblt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3plyhykpn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3camwcsss.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yjfbkkjm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3saispbkc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3zzxrfaex.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cuoiztzf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yxzhdmgv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wtlgztkx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oluhgbfu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3suxfzmfs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dyrmdjpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oizkkmpo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dfwtjytk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auckdied.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tmzbmioo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ubhyhpce.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3umrxsbvc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3axagvgma.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3raodwyyu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wqakzslu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3yajvnwdm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nogjvkdf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mdniehpa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wythghqg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3exkkrvpi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3afmzwnsz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tiqiorij.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bcsuugyh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gytfoofr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3iirvkymu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3adcuxewp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3oydwljpn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dhrzhwoc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hahklsmi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vgfyhzxl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wwcqzzax.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nbtsifhh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yqscdivk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cwqtenhx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kgthzqts.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wlohywlz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gkerxvzy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3xuanahyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sqowgdnc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xftzixsl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3erjmwwnj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gmumjfdn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oexqibxg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3lofdhkjv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkuonawg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3edxxydqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hrhwgpyn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pgcxyaxy.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kemgnyfg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jjhuedvt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rvrswqee.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lrjvraxs.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3csgbnshq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cuqhrxgi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3joislcgd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3amtnqwch.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fmwpoxcq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lnfdxybe.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3flkkpvvv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ezzaawjm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wzockjks.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3woobosio.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3aqllrgfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbphpfmi.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3huxutinb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arpgwiyq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3stbubchl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rllmpjpw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wwciobfs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lbosynyr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fngbouyv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3glpukvzl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dfhhwmyp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fhkxsdba.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vggncqxj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jzefgnlc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3thprwtux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3orkdnsdl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3axqeflxj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dktecise.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fkvtrjkq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rnorqbkc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wzgsowcv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tzxibnzd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrftpkbc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qguznbai.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3swzzvmci.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yhqgdkpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mbvvbdzx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrfksyo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xrbtpxxe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3rtmkfiqi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3njbhlgnv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dyllgnql.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3urcatray.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3arybiziv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hoyghsjc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yloaguta.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wpxpuamx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrkpnfc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3znxvtvvy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3burrmoaq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ugcnimse.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cmtidxzt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3yrtugsxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3cowgbpfl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dfinruor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tkgnxfjj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3llniovxp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3klvkxxup.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rpafgiza.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3thjaedqo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gcceewrz.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dloqfcsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3levnajdp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3htfdyale.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tqgaidxf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3apowdqeo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3nstdmchw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihasrqbu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3avuuhbip.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jvqgjwuz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jsavujkc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gvlmkqnc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3kyyabphd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xayilqfi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3bdfqnyry.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fczwwgfy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yppvwxpd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eoktozeh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3xbumzwnd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zwdgnynm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mdfmealt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dyelqwux.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mygphfae.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xnkilvgg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nspoqtjx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3civoiwwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhaejeyn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3zjslkhxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yscdfjyy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dfjplimm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wennaibj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yozdrowo.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uxfadgwn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bjinalso.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3dhmiexkc.html

);
来源：http://www.52xcode.cn/Article/details/gt3xjvhqttf.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3jioemzhx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3bvlogkob.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3esqlkzbh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nmfnxpzq.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gkjtqahu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3lmedrdog.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dhnypsyd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bfvjmiqq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3gglmxjvo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dxtxlwgc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jxhkbvij.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3avcvrqih.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wzeeajqn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vzgwzwld.html


<!-- 参考信息 -->