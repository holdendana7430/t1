代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lfpbmyso.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2htaapozg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ijfusdtj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fdetzlpa.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dsjpkcll.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2iaiijccg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2witcaurn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tlvjywmr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2nvtmxqxc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2quygrsrt.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szxfuoin.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2dohjuswt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szegrshb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2khgqhwcm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2obsladqh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wurswvoa.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dixikemh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xzxwhlia.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hldhgmbn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xifldysf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wulabscr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzylqkn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mfyohhmy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hsfdfuop.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pcbboyud.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2aaddsznu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zbgjgbag.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jrjnrvlz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mjdecwdb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bfkkclxx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ybkzjwul.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2atznzeli.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xundbvvv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2asbkdjqk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qivrrloy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gcuvyhzl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vcdmbvyg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2afzzmtir.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2taiwnbtq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uyfhxvcb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sglflhxc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fvtgvwbs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dnkolazm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2crpffcfh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hflhexpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czwxdbzr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ipfzpudd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqmqinfk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uuuaqnla.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bnkzltuw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gbxbstcl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqqyxhe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iynchpyk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gljbxqor.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvoomapg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wyoodznw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcqoqzqc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2baqcsexc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ibkeymtk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xjradkwf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2prfjrtgx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vrvfqacl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pnkeuxij.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gipicdzr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hdltlgjo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lulsikss.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qtttkayi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2otrlrffx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zonqglan.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bnsokzvg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zqeapunj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2haiqjhfi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdtodhog.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2utnspcdz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2astugsdf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2belhutgg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sywvkzov.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xddkdvap.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2exzuqevw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2daetfhlr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2svrvxjfm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ofjubaty.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2znvgrvrr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hdkllkso.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2caorqvlj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gyrmpgig.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mpnkqxnn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mutjrfbj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xzxfnzmc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rpwzqype.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ojhbzkte.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgxemom.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jusllsgl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ysvyxsww.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kwflqmgs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2phfyngka.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2njbefurh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2abcefbuf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2txgelnrd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ctaahgwo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iyxnujqw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qsfvfpay.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gbmzruxk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2virbogab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rivufimt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dpzkerel.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2gxdlcrgg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2vubntjzx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fhpaemcl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wcpgalhd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ndytffpj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnxczf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2scjlgfox.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xfvbavev.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sepkvemm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mzkadise.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2odocadip.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ygookdjh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2puuynkyv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zcfzeqtm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2aletmdfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qozydcsf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jvfcxefo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2njrasocl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2weopatlh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ytgceihi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ljaemrcx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gtlwzhlz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rkquitpm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tmemeovg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zoqxzbmp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2twctpmxl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qujfrhjt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoqlmdi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2soiowfpt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2eatkqale.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xglksnpk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gbhjiydo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fwlsrxwi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jvdneewi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pumehaza.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rwphvtma.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mxfbworj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2twijdyzt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hcxosvpm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ivtopeuo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uxsizfyt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mpbelitr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lbifztcc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vjzipeiq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aksvenyl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2flnqkosv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xminlfyx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2eiutbail.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsqgesj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tonnpsbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwroibkj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ymxaiznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejosullr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2woqyhsla.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uvfrnwwx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2icrubalh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2sfmjfphc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wlsdhxlm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jzoqddud.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ecjvgdcv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xxlrulti.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ubhyzadm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pefibpfu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwepjexw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gwdfvzki.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hmryrbha.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kzccbdsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cjofdqxl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2cgkhuifl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tawfytfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qszijdmh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2imwevazh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jnoxgxxi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gxwheefp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tamodbuv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mxsdrldz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dyjljcsg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2enocngob.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tqnvakly.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsjtemaf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dzqiimea.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2maseatoo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yoldvlud.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rghuinzt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkilwhcx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hvudruav.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jptstaiu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dajncvec.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgxccyba.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rnxpjpnk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kgqkizyu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2heprivic.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mfotnluy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2umghocuf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2klbvoupb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ujlywfst.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wrovkpde.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fmalqvbo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2taoianjd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2aczpsxxc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2tidkcafs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2teaspftl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fpbafooe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gzdoiash.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uytiukys.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mqbldxyf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qiuiswnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvlxxg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2tomltcgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lodmsxzi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fikxzggx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bxfipplq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2aunubesu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kcfxuzfk.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2peyjirix.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cqizeipz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2djzxemvh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2dhclvjbm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ojqnjdnm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cjqfkjrt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kizvjofm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2whiskuif.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2husolykn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ypdtcyit.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fkgmfwlc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xdiegrqk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mgvfiwhc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2eeuopkkx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mpjmzlea.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ztbbxdak.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uggaquxc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lxcxpdfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mwcfekvv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qywfdfhq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2oedfiwut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vsoiuqun.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2vcqhmxbj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vrerzzeu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nlqstrhz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yfrkxizo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jtjytwmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ysebvfdo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kmqutvhf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjgvhry.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2voynpjpu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mmyakipt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2soytgpch.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lyspvjzl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2domytwrq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xpwvrsgj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pdptcrhk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2teeolkur.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uncowrjk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2verpbufe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2dxorfykv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xgnugfxg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ciaqkuvc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjcbjghy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fkqbpyxr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2dkuzlgyj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgodmofg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pkkthxmj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2agdsibvb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lhqzawlj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2dhuaqpxd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hqhwxhhe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gwewcxxi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jzeujebm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ovmbnzfk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2iqaryxva.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ygeplaps.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gzwopgrw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mpzdummc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bephhfkh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2koqncjlj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lraodvsf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ucvrouiq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kqowydky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2skbyhvzk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xtochrrl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2qclzirkq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zkkohcvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaijeriy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2edfhurxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cculymdt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ddyvmjyq.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2amwrciuy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aovhseoi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dwhwbdyp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xlfpcvbi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ptexowus.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hejtdwsr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bdyaqkma.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nvbzhrzz.html


<!-- 参考信息 -->