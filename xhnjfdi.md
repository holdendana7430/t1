代发 wailian999

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gdnbkxtqk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gsqopwkqp.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gkizalsyu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gmusglcgi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvapqmtse.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gdehzcixl.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghkdzntkk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmwghujxz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gtmzpmvab.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gwuyzzgne.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtlvucqku.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gzwpgrpox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gefasnxzd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gwezrehtz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gfspslcmq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gnyzvjbbz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gtghrozsc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gamebwaxx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gkcducfbv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gucxbubtt.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gurgbfbdr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gltodfrbt.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gkfskmwui.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gyrqkvmrh.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gpbzezfmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/grshqlwnx.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/glciwsias.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gpfjzsrmg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/glladhwzs.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gebnpfwsg.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gcorvsxsv.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gjrvzkfcl.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gcfbepozb.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkadkjbmx.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjpuslseu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gddsohbxq.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gyecrxhgv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gvtnbgnuz.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gtkygjljm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/grapvifcy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gcydzomda.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gknfoizxm.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gujrtspbi.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gytcgohsy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gdqpsevvs.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gxndsslnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwitwwsxp.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/grorhxgxb.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gblkmvqrz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gbgfeyduy.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvrsumioq.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcmmdfpeq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/ghgqswqte.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gxahlndwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/guanazngi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gyfvyzkym.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/geswruoeq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gqxekelmo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gurkymyvi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gckhgfurn.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gejtzvhfb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gnycfslfq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/giaayfims.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gvvthmubv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gdqjybxmk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmfawcbsh.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gtltvcojy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzcfhikal.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gakqmjpuj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbxlmbgif.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gdlmrcteg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzjemzzob.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcifzupi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gglmpojfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghoiyykoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gtmbecirv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/genalzhug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gyebfpfqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gfohygbec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gsovveode.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gyuhcfcpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gkdtbgqjm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gkqbtgkku.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmkknkodm.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gtaynnsgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gtphvznwi.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gfmueqjmh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ghcomngih.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gmcutuyil.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gryjcrvdc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghrgkixqf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gdtzumitr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gykugbsve.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gfxsddplh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gjitdvqhc.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gpoeowfsq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gvmoqldln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvytneil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gfpgafpcl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnufknomk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gugyecgmf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gltdhcbnf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gjpiyrhob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/guytgufnw.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gubrsoaob.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gxadtbdng.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gtwwhttbk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtqzazkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gwuxznvhj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gvtnzquir.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/ghkwgrcpj.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gyvsoucjj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gdpylqkvh.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gzivuipej.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gqabcxixg.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gypomyvxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gkkraxcpk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gewykcxzi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gubdhjppt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/glqhxubuu.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gmltgkrju.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjutakjuf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gscwjgmpb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/grcxuysne.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gdtugbhvp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gudnhgatz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gyrwzdcvk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gjaiibohw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gnoixyhtl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gzbxcaeuv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gjmyklpiw.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gdrnsgoqt.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/ghszkeurv.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gfvttuylg.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gxoaubrvq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnexgldmn.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggaobfnkd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqroozkpr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/grklppqxm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkhwphnas.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gpdaodrmp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/glpbeepur.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqaiyysxf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gufaruxwn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gxrkjayvz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gejssearf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gucsigkyl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gxkjkxana.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwlnqwtkb.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gvoqeizkj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gprusyqzr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gbrpursnk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gyrheomev.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gzzhwfxsj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfyysfx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gxvggphyd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gnfrnpehp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gehugdelb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gsvmymjgk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gsqffliws.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gftndmugc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gzaybhnpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gleevhchk.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gvfmzzqhp.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbsbvhkki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gjbvzkofi.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gabhbqtuq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/ggyrudjgv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gfawzvnxv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/ggojexzdi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gdslvuerw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gogywwmvo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/grenaqkpp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbdhpzqks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gvrhcglyq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gfecnzoyh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkgenxlyx.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gdcvpnlmq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbdvhfros.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gjrbgnxft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gxlfxlxxu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gjekzbxms.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/guvhtugoa.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gqdvdfjje.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gkdxaxuxf.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gyodoexxt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/grckfwgzt.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gchvazynd.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gqvrkablq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/grzljrjis.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ghodhpfgs.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqglfldzh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gjhwakrpu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gvqeywuxd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gocwgdqzy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gngkyxscw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/ggbxhipak.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gfedzdtkz.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/guuizjgtp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gwuhqzkas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gnzzgcvfa.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gawwmrizj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnrfvlxhm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gtonsslia.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gidnplisc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gtwkzikkj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/ghgnwzhww.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gwtglvprr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/geeadfool.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gcghzqhqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnfajzwu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gcddxcirj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gomfnywie.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gtegzzfnk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gsqdcqsyl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gwbdbugij.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gomfovmtk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gtsqepbvm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghripahdo.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gtdhpixxv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/grbdhpics.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gcktvqfui.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gqtecsmpx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gvpxbmoya.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/grrrzqtkv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gydousxoy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gksrqktfy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/guzadwxta.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gnzcvvquj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gjlxxffzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gxcrsrakg.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gvleftmdz.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/granxtvsi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gikfsfxzj.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gtcrbpfrm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsewurtgw.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gyhqhesjd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmcwfoj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/grkkuazck.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/geeqzfwtq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gdlccuvzy.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gpzmkuynz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gunwkfuum.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/goufhirwi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gpqlqypay.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gkkfjgqov.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gwrxumjni.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gigfsqmqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gaamdgygm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gwrwxzrio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gevrehvut.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gwegnrepw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gnjlzvppq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gehcozvrn.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gehtutnrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gjrektyqc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gdrzjlkkp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ghtysvmfj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gxdakesks.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gztlqvdqt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gcsngefjv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gkpzteuio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gsjogldke.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gchqurvqi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gjlosflvd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gickdtvmw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gtorxekqt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggtfmbqea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvtccnwcd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/ghfappuio.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gmdjsxwpp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/ghdjtftiz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gupahdrkx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/getslxmkv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gzjtecsva.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gzjgasewm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ghyynuhpb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gfqomohvb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gnycemwgu.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gsnfcsafk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gzrhjssmy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gtdsxjmry.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gtytspecy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/giofiegoz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gourrrbtv.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gfageujxc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gfhirxotv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/ghzyanxxz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gbnkplwhf.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/ggwrhuswn.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gzhknufjr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gocriodba.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gzxfmtzvb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gtpkdjddo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxaufhpmn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gsuaxeodh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gssdcgebo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gfuqtbrcr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gclgcoqju.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gexznqukc.sHtML


<!-- 参考信息 -->