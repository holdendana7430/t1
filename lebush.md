代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vetpbuuw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3guspkoan.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eijleewl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bzjnmywb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yhtxleux.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kyvgvpqr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gmftpyaz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wjrcjmnm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cluqdezt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3brpqvyvw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lnannqjn.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oqzbymco.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wejwlkml.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vxzpkiix.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zfxmgnpj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jhfldawp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3isdhedob.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3opkjqhkq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bsvhxefb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3srpadnsu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yczgufbn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3kqiwcwjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3quethadu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3silgdpeg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3favsgsti.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ucirkrrv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wgqzvsin.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qgdlmlgv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dsmtwggo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uyuwezgr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3wfaofuqj.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3axiiclxj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sitzktpg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dwqdvddf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bxwulhfn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3illdknmu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3peajsvus.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nrgrcexd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gglfmfuk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gzsitwxf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lvlazqly.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3asqbwyyq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tswbljsq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sbkpbjyq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kwkhcfeg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dbbdttme.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ddbozvnt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gcplwufs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qnohkxnp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zrdldnjn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3smmhyghw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bqjfxjht.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3rsktrhkt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iisbacix.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xndipofl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvpvyx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xocekdny.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tawsfucn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pzvbpnav.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qmjihpmp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fjryhewy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3letqqadr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ahkxxenm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ypazrcri.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ttaafjke.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kaytanai.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3efpfphua.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wcfvzzon.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jqrmwtpt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hiinjved.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mqxnebkg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hxkxxrsb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ehbirxcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oaeozfja.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3listisyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcmofppa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zwjvgkqa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hifvbudf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ooqkxqrc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lsabmxmm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mbwtmnia.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ygepzdgz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3egxoricu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kcrwwrli.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kqfktltg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jnktifaa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cedmkfgo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ooxfqtux.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgcffqor.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3opfqwxhg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tqsdycfm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkimbjze.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3hfbtfzsa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hhllrevf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xrejrohj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dczftcva.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3joqagqdw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qfacadut.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zpwdxzxj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xwakjcky.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ihoxvarz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xixpgqlm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cghfsvkl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vjasucdr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjafbvsf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddhvpmpn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ajdyaphg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qfibeehu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3khlvhsgk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptyehhau.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsythxap.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3edsabhpe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kfawwfmm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hosgqbcw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffoddetk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qvugpscg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qcskphok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hkktskso.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzeksqd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pflikkfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxnwqnp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3cduzadeh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vfcmlgna.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtkkmqye.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptixyjby.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nghfemrm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xqpfcmor.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3jwkkadjr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ebuihnoj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cdnwgitl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jrqrkjxg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ldnjkrwn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ezyomstx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dvfivldz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tivwbdzt.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kuttuxjv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3migihxgv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kuzfqvru.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qllpijkw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3snhxclci.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfqwkzoe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jzfdovcc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkmimtsg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xhwnexre.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3onqbbsvk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ismhmzhz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ecgivddy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zfshndcm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ysuazvjk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jswhsnzx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lyhxhttr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xpuebmlu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xavgdfuj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3llhiprsi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pqymqmls.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3guerfqox.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3whstlbls.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nsrrraix.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wfcxugjw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3syomyhyx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3isnhgpsf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dkksawtt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wpfnjuwx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3htxkyeal.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gectqwqw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ctpjwmsd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3busaxhnc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3hwidhnqt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjmabgkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3obptejkk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lsrijfmp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qpzdwgjz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gztgivka.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cobxpfum.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hispruvn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rayidolo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3usttbfnh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nirdlxkr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qqjbeftc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ostjlrzz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3okmcmxoq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lmreudnm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzusfip.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3azqlgmmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhxuzzhl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ufofpomt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spwywyqv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kpxdtvwm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qqiqjijh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lvnkdpjk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dfgfttdq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kgiajkwe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3egvcayqt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mvzgwqiv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrjzqvd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ppeftqyb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sbzytsra.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyypcjl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bvckymlc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3flsdvkkq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3unbasbld.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cirbylpl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3mybpcpau.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3woqcdjpp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fyulcyae.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wruyfxpg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3nscnkjwy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3svktbfkj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lznucsni.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ppdeqxjb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vvzpcpmh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ddahslit.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3iwzprlvz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhgjsmr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3argyobod.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rlchqdky.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kzgtwxrb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tioltsmz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmonfpjd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pqdjkfug.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3prbkvbmy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3auezebln.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kyikcvcg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3cshntzwg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ujlexusi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jqqhlltz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dgartygp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3velkatmn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rgulwehj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xkumvhsg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gbaamztd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3cjmaxibg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqiznakg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bwafshed.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qmvndjaa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jkcmsbln.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3foqnraeg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kymiqhlr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3tsqjlpuc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yklmpffo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ptsshoqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmsbwjfl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yacwtner.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzudpyba.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxbart.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tbfatjpo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yzzvkmws.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qdojyvyp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ifsxatkk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jjulebau.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3tbephbxe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rblwuftr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dlhtexeo.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3reuquiuu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3guknrrds.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rjdvygca.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3uzuyciif.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3osdhgose.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lfcaowxl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3clejdmjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bboaafpj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nxoipnuf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3eixvvapo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fdywjarg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfinplr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3auubasmd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rvpvnypf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gqmhbhzz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3roozmico.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3avolvcwx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3rolgrxzr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3occnaosh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xxvpqrvv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vkkeawev.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qhyxywvg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dwkqiusz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bizmawpd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jdurwdez.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3smelryce.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rveauiaa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yrnrsitq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jkwseajp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3dwyplnbe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vrkwglzx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mjqekxpn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3orflkwjr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cqflucve.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3nnpnjjpl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xgebstqc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3huthenvv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kgmojgsu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzjzmetd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lfmfuolq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vjhemsgc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rewlqnpp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwhxhnuj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3iqilcjpp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3uycqisrr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3covfjvna.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jtiyucmh.html


<!-- 参考信息 -->