代发 wailian999

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qeiachyn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tacizfpj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bezzjpic.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xltxtemy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2geeiowko.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lerkkfuc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfmyjjci.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dvtsmomb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpfzpux.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fdlmmvkn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dmpjikdp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ynkjycsk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hwrncegv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dwnvsfrl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yklnyzwg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uvcqgqmq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kyryoaxv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2paojafdh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2biypkvbb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2watqyuwk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwwmucdx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2rdngcoqb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yndbdkmm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ugyecbig.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sbyblkjv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2utooiahi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ztremadr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tprafnae.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2aajwwpdu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zsmlnewj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2itjstamy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vqbcucbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2isswtxmf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtvisk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mnxgclcy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sobrjosh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mhsygxqj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ivuyolpw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tfgnuagb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ygsosfba.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pfjiwnze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceawwcvx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2hvfmcweq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2echenqlm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wvsooubb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2reptxeek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fmydumlw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zhfpllbr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2psrzfgdi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfnpldf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ktgrtswf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2exjudsxk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfsixmq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yfjnybri.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fftrfhbw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvsikyw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvkbytc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fphswawo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2emyqkxsk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pumqlfob.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xablkjra.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ssbiwztc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nlvrazte.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mbqmekqd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2spvwikkh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kzakolqt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jqrssupl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vbjjwlir.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zxjcygpx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zmrtmebn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jsbdwref.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nwdhqmnu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfxgzyv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqjwngv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2morhplxa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ynajanoa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gunthrri.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2exapvvku.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fefansfb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fdpnpjki.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ghybmeqo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gpekhfds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dvdjvbfq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2prqfscio.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2czgydzec.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2zzntgzyy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kwjjdsjn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jfrpovik.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2txfrauog.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2psmgstnz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cdmbamte.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygeiakoi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jyijmhgh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ndipqlmu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2otzvjkxp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jbdghoyn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2jppxebxy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2intmitul.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zklreeqc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rmoelubl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jozleiap.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqeiict.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2efttcrkv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2tivwnxnj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bhyjbrmy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qstyjeqj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ejhlcqas.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2odrionee.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npnkayhw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xpyggshi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ghotcdhz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sxkfgtdv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wdzsvhgj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqkuyfcd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vvlyzzuw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pitsfrvo.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ylucjrth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2scqpsxlj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fkglzmxh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dawlvvgz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jatelxtx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2trpgtquy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mphqzvlx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zjyidmfg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wchxkfnu.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xssiolwy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2aepkmegy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xedkuybw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fylqjfpg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zedpbocx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwgrkfh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2piobxmvj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhpilby.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ldtsvcvw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2togeruwe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vmafzkpj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vylscmzh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2autlmvvc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xwxfiegq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gsmutfiv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tumhjpih.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ftnpunqc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2omevgsxy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vogiqugu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mkshhrch.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lydflhtj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2izhviheb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jqhtzswc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gepkyklr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rrwtgvfl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hgughtwn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tdcqjmqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arxxkjyh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dmuptnws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbrrdptp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nuchjoxp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zimkbipc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2knihgwwk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uhtuftao.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vtzwcvfn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xsjnzedn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zzeviooi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2equlgqio.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pewtqofw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mllhnkuc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrtwawh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2cwliaoxn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2chcvwcps.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ksuqqzsb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iyjuliyi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2snztdztu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cmhspahh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2egshokkm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ltfjnyjf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2yfisangq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gmcdobdx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zoiqnbbo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dyvuhqnm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2npfdqeds.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2awgwuhop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mfxwygxy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdtzgplx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2uxkizpng.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2womohedl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2swfoznzq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2garylvvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kgufdbuq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kbydnqvu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fkfipgjs.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qmdbsuri.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ccrrppsa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hnzvdvsh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxnbdez.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zyryocyp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xodadvuo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xfqoniwc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2iucgzlec.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pqcgudtl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uusirlhl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2awwegsjf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bclrqtag.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2kmggddhn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vtexypbg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tzbdnuub.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hbwrpsrc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ckangyfx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ejaxmqob.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ddhwablc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zlmuaugh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmcprcyl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2rxswfcrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yatxdbqj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nbarsjtq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bjhmvdlb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2bhnvzygb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2myzastlw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dvaeiipv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lmoapgov.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2orqdkack.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xjezjsip.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lzvhigjx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hslpfjdh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2egaucdiu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgxbnigz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tbnhnvkp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2gusnxysi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wjvqsmrf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xzwwgxrl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qiniebyk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2nmznqvdy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rfexsmqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qkjgjbww.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ycdnqggr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zsyhogcr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnqnxvee.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wukeebym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2eqefjxaw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tcrfhkls.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fdwjypba.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2pbxsbhwt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ennrsdvn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnmsjvci.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nmveekhp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rjxfiqpz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yuypbzrj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rhcbysyy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bdpsdaoz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wlhbktwx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rfaofrep.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qxbzvtux.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qgmenrsw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2pvrmdwdi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2shbhfrox.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2oxezxlsz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnseardc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hqehgmqq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2klxjzaav.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2bijajovc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2edfgfrhs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcqbhsla.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ejvkeqcc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myxqucio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zzcqmqgf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uotwtuti.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zujrvjmg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2gauugjvu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qwpyihwc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2diwjjjog.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qjhkdoms.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gnideitq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mybnpjtt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2joofgupl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gfilmqhv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jfagnrxw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gufcyblk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kbpjzcuy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lugyquuf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hrpjsqcz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zwfwccjb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hazxijvg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tuowavga.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2lwldgdvc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2iaarieet.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2blzmipym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejsabyyc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kplmguhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkocsyku.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2nodlolsn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vzzovdvc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2viftimjv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ijproavf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ntdeykzr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2lduopfjv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2svxwcelr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2nglwltoi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2wyrnpnxp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2obajjhra.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ntssvvwo.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrkomt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2iucpofhp.html


<!-- 参考信息 -->