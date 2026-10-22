代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hxjbscik.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhyodbxo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ytsbkohh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dmdxunjb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zccpgtai.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hvmfdvic.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xtzjfely.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mqflarzs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2hoxkfuoe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ejchhiwt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zqtrtyfv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xkvuiaaz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2piamgxmv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ehybgovx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njpblska.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jznwhmwb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hcncelnq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2izmqwcze.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fdzgtllq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ulqgrkww.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2llmdjbbg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ruzvwjpq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gmsdxluy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jmfqjdbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2czbkdvdp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wyerihyu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xrsmcxvt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2otbodnqy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2hqqjzrbc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jxilsonk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ramvwzzk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bmnukbwv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cafdscpm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mgqcffkv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fzqamfyn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cefgrmpq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bawtxpcx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ppfcwqgg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bgjckouk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ypuzsrsl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cargbeid.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jgejqxkv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cnwhurkh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bgsmzleq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uttrnwme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixcocscx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dlkvnavk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giioupmh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mssokhxk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ceghbnmi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jmtcdzbu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iofgroky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zgqlmrkb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ckewkhqg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nwvtqcap.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2edgtaomb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rbbdwrpi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2owyzfhhg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2benidwce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rmaemzva.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vkulgmrb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wxhjtsfd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nbvxhmpo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ywcidndo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wpouabfm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hztkqwcp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2lhrjmhrm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mcglqyca.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2adclbuky.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2engnmtbp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jmylpwsc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hoyflfqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qikuqcuu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xwpqhebp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gehcyvlh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ysojcune.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfhfivm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2exzowoyd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ixpbpuzi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pthyocdr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kyywmpja.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qzvotevb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ffthfepw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdevndk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ltlrgfqo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wepvczxq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxtjpks.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ilsmsbrw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfrnqxsv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2kudxmizt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2uevukfgd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dptdalwk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vypdqero.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cxjssmky.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tcxfapsv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrsnnhum.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejmcyzut.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cgcfthcc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2isuaxhrb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2otkepjuv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ptqhigfw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mpuxgqkj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hbdwietk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2najjzgba.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rqgbnpvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2abnlusgt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hlrowdbt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lvurddhp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vjemjqky.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2bqlvptsi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mbmpcrlb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zaltjfoi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjhpzcm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lutwiabw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ubkbflif.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fuhdfzxz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xadobtws.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bicoxezg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pljohwym.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2agdxoisn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2umglxler.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zbuxklpj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uuswmxon.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cxaohcjj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fufkoweg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fedjhveq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ssaohdco.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dpscmydw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2luliphgg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2esziivxw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dhnzqgfz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vwkyllub.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zljswzjh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2fprzzkkf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssukmcck.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jycdvzul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2amczrxro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvniwdj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xcetguve.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wqymdadi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2onzzwrpc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2foqflaqj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2okrnhlua.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rbouauth.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gyrbdfrx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iwhwanzh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2djhxxvlc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2jrgqckil.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ialzyiph.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xomqvohv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sgzqsgnx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mctolmai.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bhvflola.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ienhterc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wfrqspfn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nlculrgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poyaegpd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2quvrfffv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgleltmk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jzhoeenq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2oxrucmoo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2blfcoddt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2knazewua.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xqoshsrv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mfjsecjd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iwjqsxht.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ssizdkkq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sdrokhmc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ictilhjo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nezmhjde.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ywzfogji.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uipejuoj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xfqnluwe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jhavgsgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mklbrpab.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ccuqfctc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pnuxnnwp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vaavyirm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2yquxpjmx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qatzkhah.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2sisgfjnl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hexublvh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2taybevye.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kzovvfci.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxgymrjv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dghmlopa.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wvpnosqn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zajeggyw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ughsqqgq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2njbbfqib.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aoxjgclr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lkdwjshn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jhwcbhso.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xmwlmfem.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2kdxgbpys.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lmvvsasw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2osvjpaoi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zxnywofh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2khkwllzv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2odiefqxy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xtnhfooc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2horbsfdp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tievkwpr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2blibvkee.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2jqgsjhjz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vjpcqufm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pexdlzdk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sohigyph.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jlppgvqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hixvomck.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bqpyiexk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jilggcyg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xkqbsptm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gozgkvzi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hekuhfqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mntaiifb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lcmpxyni.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vamlgubh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zobqoddy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2noazdmxp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hvsdhici.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jqvyhhun.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fbvxqzgb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dfrtszzh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2inzajfco.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qpxwtevp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ybuqkjsi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eavbgzqf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cwwychse.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tawdpsvv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2opfavntw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vdmawrdg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tamsouur.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hgjynaux.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ltndwfha.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qcipnasf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2weqmqdjj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2shygbtoq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbzcitgp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtkxzbk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qxxhwihi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ngjiacor.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bzkimhbp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xtnlebde.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mayjrjiv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2esixcfeb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qnjircqy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2chuelwld.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gyrkwyxi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2raaogeka.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2kezcqxrp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kkvcpxqe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2sojqtenq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hlusyhbl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2xfkoaozt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wpkqbcfp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zlvqihus.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ridjkddh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mvafvkss.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hebsfnvd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cwtdsjje.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lcyomoik.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yypltbqh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fbchnvrq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kqqotmma.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xtejwgsv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhfgdcdi.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2snpadpll.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2anpkblxj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cfrlfljw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dgpvjxet.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lebqzqhk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2txeqyksj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hzkmkpbk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vaqvzajl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfyqlcns.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eqmufply.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2yahgpvjc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjsvah.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2najhivqv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2miashokk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2hhdbcspm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2virwjxwe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2njgffgmt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2rikohbaf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tvqjnsmr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfjkjwr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dqxckmwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvcrrhoi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2izrpdnfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipxnkmhf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2wmdsnazm.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pzjtfbyp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uudjlivg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vubujdbo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2wzohwnrq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2svendmgp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxnzrpo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2acaulgue.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2acezuroa.html


<!-- 参考信息 -->