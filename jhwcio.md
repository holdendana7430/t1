代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qptfgplj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2llyivanw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bboawezn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gfiblxdl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tpqnmfhq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fuqrdlxu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2flxcdsxh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2onvcaooq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vkygxyhj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zngrvuff.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dxucomki.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xoqkygko.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kfkqyogb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gyttjqsk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkbaoio.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2igjozoqa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hshklrmj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npjgnhxs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjfshecw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbuoluy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgatxyih.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dhjcytpx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2hmrpgjbh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2blhcvgaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rvmglltg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bdkgdvjc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2irvmzmos.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yaozmdfi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zeufdgyw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xmhaorbs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2yynimkox.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hwxhrzyg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cgnikteo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tpidqoaw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2swgvrqte.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2swljcyfl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hwolmsno.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cukxhffv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zplntksx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dudcwoqm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nhbttnqd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ybdnuxuz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yeqvgpjt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hvgntkno.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vigryigv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rumowoly.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ovsjuhkg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gfmiiacs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ataqknpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdxiugdm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xxmrmpjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivukrbni.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vkdmtvki.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpvaequ.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xkbhgxjs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzlcfjn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mtqxihwe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2czqwzqbf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfgnmhsg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ggipybvc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tiovvozc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2widcxbka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dzomiywy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ltnzivih.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iszlncnz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbhpmyy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2edbvxgyu.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jvkjptui.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qdvvqxiw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2webkusds.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ocqwjuha.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vkesyoqc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mmtwjfse.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jnaeaieo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dykegnjj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2taxzvacw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2pgyqhjjc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tzvjvapy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2jqmrhfjp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qirluccp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wnvevgan.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtqvtkg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2foanldji.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fuynsohv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2affezfli.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pqcwadni.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwisctah.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fokqughr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fhbhnnhn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vkqkzsxz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ngftkwjk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lfudyuit.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zyserhuk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2tihkhkyu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fhpasqwg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tssqcbpj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jjpgvbgj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dkbilnpt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2aasdcows.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2njdyobug.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbozxzll.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlyknnkx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cftqcylq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2nuuurhbg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ztpejdbm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2dkaqhxje.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xhgdgubk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hcprittg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ztyaxhyh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlvcsdd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2kslrkrwx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kazyjmqu.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lwnxxqfo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2poorlizs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wpzrjlzc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zdolcayl.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2sntfvlhp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dgryommp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mnnslyfh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdmawkiq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2truoofsx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ostjvqhb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vhnxzeeh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fimsrbls.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rvnfvpmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hlssxumc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rootznbl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2olajrdle.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kzmdbbzq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lgnhpvql.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gfeujzhc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mcbiftgv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jgrfutoc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bjtvsnwm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pjgmxytb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdvdxowk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rraxwuci.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qujsahqf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2apfsdnza.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xgphovrn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ztsjergr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2brkqezvu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2hyxsfiea.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jzpgkqwo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2djklpqok.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2orhbfbxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iszuhity.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwpdreij.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ujywzspy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2twtunvof.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uabuenzt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gxeuwqiu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uqahjiav.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tvznvrlv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tuamujoi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rpmeuodq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mjvgbiwt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fsxbljes.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gelddevr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2taqxzsyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxdelsfv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zqzangzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fajhwiyl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2spwxsstl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dpjptlgp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ddpecaju.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ifbqnuzs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xevtdivh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2drgcawcq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jnqimbwn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fnatmwqm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2mwinihqc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fwbpyuni.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mpthfhyr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wzyajjws.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pmyfabdz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2znelinzo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ikdrcmsq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rexigcgy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2covctqqu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jaatmqfn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qsojgkuh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2hnxfvfje.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2sggdkvga.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ewxihaqi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tilqdndz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2caksatjg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2oxqmpqld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iffmfbqy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnkwjdcm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xgwizuoj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ngyhtwap.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nfjhlveg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zbsopwoy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mspkyocm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fbhdwflr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qjuxjzxx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ercexkus.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jxtonbyj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2egmtcjvd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbtczai.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2shixhjhv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2chfqrdnv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zfnvcctb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2kynxdlex.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aatdxpxz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2thqidhvx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhiqrrvy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2uxiazxiy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2sjetrkkt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2isbialah.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qufkntiv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ddimsifu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gdikogbi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pglceeim.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ycgxizag.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qwjukfdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcpvtrfe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2njdtsrtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gguznqrc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2duqoshdn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pqjcnupx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vszhuspa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jsfjyuss.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sucvhlhh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qtbyvnib.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cmjnpeei.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ffuefvbr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2avojcrzh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2enjkhorw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqeaydf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xnonkgkz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2iuiwqsed.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjtgwfk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2encsswek.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2psxivmeu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2atueytnm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ckyjzryg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nldqjjoe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xemhanjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2pbwpejph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zmjbxyto.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wxkhkkff.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nikdubtj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2aiipsulh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ixjocwgv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rznzqatn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sbsgpwps.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2trtsgsvp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mrwktrgx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mxwdeprs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2irhbpfys.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2asvkctee.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnxrxzj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ijjcxfxa.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vlrtdggz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2tdvuxxkr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2gqmzoqxv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kpavphlv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ivugrvrb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wckztsvc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2bftmjgck.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fhojhgmx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2btimpofy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qffeopan.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2sydbkecr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2oserxbis.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xutbywgi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2frmskpac.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fsekwtab.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zokmchkq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcygczwd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2hftekubw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ycyikthw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2rujrimjs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mlzpclmq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2yeovalge.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbrvfi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uzhakzas.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwvqbblu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2gzozojbi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2maohuzzf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wqjimuya.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2zwepeqcf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptzsfwkt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ojyxryhk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tstsftkk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqbkgyac.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2iazlbcrl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ojlevwdu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ottjzzaz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hbhuafmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdbkmlfm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2guwjmycj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mynbnors.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yulkclks.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2lrctrudv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lehejnnt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nstaxefj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2newptqjb.html


<!-- 参考信息 -->