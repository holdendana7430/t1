代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2flcvqnwl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qfzaugys.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2caksrjka.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jvjsphdn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tquzzcfx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rhhvxfvq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zdtubtdj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omyfxrvu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ciyuvpdd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2evgozert.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2coxmxsbo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xndyumxn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xxtpxtki.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2awurvskr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lqzdktxq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cgnambdi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xuazcjwb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tqosqepd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2eftxomjr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tbihkfha.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2htqmuzuv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bdnmyzyw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qliprwwf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iexwdktf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqicyzr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rmykkbdd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2lefwnvul.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2fqwymvga.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2bmjazlev.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cibljgun.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ycuouyml.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dzygfgxw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ombjybun.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2khylktra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ngsbmiya.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ksqrcfby.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2baczucun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdcbojsh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qcszdbyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otugotry.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2itwovyba.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fojtrvwj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rgclvafw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zdwikvig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ierfiasa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmkhjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bdfhwyem.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vncszyzr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2souyeomm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2aiafaasm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2unfpulog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwncepl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ogizuljp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpyyigpy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycsjximp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuvnbst.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2osiyltgs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pbooxmvy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ybewdimx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2juybwvqp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fvufwtng.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nvzacayl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xfhecuzb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pwtfmvbz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xhetotlt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wkyzfxpw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2feskqetk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2fqcglayo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aqpwsvpr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2edymmhek.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yeuawmhf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hriaahln.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2atiagcql.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dpgpddyg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ljfrylpy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwbqpkru.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ogtjjazl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikqmarkj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iywwjwmg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qthypofb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ejetbdcj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jdmqqfmr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qlgnsqap.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2oevxoljz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gzetceez.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rhjhwnzg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2exnmupkm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jcdlwins.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oxpdtiwa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bkdfezrd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2niupzfrc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2toeuhvgj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oksqjjro.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bcprimgn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2sdzqsnss.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oeijhlkk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wlbhrixr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zyporimx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ogsqkpah.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ypcpmhtv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dqzqcvoq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kfajnciz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yqatwyda.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cmsbgvrf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bssqxlkm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2atqfastn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pbthnxbo.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rteevqre.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pyvroweq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fhxffmyc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2khpmnbin.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gvssojft.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vszsefpu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2unnqhott.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fahlpleq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bnqpioqp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jtaryymm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bxcovrzl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qpemlysg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tfpaaomq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2glcjdugz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nutvcbia.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2bmxcafhu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuisckgv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2exqpobzy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2sfedjpih.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryftepsu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pujgzuqu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xeayixoa.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xafswpxt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2jxugtjll.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ujfipmsb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2fwmshycg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ppypvbtp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kshsqizl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2foldckxs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fxrwgwmn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iimepdsj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dnppjnle.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2oszyddph.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ihhqibiu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2vfvcnkni.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gscyvryx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pxyljpyl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ckqnvbrq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2eopxrdxn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kghgsvla.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wxxcnomn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwobefiu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gneuphjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spktzhuw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2djnzdiqd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uihakwsx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nuzqkmqv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2oiajrnon.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ladhnqxc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2frwjceus.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rvuhddfy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2lpbfybnt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ftssgsrw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yrbzpluh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpxuhlox.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2wndxwazz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wzuuykvq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2phacneuv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bsqpqpar.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2tpnexper.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lmcsngku.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fcowfuok.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2trmvrsnx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2rdkvpmsl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2goothxqr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jmsnrgno.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wncddirh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dhlkxztn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tkpqpnir.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lecorxkc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kbdzwbnl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ssbmhgpt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2essygtcs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2skpfwrpw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kzmjmboq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qenkqhin.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tmtnlroz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2iwbvqjua.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2twtxkahw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hpmehjlk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2exccvkpt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyttxaw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2obrnazae.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tlmfqgsf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gvbvronu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vdtiebuc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2oategzgx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iqurgnnf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dazhiyfp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qaivpyxq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dumolfas.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zjofcrag.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fxshextj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cjttksje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dkmdrtpp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hlinzurd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bxvtnmxm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xsszixdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joxuulwa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnmgxrky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlzyfffa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gcrzlwru.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wemclnbq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cdztuhjt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hsjiudrx.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2grmachvm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zbzhykqu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ktlryntx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2vfpqtsmm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wldoukqi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ceznrsox.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tjxcjybk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xraqafrp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2izpzossl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nkxnqjvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbreood.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sfuhsbwj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wokjeufz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2snubmrjm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jeugshmk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2upnlmguy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vundmtwx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ipfafzfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qfiflbzw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ngmckyaa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fjcsdhhg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rwulwggy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ukynmfrv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgsakvkk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2askhwgez.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oyszvbro.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ughjonua.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2zheaoril.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szjygxdy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2klribbed.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qjpuzfvq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bimrmzsl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ofhlmrnv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2sfzijugm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tbzdbcdq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wmxtknml.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjlpxlma.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2azwgppjg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfpwlzn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fdtuipst.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kfjeuuhc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vexsgfkg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ulidxdgs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mkliwqjj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2npmcdcsl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzmiakns.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rubxumps.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhnogioo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hnrrionh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcauqqos.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzvauz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rjgnyryx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dceavwcw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xxajodtl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qpabjrts.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ocemtbhg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rzwnelac.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2elblnult.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uedbmadp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2trlykadw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2iumbuhgf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ifashkbg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2umkutkrr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jfdpenfd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdazmf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2nemdsyfb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ylisuqwn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vnzcocpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rniirjbm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2myylopgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rigsjtqx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2recescsl.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zdkmtbwy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ljltttwh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2eyoxgbun.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2apemhmdf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pdcdqlai.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xmilatqh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2cicvywvg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2icezuids.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iehxqxfb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kbqozmgr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gxxolxlh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xdruzoqz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ljcodhex.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ebquuurw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2vvwgkmpo.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2wddxbrvn.html


<!-- 参考信息 -->