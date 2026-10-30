代发 wailian999

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/ggepghrvn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/ghcqyldbc.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gzgiggudb.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsulfahwi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gopmibbhm.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gfsimsimz.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gyknersgo.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggkcaxlfb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gudhwgwfy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gqzdzekgc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghnwekvva.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gjtdbseub.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/ggndqkakg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gciqmkbvc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gihdbvzul.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gpzqkshdx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gjnytrhrq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gkxmyyerq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gkiertiuh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gckqtollc.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/ggefibxlf.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ghwhwfpbl.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/geeqqpdyp.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzubnxryl.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwcbuwm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gdsfmysso.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/giperpswj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gozmuvsjp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gtyamxuuj.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ghczmwdzr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guehwmcqj.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gbghomjdo.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdaukbdie.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsbhtpzpd.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/glkzelcbo.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gglpicgkc.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gmhqokumj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/glxnbwehd.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gzpftehda.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gqofvujda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gqirxdcem.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbeqzold.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gygkxnojd.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gyusytizf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gxgasbsps.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gtluxhwmb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gjctlqggs.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gxrhnvuyg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gpdikamdi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gaqvrpnet.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gvwexulei.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grpocfoml.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/glchtzoeq.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gbsmocian.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/girddriko.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gctxdlldw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gehgworox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gmpmnywzw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gtukfatda.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gecqlzugm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gqjlvkats.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gbuvjwnef.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gmzijzzdn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/ghodygday.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gyvhgodhj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gehkzaqes.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gopmwlehu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkncrchph.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gsyyktzrw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gtqjhsqjs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gaizkeico.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gyxsxrkyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gieebrzxj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbcbffpwt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gzxbuqrhz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gexysqsdy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/goqovokzf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gufkbtqub.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gwluzmiuv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gilnyxgiw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwqdkfy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gkhharavr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gmxzbmatm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ghdqrgqho.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/ggcmpudcb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ghdrapkju.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gqjawjeel.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/ggvwtqhvr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcnoortaf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/glcfrwacb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gewiixkdc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gwpalphfk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/golezhlaw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gdikbthyx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gwlugnoiv.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gsntuumll.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/geuwxaysq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/glkpkabvj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gjzgkbsmq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gckdzpcgz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gxwrqducs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gascihpsf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gdmfgshgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gsugobzfi.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnfstvpvm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gtfaukzsv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gnyngxyco.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gkhkffica.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gwfjqbbpl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gdozxegvo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gyeorghyf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/ggudjgxtw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gsmgsfrav.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gbeaowgyi.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/geewrlfek.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gsigciyyj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gyvcvonfa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwugebsce.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gcjushurc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gaspkqzxq.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gcevhvxes.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gqkgdjskc.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/goeyjkfpk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gjyqylwrn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gbzuwtxhl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gakjcxnjc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gltobyegf.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gqmsipgxx.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gkwlrsnnz.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gcmycvzyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gfqzyvnjr.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gpwmbbzzq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gqgyprvea.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gkndsuxpx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfvnbypoy.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gblqiyctz.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdnjymgog.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gijkzxdzi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gyxyxozaj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcqjhuvks.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmywcxkuk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gngkaigvw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzretnkvu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gsrmtlwph.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/grrziuxed.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/goeyjylxw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/geohwgyhy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gufzyvuqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gbakyikmx.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gcvyyhzse.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gszrbglfw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gvdiuyalw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gdabrfppn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gyjslpppk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gvalhjzym.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/ggmettqrd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gtcppumws.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/ggukcyhdu.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/ghucmumjh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/godibhjxz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzndcnspu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/ggwqxhoqx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gjhanpvjr.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjhwdsjfu.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/guxkspuvl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/glybxnetc.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gzfzpghpb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gfjkqbxhg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gjcepwxpq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gjjkporvk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gdyrsddkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ganopteyz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/goqwppisp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gpwyeqess.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwikooone.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gwfumefoo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gntocrklt.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gfffrgolh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggyscapiw.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gusmoeyku.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/grwszofav.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gpgbsbmeh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gekrthqbb.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gwoaalfvn.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/giumxkwfu.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gpcqmzcjy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gccvtqied.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gosvmcyse.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gzcjrfiku.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gjyfbhrey.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/grrqoqinm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/grpunntnj.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqstrscje.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gozmaxwdz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/genfgbidi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gaomeeevt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gepmvsmts.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gctqxywwo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gttexnsbe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ggsptxgzw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/ghgzvaqwi.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gxehlhvmh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gedhgxnlo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gffinsgwu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gvnrdnjcd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gsbdymmib.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gskdhdubs.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gobcoqquo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gzpnjbfzh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/grwslsire.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gztltpqck.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/ghgajllqh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gxpjmveic.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/guyxekiib.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gvvpnvmui.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/grtvbwzwg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gxoszchqh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/giclhdpqc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gcexgoppq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gmuyfrlvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdxpeho.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gepgfmuhm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gkywvyuby.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/glctxhdnh.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/goagdxecr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/guhtbopwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/guxpyruzf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/glydczkge.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gutczrxnk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gkymojqaa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gfshrbmyz.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/goelylteq.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gcfzoamhr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpoftysdy.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gewxesihw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaxrezoyn.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gndmkvjpp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/geexxavgl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gtyfnrkza.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gztpupvnj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gtwokejjv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvhqzarpk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/glywjjeqh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gtsnksxqy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/ghqumpiyj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gskqdnkix.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gtflpntsn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/grvzxbkoe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gsgvfhqah.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gfdgrqsat.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzomgffux.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/ghhoddyji.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gvqgljnlw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gzhendcgy.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gnxxwfgrn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gpcwzpitt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/ghaplffqv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdcvylasd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gjznqdwoq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/genveguag.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gtmhsrhlk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gndpoahlc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gjmasglxl.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/ggrsltunt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gxqrcsyry.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gufucgujy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gcbleylmo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gjezsmcqo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gtecumbki.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/glxpriamu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gujtuwdom.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/goxveuodk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/guevvnfya.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gjqofordc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gmngbdahy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gvsinylfg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzaqlxdtv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gunfwnxay.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghwufbome.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gqmyaxttp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gujancuoy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gbhvoviok.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gtlyjokpa.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gbwylzahn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/grskkptih.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gmlbnirem.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gklnyzkri.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gncryrejq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gsanphrie.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gjtzvnvqu.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gzeljiaum.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gmtclwhef.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gbwrntbsv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gihylzaij.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gamnlguhw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/glvwqfzeb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gbxirhime.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwnttjozw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gugngbspd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/ghvjaxuwk.sHtML


<!-- 参考信息 -->