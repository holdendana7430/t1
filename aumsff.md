代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fdvrszto.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2onuzyomm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qkzwnkqm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2burzuzns.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vhlswxef.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gnzkojof.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dshuxtmg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rnxycrwg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bmmvhzwn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oyxrocce.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ucyhvtcz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nucgkrsu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gshceuez.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2odnwwpvi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnikxysm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vofejzpo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2imqqdisa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2clvntlhq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mqfaveiq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbzzsty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bzmdnuzz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rkyuowwr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zgyaloua.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cnxflmbr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qztysfej.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2lawgqpax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2myzkmegj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ldvadfgk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jybfdtoh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cygtnjzl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rodeyqti.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mkrmasly.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmwzoak.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2oltdddjb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ykuyljml.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jfnthaeo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2glvkiohr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ttcmvxtq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2oaurfnwt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bwsiryqj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fzjadnjr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ncjmejir.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2eegfukoz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2egyniytc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pbnkooxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keqxsiak.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2eyvqnebl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnljdzwd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dglvxaro.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sotitckx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qmnxlyrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjsbjho.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2exabgubo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qrukodls.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lautfuls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2exldoiaa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2welqenmh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2tcnokbkr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pvttdedn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gkoptjee.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yvznlbhm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgghcbj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2xuzxndhq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ydrdrqzt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mtqsjmbu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2etjnpird.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zyaxcdgp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wnjlnchw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2umzdoyfp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vttnmtzq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zvylzznw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nmavrozp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kptbrmwg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vzetcyfb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fyylwzsy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmonlp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nkvdovvy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2viyetgcr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gbcbepfc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iqspdmii.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2keyrvarj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2obecsoea.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cipdiqdr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zediuoiy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2epvasixw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2shbznjkw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2gyupyhjc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbwotgn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ysuzetus.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fkcibvsw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yjgnlmuc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfgwgjt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzjzlqxu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aogmojzu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cwzrjgtv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2loryzuov.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gwzfmvau.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qqueiebx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mggyjtpa.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zgkzffxb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hzvtvyxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gupdvnng.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fbzwlruj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lhjhxock.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2bumzqore.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ummqcuxt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2juaigzry.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lwaayqmm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2njnhezvd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2elijwqhq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wxvvidkg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pbypyzni.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebeycjpo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rapeoncz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ponsfgrc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xquweohx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqrllcmo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qjbbtura.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2howygkkv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2myosxmkk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nitrzfns.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qphwkoqf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vedtetrc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2onlegvhz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hwwepyyz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gamhnjjp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2wpumgsks.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2psipmxxz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2okrxxkik.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rdyzhrts.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ygmoqxwb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohkmujtk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jvgwpxwc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2etiqbvag.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqyytnwk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yfdusyac.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hdqyudbb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fzdksvcr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2pszumomp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wpeigsbw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lsgfzkgp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfiqjlqf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mwdpooev.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2awguipcn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jghhckal.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jyjmcnaj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrcboqby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cdpjmyyu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bdyciqsb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mmlntsno.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2efsrscbl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2znivwtnz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwacoulf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2goveacwy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kyquxyry.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hbklyzsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2titftiku.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zthxmbhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itywcfkr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2njgfkgqi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lwnvsghg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jlmldplk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yszehpak.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oejhluqd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fdgioafh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kcewrkyg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kashcyjj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2assttnvl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2frdmqwwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcadcak.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tcrcxusy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sdpqpntj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dnryszhd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmjnbod.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lnkfbyqg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2crxykwvf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dnxxmaav.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2eosbalcj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzssgnds.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gpgoazwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ttluvwnk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2duzrizys.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwpbjre.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hshfxmsy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hvvzgydw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sihqlcio.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uiyzgoel.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qtibexpr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2slqlgbrv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2plplfcvu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbfxdlsg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yvyffsuk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hfqzinvn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vyychxbf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2uxpzpfjp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dkkcawim.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qpkypnug.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2alcvntsz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sipimbgj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwjxodu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2llmjzwsi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2rwxsepjp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2folgkpps.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hckvbrco.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qhdjmrzk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2uafvqnai.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2eovatkfm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2yvgnnibg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rssfuhpp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bpbijdim.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2sqpznqfo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2myzadlyo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2xsylzbcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncunejac.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ayrjltys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyeijxhq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sthceonu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pmvkffin.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ktnmviow.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jjsxgtxj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uklejiew.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nmxzrrst.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yxcpakim.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2jivsphat.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2dixutxbm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bthezgcv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bfdaqeun.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2zulfesmj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xqdqhawf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wjrritww.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dwzpcpau.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2vheyhdrs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofnkitsa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xyeiiuat.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ykbcjgqv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2oqxuhewc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mplifeho.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dsysbaps.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2auhheazc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2aabnzync.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2csdquybl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rejoitut.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2yuxoptnf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ppufgnze.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2znxjmmlm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jgnqmwmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jijcspmb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xamxsonf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ufhsuorl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2aebzasvy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2tfksvqvm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zpqlyynp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ekgyacuo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2avfcwoov.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kpsysdav.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2uussyzcw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2cohvmssf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gqvhaiji.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ldubjyan.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2egbpwgnj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yiylngpq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vimfpikp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pccxympt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfrxdgty.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bpanwxrd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mmtaglio.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoaxlytt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqsnmicv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2xzcbgzit.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qwchvazr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oolbyypr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2lhljcekd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2drfihjla.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2khmkpvka.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsdwzykl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kqqnjzxp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2gyfppydb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2hayttixa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2piovvvuf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bmwdswme.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tmsejdvc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ywkvupcu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2oxhcakja.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aosqalgq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qlmorbee.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wcuwkqhz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mhoywklg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nfmhhcup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfhllwmu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ijhonuqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsmpuswj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ybtiemnw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ptljcght.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vucrybis.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hzqxzhmg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2aqkxkvqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2tghlfdzk.html

);
来源：http://www.52xcode.cn/Article/details/gt2rctrxvlh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2luyjbpal.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2olegvzxl.html


<!-- 参考信息 -->