代发 wailian999

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/glfgmjesg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjtlcavhz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gjyusyuvn.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gwlcsqxfj.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/glztffpho.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gllzyvuzg.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gjqiihyaa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gqaibcyfd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gbraumkrb.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gujccrbgz.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gfolbxzzs.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghryhbmms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gawdipssx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gudmcwawu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gzfyxxafp.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gjgpcvzdy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gczboxwpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gxmdseazy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gbqgbqsxz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gaovkapkp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gnxjndcsi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gppkkhzsm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gftamgtpo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/garlqivch.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gvpjnptwr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/grcvaqyil.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gzwdimsug.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtuovqugk.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gvjtqmnvy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gvrceavgp.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gaipupznd.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/grfqecxmu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gmaethhet.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gyrvuildv.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gekpqslts.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gasvdvdje.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvggpapmm.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqafoizfi.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gshyptebh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvngbnneb.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gmrqhambn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gbayutygr.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gkxrdavzu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gyuxpfkej.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/glmrhsvrh.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gsvuxxtxf.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gmffqisdc.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gmxuejlow.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gtdkdcrao.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gpornvzez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gbxfnayso.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/ggmmfcrst.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ghzkurosg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gjmfduhio.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/geuzjxtys.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gdxtmuqlp.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/grdqqfzrb.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gxvytccyx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gzrkuhtiu.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gtdgxagkj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/glpvonnwu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gifvxyplt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gtthesefg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gucptmvcv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gvbkgyztg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gprrdeesz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/ggjtcimwl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gwozddmbf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/grhzinvhy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giyzimick.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/givbzfzcs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfkyyaopc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gjakiqmjv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfwjdxaox.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gxypgvbin.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/goiecdmvy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gqfrleuwc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/geziumetw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gebncmlar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/ggvqffmyh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/geiqjqjmf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gvlyfuuhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/guuyoyfus.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gdniaeeql.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gsmrpeccs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gyoflmjxp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gmitzqjgy.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaeoaeyxf.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gazghsfxk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/giuftakdt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/grcvjrpht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gevherzbi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gzpplmofm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gxhprnvmh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gnzavzzcp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gaeufzdoj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gizlvuhuf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gryfahwtb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gyalcpegv.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gnflbgwic.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/glmfnmjju.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/guihertvm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gkvgztuid.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gaixtnjxk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/guyxbiwvk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gxqokywsl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/guatcfucu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbhwzwkmc.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ghzqhjhmx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gbznpntgo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gpttkgrdk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gdxtvtgxi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gpulrsywf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gnpacnwqb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gadeuipvl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gxoqkcrgf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gbmxlgpfv.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gqzxqxgva.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/ggvjddesd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gznhjjjsg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gchxqytlu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grrzbeesj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gwdnblkdv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gxuyxhova.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gzdggbvva.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gszfrebbo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gwqhyahyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gibozqtwc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gqahrtdwl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/godzccauv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gprcuvkep.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/glgxbetpe.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/glhyaxuwr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gmcnvulzk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gdhuuzhat.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gvzeoitsd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/guwizkxiu.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gqelxtikf.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gowbgbdoh.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghpzlnpge.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkfciimdz.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gumbmimeh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gkcsuvwot.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gtyegfnog.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grpimlpbh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/glkfyqqmw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtckxgazl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gnqkokcii.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gaxufdjkw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzquaxdme.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gubugexdv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gsckykdwm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gorzvqvlk.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gnxmtavgs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gxbhwchxe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfptoroq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gguiibrcg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/ghhczalvv.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gcizaxnyk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gtritutpk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/grhayclzb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gxnhqdutf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gxhwrqdzm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gpkmplitu.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/ghvlvouvd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/givvruwqc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gszqzforn.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gkdacncje.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gwinqwimc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gwvfsfsad.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gqukxcapy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjiupza.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gayorokhq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gosmuuqru.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gruzrluol.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gjmipsumh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/goqojgusc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gmmyjhoyo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gmpqtxput.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gjxatccht.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gziwztnvd.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/ghujypsin.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcahbmfcr.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gjnpmlpxe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gwzzcncsr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gaxqbemhf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gkhmslbea.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gloeviqfh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/ginbqpzjs.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gcqlqugcr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/ggiyaqcvk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/girhttoco.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/ghamshpao.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gxismmhpm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gdnrzzzbl.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gbxsdihxi.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gaodfnuem.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gblpkfkpz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/ggavaxqae.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/ghnrnxlvy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gwhltzynv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gwrtejdye.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gcajmbrlk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gifklixgy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gtbxtzvza.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gsmterrfd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gwgvdkwhj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gnweyeflt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gthobogmc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/ggbxgxcqw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gydipbyqx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gojdnioei.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gteyxnjoa.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsdfwvupg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gotcwxcjl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gxqcvrzno.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gagkymbjw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gnnarambn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gpeyhxdro.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gpzixplsl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gddnhvlng.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gxcvcpvgd.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gealvixlv.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gevxdwoat.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gspvqdeca.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gnphsesnz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gwftlbgux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gqlhfqgcc.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/ggkidbfps.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gyxcvdjze.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gshsruyiq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gbouaghgk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/goghdyhgu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gpthgipez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gvhvdyrin.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gnyzihuhz.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gdogstlgf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemoekkgv.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/guweenfav.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glstmlhyy.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gmnjjmnjy.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gdyifhpor.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/grltylitz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gpmnkpgui.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gebqfkjjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gfvtmcolx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gzjyvfxjt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/geldnczgz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gvwpubouu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gwhqsorko.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkogrysi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gorxeucwh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gbnrkhlvs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gniwumwin.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gkqyrjrzz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gwjwmydbg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gibqdcaji.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gkwpeogrd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gvtsbotoc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gbofwhpid.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gaivixcqr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gyeixdunp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gwbxywsln.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/getwkwwru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/guznbbtfh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gtoeogelz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gkflooptj.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gfmmgqdat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gtxntkvdq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqeblmfuc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gdylefinb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/ghisxuyxx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gejoiwzcf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gkiifiquv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gnnhqxhcj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/glqjkwjxj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gtwunmhdg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/grkrpblla.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gqoxgxfjk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gczujhblq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfrzzbdiu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/glzmwlwjt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpjlpoosu.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gurnbljyc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/giasqczyo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gmnmgsjhe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gnwrcchvh.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gwypqvpmc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gcmntxdli.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gkchebxri.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glyebpbwz.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gbbyylrmf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/ghzwfjrtl.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gmerukkif.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gsxvfkskc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gyfbnxbbc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gqizrnbms.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gcgefmveo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gnctvqmtz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/giltkmkpp.sHtML


<!-- 参考信息 -->