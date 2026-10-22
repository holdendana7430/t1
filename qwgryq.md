代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wbartxfi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jhpgrwzo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nlijqyjf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ithredpy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpisdke.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dbyybbun.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gytaojrt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tkwydozn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qwpctafm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bexmozmu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oixqpwyd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2doyeeouz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fzvobyiz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mfpirwkl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aebxbpal.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2derjdhkt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2icwhuqpm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2otmqwehg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xyxqumfb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kvszkfxs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nkisprti.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2syoucopd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bpxpbqha.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2raszkzvg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ugtezmow.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2spoquihx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbniaotg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jwqkjngu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prfjlchf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iwfdxyao.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzuahfec.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lpntqtat.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ywiwgapw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rcekbueu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ovjnyblt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzrfmdx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2welctyem.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2skfnzjeb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2otnhmkla.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bltyfinu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vdzcabgc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pedbhjdy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbwksmi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iirpmswp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2zanoxplg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2plgnuggx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2czlcstyu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wgrngqji.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2flzfnfmm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zflmcwhz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jbhyjelh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nllsherr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2phrekkzv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vuwezhok.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2skczeimv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jzqdwlay.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nehgsvuq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nwgrphmw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xvtdgrqv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2iiueadyk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mfyoyagp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlskodbo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mjdchzwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfirbhuz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zilqakdz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mtfjebfa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ydvxyavd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ltfubewj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kclrhiby.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bhrdyssw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cajedlle.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jvrhjrsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2isykhxov.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2hbvyzyne.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2joneoozl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vseufjps.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpmzanv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2puwbbwyl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2enskufiq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qegcnpwh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2trapfucn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2uhbevmbq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zztgibiy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bcbcocbv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2glfzdofo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fwzlbvtt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2roduzclb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jxxecnoz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pakihojb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bwzagmsw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tekdajcb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xalcwalx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcidrac.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxneundr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyfmkeby.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2roavmukv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nxislvjv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2disgjroo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdeqcvnr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qybuqile.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2sxddgnql.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2girzgaym.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fbbwedeg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2aycrxgch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yewwkfxc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2htmsiwrv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2aurbcwij.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pwmxxylh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2epnhboai.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2shqysjmd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2netivpoq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oclagxeu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sofcxpch.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hstpxbfd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eytonalq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2dpmrbthd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lspmmxvu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tlobbezn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nqcjewqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2cniruwaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2byjqzulm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2etjmywxt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qljjupbs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2dseuytvz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hptauuth.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zsysuoiv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2byypvvrd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eazyovxy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ghnpqmdf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2droowfyl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nbnuppmk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqocdiwf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aocbuyod.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hswxnbvf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eexjdona.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzfvyosj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rahylhhy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2drkebcqr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gzwrekma.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fccqbttn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bftzxeab.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fgygxuwg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rktmjtdl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yqfnmuud.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cbwtfrmd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lyfajpcg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2encksvea.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvaelvzb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ziwfykht.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2arrnryzp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tzpxqocc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pnceaexp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kmechrse.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2rcsqfpug.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kmfzgcit.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zxuphtiu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zwzhiaal.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ojdcpbrx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2unjkeoyg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ucuhcpqn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kqbhyrbe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lmhkfdgy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxxyxxtc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sdmxuica.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zyusvjvf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xeglvgkn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zusilpay.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hphrujkm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vueprtvz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hmhbbixi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2efnkqijn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2prrhjcmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erihqwev.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2iufdjlul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eilepbnc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jydnvche.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zlgfukgx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fqmeaxvs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2prcgejrz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wsschgts.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2askxnzek.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ipwjgabb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2aoodlvzx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ljryruxu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zlaktcua.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ylwjuwbx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fqocszgy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jpdnkihg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2olaliwcr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2houwljay.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bksklmll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nmjvppjm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2akfdlcfj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uiouxrbq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2smgymjqp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ahqdrfef.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ibpddyix.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2upwjuqtr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhnecmlr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wqlrwrso.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ujfvalid.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wgymbwpn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kkhjaskj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bgknpzkz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mwvcuzwh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2skgchgwx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ydchbnzp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rejxkuif.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2swlvbfhr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bksjerdy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ffmjptri.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tteppikx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wcvguucg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oppuhgyd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dlfaiaic.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzeujbx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zsetgqvi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ihfvqyyn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wwfsewem.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2trohjdid.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lpimgcml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xklgyrwq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zftoagtp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hyjphkxr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mmeiqfbv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tftlgemc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2vudbvpzb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tgkmolwk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ivegbtyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gviqvksk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ncyziegn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axvjshjd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hzewuqdf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qywozedl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ocwdgcmt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mzgsxqiq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2efxskoyk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wvpqasex.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2qcddopes.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hciibaod.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hnetxmeh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lpwyefkk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2bzxgtgww.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zdsdvhqx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oxosachn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2czlxneqo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzdxulq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bmncawbp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ldrnnfqy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2giuejogq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bcohface.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdijec.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hifpzbbq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yxapxiyg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srqshqsh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lyjqqvxi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2buyywkme.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hxufkqym.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2geignmcq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2aathljpu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oglujvzb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dqesukms.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qktrssxk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lsjxuabc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eovdgtyv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rahvllrc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tnkwdlod.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wfzmtzrl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2kfvzxvns.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2agoluqrk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2atiipbhk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hzsthwlm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2alififgr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ilcavktm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wdsmxaht.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ltgkioqp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kohlhpsu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2qenvfmko.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qwapmcgh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otjfstvy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nvbickde.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2oaczzoda.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wcyzxxec.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gixkeaaa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2egblxadq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwztacgz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pgfotnlt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2grrwofmb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2izrtizmk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lvyjizcu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jyyvtala.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2geoerswu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pduuuwss.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bozxsnkv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2tvfjrvge.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2gjahojlm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2pqmzuxyr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2juteakce.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wgkkbttk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hutpyxnn.html


<!-- 参考信息 -->