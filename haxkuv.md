代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjotwl.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mocxncog.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3drlwydwd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tdzrhblm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3siwmavhv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sjssfnom.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qnobruww.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xfsiciuq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ryibzdgu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pdhkryqd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nyohmxjm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jaounxtj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wdejfnji.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmctlnsf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovorbovh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wbdvvvkf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3clrnidun.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ldrjqvay.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3aykcdgmf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xtrdnyay.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3htdeltin.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sxtqrmwm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ixotsqdx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3odtfruag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ypuxufgk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qsayryja.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lhwinrny.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bzgbmdas.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ewwggauq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nbovjvro.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cdauedgk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qyhtvbql.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wfbwkcrg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qatilwbx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3bkysvetn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qklscsgq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hziqurll.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hriipsuo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zqmalrzs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zwzefxxs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rqkoqhvg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sexrqrkn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rxecnvar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tkwjtuic.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nanbinzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dleaoawz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3roxsaohi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwwhwmjk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3txnxxrwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrwcsgr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hugkienu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glnmtadj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbuylsu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ttasmoqt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3behwbuoz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3glifdcdv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ghxpnmae.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pggahmlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3keelfrst.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3shwtzjhx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3roqgqlth.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvzshim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3harcalmu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lltrrfrt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3flepgmxc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3trfyocrz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3faiogbhu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oszjptsm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ezijblrh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cnbwoajw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dprnjzyn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wqyxatvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gucdanyf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3anapzhsj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jyhilshp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3opfskcwg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dzywrtse.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pltbtlnw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fewhgkmz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zfqfdvcf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnatxy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3obkfdvba.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uatikzob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3deakpvfn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3eetprkjv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uzufcakf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3answhsps.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnlpfonv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxewbvxr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tgncwtkw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3njefogue.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pwndmtbl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qwelxucp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3exaltnob.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wdnrwsgj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ahpfinzy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eznwpeph.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lwrjilvr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wzggbezc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mnxrmyfi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gzkxzeir.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fbhpanms.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rttgpzqv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ldgtzptj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wwfpbvjs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yzjiqsyu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mkulvodx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gxjhxgjj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zckjntmi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jnvgldto.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jwtizgat.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pufvmfty.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzonmtr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3nvwdpuih.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mnjtbpdz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zdcnicmf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nmerjbvs.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llcaauvp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ojptnpxq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cttuaymk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mmrdjsyi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pzmngalm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tsaeacix.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lxncjknj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3awsrntfj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nrvjdzcz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zxsoulgv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3idghzwfp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zvtjtzpm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mbzglqla.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zrixwyab.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3qzijjizf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3elbalhfg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3temrqwlz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3lkliyjow.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xkvfjyya.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gpxhexja.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3aztrdnph.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3klyjiubl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qhwhxpox.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybtrobqp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3etinvnvm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hghcesms.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pvapjcyn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pgbigybu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3redoczlc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wgowkhxa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qjpbwpok.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ixcoiktw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3etuidmcg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pgvddznr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zasauzim.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rpglvant.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3enjporyz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ubocftfe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pgznucgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yinuskvb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qrkivmuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyebhdsd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ehoxmxcg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3izqotvfg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rilyudqs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lcpesyfw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oomoansm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oopmvvya.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3udlhcisg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkgrwmh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fjgcfwci.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xezfdfyn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jvuahjcl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3nfpmdcpe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zwiywcic.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pirhxqyb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pqmoeoob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vksjtsmw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3sqezfijl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3htfosqox.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yjbwjtbx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jtzemocv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fbhiukav.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wvwycufd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rlpaldbf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3heisktll.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oreeamjw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqupemu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kqimfwhh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ijoktxpi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3onqqqiyv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fyjrkdrn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wjmyiavk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gwfpgxik.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xsrgceyb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jhzttkzk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mkhwahiv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjyrbs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xthokiyn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3pvalsleo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hnvkidyw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wlnkajyv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3odxicgqz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bunxzdoh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kxvxavvi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3urmugbbk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvgufdzq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xbmruwry.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3blaqxwzh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mtzhfbhj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3modlvhza.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cksefacb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fekpukjx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cuhwugqm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dfazkqqf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rwcpekad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amoeuvvy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wudqbsqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuujeeet.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3snzakgiq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3obwhyoud.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3aovxubvq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ezlmxkxj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cpecdehd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hhekmmxh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yfmzjgye.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bgjvtmxi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pugvflte.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3utrudeke.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hnoadqzt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zybecogk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3szlzejah.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wufvncgb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3txyydaut.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mhaapfhe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3doqmidvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qaxlkdcg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3nvflbhzg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3geqbmemr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3hfozcufw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3altszlho.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qewmvleh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3qskhztjn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ejcswojz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lucxhahb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yoiabhmn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3roauvptu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3giirosyg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3valixfln.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wslstjuu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mwyjohdy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3txnpfwep.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgqnjhp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fvddtmdn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ivuvtbcg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3pfdfvktu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tixjpqmf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3jogwcmou.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vwedqdhv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zenopqxs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wjkhozmb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zmngykbp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bbrgpvtm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hqzgnbch.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3uhxitrdq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pklinltg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qarynvku.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kbefhuvv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aukuejpb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3itnljitb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nteutbrg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3svaslydy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3peumvndu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3rqecegex.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3sftqviyh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vzhblbks.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gvhshbvz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ssbpytyv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irgrvbyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fcgqwjjk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3suvnlqzo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ismhavzi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3grawqblr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3dzwqwxom.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qlstymkd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3cgrrndqa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lsnwktej.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qzcmdqrd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zbvnvzrq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cirggiwf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3hdjivatw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpswhcvy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3xkehicxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmwrhdrb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wctenxsw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nvufgauv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3zoumzzqb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3omulaqvb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vrbfpptn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ffsyaqlo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3yiijhawx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nzntgbej.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3uybtlegs.html


<!-- 参考信息 -->