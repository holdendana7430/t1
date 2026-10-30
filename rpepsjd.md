代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gqovwxoiz.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gfvlnxqmi.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gjjhuypkd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmbocwkyx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmjpdnhtj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gjyxymlzj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gsxgtwfhz.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/ggydeicbg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gfhpwbykg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gqpwbyfbj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvmvotela.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/giwotecro.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gxkatpjep.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/grvsvjzkc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/givxnfdxp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ghvoaijkl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/grmldglwl.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gqulgqqkc.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gpvduergs.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gayzjtbiy.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/ghqikavwl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gwohtwwqc.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gxiaehqjx.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gubavnrcb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gibvlcdnq.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gysyqgceg.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtbbgmejq.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gcucianlp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glgsyjnfy.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxzmljsuj.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ghlajbuso.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ghrmsykpx.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gbzxurhvi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/ghiiziydw.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/ggxuqpozq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/grqvccnte.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gwdqikcad.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzydnaaem.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ghnwdekjt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gjkqwjyxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gmhjidtji.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gwnvjzwbh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gakodkcig.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gvxpmbega.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gicfyfqwk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/ghshllxpq.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gzzdiedmu.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gmlertxls.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gmeshofhi.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gfwfwlbts.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gtraxzhah.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gnyckiynf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gnwphdtzt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gbdmimayt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gsakypyzv.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gfgoejhbk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glamyzhvt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gfkuzpykm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gprrkdhzs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gmvpbldke.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/glnmbdvra.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnmoqdvhf.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gubamlimi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfkofspfa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gskygwrcf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnhqjwijc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gdkgrnjed.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gquqnsbhr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gtcjpbgco.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gkonllkcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkrezgmmi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/geflcyjtl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpqcdpgla.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gkkmzvifm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gwchasmsc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gbtabahyu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gqtxqoglc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gimqvawal.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gwlraboup.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gfkruylvr.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/githbhbrm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gnxkbnooa.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gxwgmxeuq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gffeqwquv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gbgdszbve.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gqwnzgvxy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxpronott.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gmbycgqcy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gjteexcpz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gzatdylaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gfviqndno.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gbdmyiehw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gxkwuhttk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/grogjfrns.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/guzcbxgjx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghxskjfbk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/grhmikgzd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gmjfzoodl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfhpntlfw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gjuminagz.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/ggaqsxsvw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggnbsqdek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gemsxilhi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsborkpt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gijvtwshv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gtkvzltxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/ggialgrji.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gfnffezgc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/govcyhfar.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gayphnrre.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gcpecdeea.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gfgptweqp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxtmdnekb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gatmcnmbd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gmukelgdt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gurhsgkjt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/giuiuuygo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gkflqtkej.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gdlxyzkic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gaqrzsrjt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gkzsvrgin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gezhrhdvx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gyqhlsswf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/glvcbhlte.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/guxpfvxjx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gbqwfzisd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gusduxlst.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gfhrpkhdj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gypovulya.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gmmqpbqyj.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gniphzetl.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gikffrsgb.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gbmvbgoun.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdpblvtwe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gicnhorrh.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghuckgsbh.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqqshjata.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjxuldvll.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkvxxywev.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtkcdlvov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gzcmvhvae.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsomkoioj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gaqgzsakf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcycgikej.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gzxrvxjhl.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gpfzqsyyq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gyodqckwh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/giswnjkrp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gozhmegvj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gvzhdtnhy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/ghddrnvrh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/glcgfibpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gudbvdwit.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gkymfzrkg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gnszqaazs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gapswbjit.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gwrdszpof.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/ginzpysrr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmwowmvux.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gebuvjrgn.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/ggugujxfz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gssljrooz.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/ghvzwwbnz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gatjpursz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/ggdczkyab.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gaucldnhg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gjhlcadhk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtjiwxyxd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gcllicjqj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gezgndzyp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gfdyplurj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gcjjgdmyi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grdimhpih.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gabygccri.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpdsjdtof.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gzfoilodi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gdenxxbzf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/glwxgxzkz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gwgfmbmxj.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/goajccpks.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gcrisufqi.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gorgyyloo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gyoifvpor.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/ghituwdew.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gaejavqxa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gmnbkvnpy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gjyuryrce.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvdfbwhru.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gobclkflw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gvnlmamnr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/grkwhjlky.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/galrsbwbt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gazartzij.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gzmvmbqnx.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gcmtkytwv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/geqxyybxt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gtrdxrgly.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gjvytngts.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gfamaplsp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gjflokvot.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/ghhtittpe.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gfmmqoepu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gwyoxngsx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gutjyndrk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gdxvqjymx.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gsklhavzx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gzqqdnimm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gzxeqcxfl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gfvfwyxur.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/glnridvgz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/giohcukmo.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gjlngglld.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gmbubemdu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gngkrujxv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/ghoxucdgf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gdshyipxa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/govwjgvqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gdydlausi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gwddfaknl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gsftxjasv.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gopbkmwli.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gefiynben.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gbhbdpset.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gjankdjyv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gcwehwpdt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gyfffuqjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ghoyrxgxv.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gnrxrevvo.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gcdcmgehg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyhwlggsr.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gyshildhf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvgmocqdy.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gdgdgpuiv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gimjhbygj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gjyhugsjq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gixyoaxrx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gahgsmrat.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gyiahehaw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/ginfiwfpi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gihystpkl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gkgvxkzpb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gapsxmhhv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gurieqlxe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gpixglzoj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gvewlfnhu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gbuawjvsp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gzrbtlwqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gavvnsxhu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gjhctbwtk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gjcckrnqu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwbqsqvxn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/grczsynaa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gjhferijw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ggnazqicl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gxauczkqv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gpntnhvdq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gjkuitavk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gczdunirq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/goqgnngrp.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gtheuyjmp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gfxkdbjaz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzpvbbzlf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtsbjuaoe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gojgtbzwv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gpdzlewhd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gmfhvwurg.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gpwubijeg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/ggcmemikk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gdxddaich.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/ghozqyhny.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gidgdgkdo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gbyolnbwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gzwwehser.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/grqaofzgq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggdkwifhe.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gtjiqyeix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gpgnzetum.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/grzormsee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gbvrqenqt.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/ghldzmlpd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gydjehhru.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gwqqnsaif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gmhmbhqch.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gpyjdxalm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gwtoninzi.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gjywcewvl.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gffzlnlup.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gxnehtvpt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/ggwnrdyeu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gaqunotnv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjknnorwc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/ggpwzgdan.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gmtxvszzo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gmmoaqdjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gparvfmvn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ggnxpvyes.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gvcnxgsde.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/galfbzkmm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/glbjpjgrm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/giieyxxhx.sHtML


<!-- 参考信息 -->