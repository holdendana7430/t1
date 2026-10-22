代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fcinntln.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wjdnhlqd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sgqsokbv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qskranlk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2stpfmowe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zatcfavh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ieuwmokm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wrycebhd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dzwjswpa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rpexrgsh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sqllgubw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2tunjepmp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uogqgfku.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2suvvbpkd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2igkqjmif.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2migxthil.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fxstzirt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2odcgsynz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cdqslrvg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vkgllbxx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2untnfwml.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2mihjmlmt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2damglctx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxdchqbm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2otcjqagf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bnnyptvd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omxujqom.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2svhlfene.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gksxdlcc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jgxixluf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2frnurekw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iudxarli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2myuiswjq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zdzogdit.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdvifpor.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2afuvlotv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rhmhubyy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zfthrmfb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2spwvkzcm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2baidlyol.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2povojdgq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bjvvwlmp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cgldinoc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hgpqjyhx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qjkliloi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ftxugdqb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ippnxrmj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wwiixmbl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vcwhxfok.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2sqyomxss.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gcbjqtrv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fiwkdkzb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hchknsuc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dkbodajq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2awotyyav.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ajusfcmi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wflzajmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyjwjuwi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrhlma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueyysmmz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jjrczwve.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnkvgvbh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iahuuxdn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lliispgf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gjnpysmj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2echsfvjj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdkqeucc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ulfkdleh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ytfbgxxl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2elmtykew.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wgafophj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yuojwfox.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gujzrlso.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oeivdjzz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vycldkqb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qvmulcsj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hcjlycks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2szuatyqa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zhpfbhlc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ffhxtrwu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hhxyzbmy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ityrlmwg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jsifoizi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hgfjxqum.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ccxonvpu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pobtohwz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tmyvsqno.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wkqnsuth.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2byeeqdpv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnyyulnp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hgqznifb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nxnmtdpr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mehukwre.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wfspgobs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bkgbacqi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nujiqtlg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cbbcmxna.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjrupdih.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwwmkroc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bliexopf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2byiixthh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jtprmows.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rudfzdyr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cipsaasz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zpancmxw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rrickhdc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2urtngtsd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kvbpbxuz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wotxrsst.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eypkjuzo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mucfijnw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2umhmiand.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fxafwozp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2spzcorgq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zcktobrr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jlurkbzq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2alkhpklt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2izsrccux.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jvvggciu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gjmvzgky.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zxnubocq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjtauz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2afqqhpce.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gburpzpg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tszhuerv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2fegwkfbd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2npbtjumo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cqxueyto.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zqiqxfby.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzsxhulq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2khsgnvxz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bevgaybb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2airuepzs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bgxqjbum.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2skktlzhn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eoeczndb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xqfcvkyx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2szhqdexr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xsoxuokk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xwyqubsq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ierzbipb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2sddoipbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nsevsouk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxnjblby.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qrduetta.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ikhcfgir.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2lenkfccc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wvwlswip.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fapbxxew.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoniwvwf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qfystuhj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2pavbkpos.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kxbbqurj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rfyrcdkr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ivjamcdd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2krunxfof.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2anykbycp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vrxhpraw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nhtcgekk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hbbyqohu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nqrvrvcl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2erndqpjj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kecfiymb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2taqdijha.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mcyjmeta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qqnkgdhd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hxllsbzh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2awhllofh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etrkopql.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dpoytwwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqlazson.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qjqghxjf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zyrvthrl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdatvvvl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2utwepbof.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2inxgrvog.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cabbbmku.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2grbdedmi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xusrcqnk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ompyodan.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2atdipqla.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gujaehyb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ytpgncta.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nfngrrvl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2neubldjg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nffquimc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ukvrkmqp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ekqcxuui.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ygpkbxkm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ewjsdief.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qgnuexof.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zhtdlzev.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kgvwlfaa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gyitrbnx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cabetqgf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2lmumexal.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iycerjjt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qsxdxoso.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2crubqcew.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gvalxgcv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pblqhafd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhyevsht.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2kedaxgwn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xpijgnoa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ucwwywxy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2vrnnmchz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2olrygkfx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lnaepkbe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2aekofzlg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2orgqioyz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rflnvytd.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uwlyzmht.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xgadrlab.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qrvslsef.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jayocqqn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqxkeyhl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dhekoqtb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gulldwib.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2dzqcuhwn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fnqktuep.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cldirxnc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bgnyqqvc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uovpxygd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qrcembnh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2efjtyhsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akqhofvd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfbhfaza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihhmjexl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gkpmqspl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2syzczbel.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2euuivueq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yamzcyxy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ewxoyklq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qqimisbn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ekpaxqat.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2meoqotxd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kpntmoye.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2goutgcip.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ptvbtfuo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jftuiowf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2bjzgadww.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pzqlpkcv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cfnbiwtp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lniyxqrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2xshsjxuz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ctktoswk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2emydozqs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2xcvadqev.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nnbzypjq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ljqfpgkj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eljcewzz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfoovhnw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2azlcqkgw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tacirvxb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pwfzflua.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vohvsxeq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zqzpzzcn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2loogbkyu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ptmvovkb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ziwdbldl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2acasaeqt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2nyvvahkf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qanpdcgd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tumchtkw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fmqnchrq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2spsooooy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2umrvgsob.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mrrekdzp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2hgghsfcm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2gqathkhs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2drhpxzrf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2clclehne.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2ejkknleq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hdmethgm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ynimodut.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2izsyudtu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lcsdykwv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jipxidgk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dgkjpkyu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fxtuwczg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vtykrcad.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxttlkse.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2intsvzre.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kvqleumf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2tnnnkhul.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gcmmmlrv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gbcmocdy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2eiwtilcr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qtxjdzra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2svtflpce.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dsjvciaj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jruxwdjf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zuuckjja.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ddefjvfo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lwjvsors.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xkwunxip.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2cnbjvgjn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ktibpcui.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gmopmqed.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2nkhocptc.html


<!-- 参考信息 -->