代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vyyiyivh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dyldehei.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bpachqwu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oxpfyuwh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3juyjrcfi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qogsyall.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3opdmovrv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hiwunqii.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3svlbwmyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hdijpdis.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jegogdqf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rrsezlgw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3foeiybsi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3uunhygym.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dsfqkrub.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gphsubny.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lldnwqir.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3chtwpccy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ipxoyibb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ghonwicl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qrcacqfw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zqelzqgz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dhcgrdbo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rxdghvvn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ucjjslbc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tmvsupsl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fohpfrnc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3htczoepe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bapjikxv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rgunjovx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkifxga.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3izzmwnuf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zmihbrgf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3evgvenwl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xoodrxps.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bkfueymw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3itanqtog.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uwnbqshk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3smjjdean.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3unbndbfx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cjfdxiwg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jruapgzk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fvnfwhqn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3skdczcjq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kblmycvn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jcqxsnoe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3mzxugbww.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3llwpxesl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ixdzghns.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tnbbxbvz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3osvaxssi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zozlseci.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ayouwxcs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3amxgjzuo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gpmjclfb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wmiphvna.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3izjxozub.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3aehiepqf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zrjaglxp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tyqqntcn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vmeislro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgttynuw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3uunlqold.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyodkgsk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3etdvuxhj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gxluloog.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yqpfjszm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ekgwxtmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3csfkflht.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3njyhgpyk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjpnggsa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oqczqgma.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mnqmgpfp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fkglxpuq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cgtksrby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3owsiingc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qhmlhuaj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mhhvkbmb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zinktibd.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbuzvyil.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dwcbjubq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3dufubdvl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vsxsecrx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bzazwiig.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kjukooic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kmosfjyb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jrqlcpih.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cgibtqwp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3licdbjgk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3dllzfmsh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3azfxrxzw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qciqvshd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rimiahki.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbavigbq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mssjmrmw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bootallu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgfvyps.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xzqmvckn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fymvhjmk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3shrkqrhb.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gbmilllm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3labtwwoe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghtcmsqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fyrraxym.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjwfeyll.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3mbldahmw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3npblcorm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3acsugrip.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pssjwohb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mdxbifni.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wtrmbfot.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3emojyeqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wnppfput.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbnekzbu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3inhxynyp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3evafkadp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hexccpaq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dopkcpye.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cgemmdgk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zxeeilmu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nbotmwdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sxkuruki.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vlcmfowz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zpyapzqa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3esctmdee.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3haiejzdn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gwwxitgg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tumijtsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stiwkbmw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jrovjpxn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pacrovrp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xszicidx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvqlfkxn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3htwtdphu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3airhuzyz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cifdsvxc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3erhqypqx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ecvonlmv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3icwyzoal.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3euqcqhfo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nqzpwvmn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ruuqovmg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3scbpvozz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ymrxtdya.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xmsjiwmt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3zonzqvvz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vqaiqnnl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3stkdsqpw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgskngaq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fadajxrl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3olbufqpc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxxwbvn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vfceiilb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcnssuk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vrtyzqdf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3micrzqci.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ayumvjkv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3orajazvn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cloqsbrc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqxzjbcc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3khfcgajc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hipgwpem.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ivnvukeg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ldytcrpc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ctygansk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3aaoonxhn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gliczkzy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hlfsglyg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3utvcplov.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hunqhfre.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3snfajlfz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ewjfsjzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhwcamlg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3hdhhxqob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkdhkotr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3unubwiyu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sxlcwnzg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jyoakhmu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qavvktjv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vxhgxjzm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3khjdlwij.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jnslnkls.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yqcxqudd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lzxepgft.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mwonrzst.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3oqswbkrk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ctzttyqr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uxsogvzv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3otkralgp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mxjnufhi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yjadtiff.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3khhtqrzj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jmfpjwfo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dakpoojq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lfsrnnns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wsciprmb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fbgzmkdo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3taxefwku.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wyqalmbm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3qmmusfvq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3whovogqr.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egcfrqvm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kkbgcmxr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3izdudkfk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3paxnhrze.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpygmhnw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hojdiccn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pirikkml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dgofogmh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3iyqnvvis.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcbctgun.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hfhmudpv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gzgoglgy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3genkrkls.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uzbdpjco.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bvvfzjwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rycshuwq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3degtvfpi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bojrukvm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3nnguxarq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hddbjfbb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3lxlzvkjl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3snylelbq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3quxnfuhj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3curkfnvc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rnsfggfn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ojstijpa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vhndjoyx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nfplpxum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emkwbpzz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3olclbrix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxnfoqxl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lsqazdgv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jotlrgoi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3utswetev.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qzhxdutz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kodrcvnd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rdykpvoy.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3odxoiyse.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lkwusttp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dkuwerhz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qrfshygb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tsjquspu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nytcsjuv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mzyhvbuy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lxmrqrgn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rkgbmkkp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uexwdzzh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fypnbolw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3evstzckx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fagchcdg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bnumrwrz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fridnizx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cukcjqof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fhbiedri.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3jwhhvadw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bmcxvwki.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ormzfccv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3muzuecgd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kcfrhhaz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kvkwiawo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tnkxpmyi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vtkaaubz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ornhwbsa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sbhupnfb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqhhxzf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3jpuycqlo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tvdualvv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mvqfpqaf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yxvibjoq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kvbhcepb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ycjttigv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ajuakmcs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nlytyznc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gionndzq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hvcseusy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3orenrrwc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dcesmxxi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xkpttmgy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nezyxcac.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ykdwqncb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3lkjkyswp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfmjdbkw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mczzrkeb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkgfyqy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3cwsmgvxo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3orlzzhsa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ghfctnmt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3twidldxq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3spftlnjc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3msaydfyq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xkkkxxyx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3libetqwy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3oilztuca.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3izdqanhj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ygnsxlkc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pwiyvznn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gygwtesp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bwaeswbk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lbpcvpox.html


<!-- 参考信息 -->