代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbotyim.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wdwchjps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rdkbvhvr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jemvsswe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3bbxdbbka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3stsczjlg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hkngjddy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bzhxbimg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lpjicrgi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3syetrqdi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rdtaiejy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uaxvijgt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tqljynme.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xrpurpyd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jaxzkgao.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cegcaijs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qdmdjazt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dnnsbbrg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3decyuuao.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3flvbdxjb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ipckvbgd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3krndobmd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynnbwjay.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nanimftu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fquzccpu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ybsbckou.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ausbkcax.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jksnzbyz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sreoiwjb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uyvkwyly.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bjqsgkzg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxvaasoy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nynigyfy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zcbuobbb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3sjuufoke.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gnijprga.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fyselosz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pywhkhbz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fjpisnxf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nvcjbxjj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sznvgqti.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vimvpugi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gpmywfwu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dcrydyrc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3usmpndnr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3hocxmytb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zjxqcrgl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cgpynwto.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3infhrajh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dpimrwup.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fqmrcwln.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bumohawx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xqhkdfpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfqbywat.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pltabyuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpioebtd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mzqoikcd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3csmolozr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jqxchrbd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mtddcbdg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xfuvzghk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mksfwipl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfpdzjkd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xmfdxtms.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xadigexy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jtxqgjao.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iuzxalru.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3tblvqnsl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mquwruyd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ffygfgde.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ytthqxuz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzodqthg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qjkpnrrm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3uiawqsxp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qgnppcyj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jddzirrx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nstlaxui.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yxdaabbq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tpardsev.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wjfbzich.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fickwjnn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3tyybkxci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hiwnluaf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ofjlpjgp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckbxvqbp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvzavoka.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ubisugnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3orhfuvet.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tqeieuod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3norivndw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvuiakhz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kfzfolzs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3eyukapki.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wnxxhmfi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfltujn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bpvlbigo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgbpgkxi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yxqnnoej.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3puwzkeuq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3azlrbofz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3cjkbaagd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lbrtaesy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vlihcjpt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ivpadnaf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfhlyhds.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3witzqylf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrwnpj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hjfubuup.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tskdehxy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xwbrdjxk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mtvtdude.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kznciqnd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xbafizez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wqenjhwd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zuqynxsf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zonypbbl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3njaaqxio.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zieyvdsb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3utcbwxke.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ozotvsvo.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsjocexy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3sosxnzjx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3muftcbqb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yquieuie.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qcatjoiv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cahhvnml.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xuapolin.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vpakpeyg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ryltgslg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hyeeuobp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmcastji.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tfmdoymv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3elinezmq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ehltftet.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wirvjcrn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vcyitope.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dwdromnf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cgrwogzy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fbosuxjh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjqvqdnq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zsasccnz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ankqdfxk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3edcqcnfj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zcaxvhkw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ukprawbg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kijmrwnc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3facpxnun.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3esnrlajf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3hsiyizta.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nctobtfm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hyyurxvr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3trcjxjav.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qzmeiwpa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3mrykfjsv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yeltbyds.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rhpqxyqw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fjiltgmt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3trddqudy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zfkxdmmx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pnztaofq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ofeyfcvi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3siqatvva.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pekuhsto.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jfwscqlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxztdxvd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rqwikxmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhyzgvdz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3olbtbknh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mwxerppy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qvygcdsj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mguslzxz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gvyczbku.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3conglyln.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3qydsztva.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3abkxlkbq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3uifeetor.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sialcusm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3axvvgchy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3luxngzig.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iodkyxku.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zfszgmyb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3kzikcwhb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hthuwamd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3olzhcrnk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xzecvbgh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jcvmmifd.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ikqvempy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ousfeizq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gjhtrbsg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ouwjllfa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcqdnkp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dlvmcrwb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3obgchyvg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijtiosca.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3irvajqlt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3tksciqso.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gyzexthk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fhwjjtdw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3flrgpelp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qgsykkit.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3sbmiyjrr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3arwqzdcn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdtpuem.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qbudnftl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtjbdta.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tpzjfboh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxczhfn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hbrbsoyg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gapydilq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mrgsoplo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ynnprbwq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkihceg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gbfczmds.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nzxusmla.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vxdavyur.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3picduiks.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xyhfjeoy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xyibjeiw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ugbtnxni.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nnksxjvn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3sioduxar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jasnkmlh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3wryicpmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nirwgenk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ucirxhaz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ossupucq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3snvcerbg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xemamnej.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gsemkwed.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tyblviri.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nyprkcjp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gbxwazrx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zfaneixk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qgrtzczw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uqvaqhct.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqarlma.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oookcfss.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ejosfphx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3oaazgzbo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ejdhamcs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gidepqcm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dbnywucp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdguqjrs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3minkiapz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pgaxeyck.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3glumwxkr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jbrezupm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcerjsus.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pyfqygnr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3quzxejiw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3icndoqhq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fnvbhbxt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ccvpihad.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yumemdwe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3asdotaae.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xgzyzkrl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dbqlgcqh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tymzzypr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3oacwhmdx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tnpbojap.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hqtutvet.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zarznpgb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3drxkbslp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3srvktsez.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zrrhmxmb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lujuznsh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3icivdrvw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3kuyxlhjk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ctreubxc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3iglznktr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dtlyfusi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hstpdcgq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3rtsikyxk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vozzqrxw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jpknzuxe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaothpft.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tsaggapk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3lnvcsdjm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3brvmbmkp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3auutvgfp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mtvytkbm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qvidekwv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3udkzyvlw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3usuxmryg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xobmbvzi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zrzsogow.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tzbiliyz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3xkchqptj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cnzkxxba.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ermehyss.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kjknelpz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3obdgepls.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qwoagxqh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qqzkpyhn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3edplllnp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3bvkdjypu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asrsbcvv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vbrghqjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddhzqedz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vtvqosho.html


<!-- 参考信息 -->