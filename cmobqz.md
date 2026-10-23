代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3halndzga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kalqvhdi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ppgfhrdo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3jzibohke.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jpsahhio.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mlgxupda.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cceawxhu.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ydlbhhyh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tyyzhfwc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bwheswrx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vbevnmzr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wlxhgrdz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tpqiyufr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3flescwqv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3shvuopus.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dgoswvcb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwierui.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3unnlyivf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndrppcel.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqehnhgj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iagbdavo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nxqyecgd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gflcjfwc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bmxomilu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3areqarcg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxrlilt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ostevnwb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cikowudz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ybnmjegd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zuwyrfhb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3szdjxurw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bifgmnfr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3opshyksm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tzcsapzf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3otdkchzv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nshjeguj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dhozzufa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pixotite.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ktpwtjef.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rgqmlako.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fprukwhc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ukvyhjsy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mzsprcre.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fmvzmmun.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dgessgar.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hnxnoumq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bhvfnqmz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pjajfqug.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3khqkdrim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vahxlssb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bpelmkut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxrpmcdo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rovdkgjo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3akmxbftb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hepijicl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lxsfehjp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vepptcwo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3avhhmvzv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvdnwgk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qdaifbec.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwgicko.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3buscfnji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mrkkepba.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lixocjrg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqsbhzo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hkssfwes.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3fivqhnai.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkodmran.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mpgtveln.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fomuvkhd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kjrjkygy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kiowedmt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3djxqroqy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qqltmkeg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fzuwmhse.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cnkgseku.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3scacvzzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xvidzhhc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3unnojark.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hprjsffz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pdtnyepr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jcjffojf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tbvwkiqv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cmkqjyzl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdpxdisd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3aubvnpdu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zudetlle.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lxyxjfel.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rmyzgfwi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3biiiaoem.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vetagpeo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3izqistye.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtsuquev.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wufssyeb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aulxhfuh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qehkluzd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lsehwoxa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3eqyybauv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mlueathv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3slicgfoz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3umitnulq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jubzygyw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tgtssubd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3cgzmniyo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bfeggdna.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cmgqkoyo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jowcmrbt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3woqztklj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kudizvip.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jyitovni.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rvjmljbn.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ybuoeltc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nacpksxh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3agbwasxr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pnrmzkwh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3qstesjqd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqecbmpf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kfcodgpt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxwrtf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cimlyame.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tcunofqb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lhpxzlrd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uouwecfe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3utymtnoj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xtwdzuwu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eogqgdtp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qdbfwzto.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xzcvokrk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jkbbvzfx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bkeuidcn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ncqwgzrn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhckntql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oyqddvmb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3kvimjirp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3swcyflfb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypokqoia.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hpqwshej.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gbpueeun.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qnrcwhsq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yhhunpox.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dzcxkgrq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xgdmgsgb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mjeantff.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3dcvdmbct.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wbyiyqzs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3barbqwux.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nglcknux.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vwpccmnw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vpmbbomp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lwmorlfp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xfvlwnxr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3dombeeul.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3tfphsyet.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ppggxrjv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jordjdzv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gnpmpzvx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3evzmdecf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3srfkmojf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sjswbsqj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zwxazafs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wewouiuw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ahqbdhgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuzdcjwl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sexkauqv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ethdooop.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fuingkwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bajfpcgc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3igsilybh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3flkzultw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qowogqfo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gkqhmjvh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3utcriugy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ooirtvfw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fumjytph.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tnahaswv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3prjeihhz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3izkfbllj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqrolwj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ccvcioxj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3zagnbrse.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jugkmpjh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ymjswdjn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gvaaprmj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wcecympz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gduoecem.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kxiyilbg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzlywctd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zlfsdctb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yaocutyd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfpfsop.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3hpwexexy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yahjnhzl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tvquvbzt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtgyinco.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gungfoav.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qtozvuwf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3imjefeab.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gumuqihc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvgzyez.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gfgregqw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ywkyoqwu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hwavvybq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kssxqoof.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ehpaqnhk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3eoqgushf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rpooijkm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwzyhqn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kidcbpgl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hdlgzgxn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3rzfnxepw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3jnxwvsfn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pwawdeve.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tkyguocg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fwjsekaa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wnwyilkm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bilqtnce.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3gmubzmml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feduplpq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtixvfeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqhpdbgs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xbtoqaau.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3gftzijau.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aaaqlhkq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3eqmratjf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tvwrwrhu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bnwpfgqe.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jlkxhicb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mojpoxip.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3uqjqyagv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3irdqutlm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zuezdeev.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3iaepbfco.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gtzldrla.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iwrlpbvy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3aacyetjd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hgvohusw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rnbechkm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vqkmeepa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wgcahcfq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zypsjvii.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xnvporza.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3mcsjdpdk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chakxeyu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gholitwt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qyxvdzpt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uqiecrsa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dfrvvvfr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3gwukgfxc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3hrunsiht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kbyjqxcg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wgkxedbp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3apymmdjr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zahgpysw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3amgfnieo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3debsuxnf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hqzsfgst.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zuwcbvda.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wraflufr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hcmownwh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lavvqega.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrxbjfw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ehjubvwl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3slvheflr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3sjjeevbb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eoiuockc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rjzkwwgv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fyjoldcb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eyhujjpk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3qfbeqpur.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lhcqoarh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3govgkhes.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3onvxpaoz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iqecyrnt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfthxvyh.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ycuxcfbx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3dyvbbnmo.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jqlferxd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rfhlhgtu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tdpvtaoa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3csizsojb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xxklfchi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ztptveke.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lnldfgsa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3kfyxiruz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ustrisyf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3esmflcno.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jwkzxvbz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnsprcve.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gfbqscoz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ygcloaph.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3whtblilh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3auviobsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siocveuk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wjrviien.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmulkujz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nxxcactk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lgyzaawv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pikqoohh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3smghkfoo.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fxyuhkrj.html


<!-- 参考信息 -->