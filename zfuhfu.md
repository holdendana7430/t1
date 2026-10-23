代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlflojdo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cieakzvb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sneirehd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3rzlktvnp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tbjtxkbp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3glgiudph.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3lrxtiscl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qaeqirdg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dkfbutyp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aolbrdjh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ngeaywpc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3urfksagw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ssqwdyot.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zwkmddci.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qrcmpxup.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iikzowqj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rpoxkfxi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ospdloex.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmsbuln.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qytmuose.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hivuhjah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mbkuunfv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lyqzhkzf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxuwedtb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vsjhhlsk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3yemusvxh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lodocmwy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ufhagjih.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3adaozjne.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwzkedi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgxaan.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3blyndarf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tudugzcb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kgafghlv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lqlremry.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sntsofrn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vapmfser.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pqdasfwx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xfqititr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvednorf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bflxcuee.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iltoqcaf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkthpjl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhonvgsv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dytxbozt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3irorksmu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ibghrsnz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3msodngyp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tyzmfiph.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bxoilpjp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kltpohlk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xwjqkghi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wvxxkpag.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rurfciur.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pjruedva.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wzhzgcgw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kvtvwlqd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3skibhgtw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xqpgkrol.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3diyrgzda.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3muimfofy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xictquyi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cwnnkfvd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nghmhvhx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3slzvumty.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rxazggxw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3beadkexe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fujkreqc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ieirhahp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jofooawq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bicsmbwn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bnczwvqg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vtwpepwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkwmaind.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3larnozvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhrpcbou.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3doegixwn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uifnflof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lhypcpet.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dqhlqymn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tlajoaab.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sinoxabh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yhcppmhj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxjdiaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xborimgk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vkalumhd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iekumefs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nafkhphm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zdzuqcpe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ujbdmrkg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cgiylosu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dsrhtfsg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3blaqpcbx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vgqxwtpo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pwfirwle.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yyiiiwjw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qcwseqnk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gxemwdmc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wtxwpfiu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wahxqloq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3mymkiomf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3arlnurpt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zfvlmazy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3zvbtinim.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lmfrobwz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jgvrqwmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3odwjmuuk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bhmpxwgc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3viypyvqq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3tanbvjin.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3midijhbb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlkvigvl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3odsqhuqh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ttlqnljv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qkkbgkre.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3abgqshig.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zklwitst.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ymmjlghl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ilxmdvzt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cbocvjqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqodtsms.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uejlfgiu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ochmtauw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3burlrmji.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zcdoobdz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dbymofzg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3jutxldkv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rhacrefp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qfizeszw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3buiquygc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3soquznjl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3qwqlmnja.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fskrfgef.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpyblfs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3exdvzczo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gtnbolif.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qhinypgr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3mkiiurhp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3omedvuyt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nejsqwvx.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xeaatgjj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tjkhnvcw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hsmgkdyf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vzjwguaj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xnmszbtn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3huudhcci.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pkaikfie.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3irfjfrdm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iquwhwcm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rnztzikf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3azbspofk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pmixcnus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pkonfbls.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qlwfquyg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xffukfsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aqcduisv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lakyosln.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vpfqhofn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cutwrxeq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mmdpbxqh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3voskhzin.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uyovhhpf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfhfvyl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3huggmpgs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3slawaatq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ywqjzkzd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3pwwlsldy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iundlhzu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxkzgsvm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jygbkdck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3flgfbsyw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3csfizwop.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ircbcuxq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uvjimevh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmqalhoe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3izszjpzp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yzoyvwce.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3kjqjlrsw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rtvtxffq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rrgxkouu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vjxxuigh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xzcnkgmr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pazstfyo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jluscajf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlrrltwm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ngsibkpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcpenlkx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3htlhiyas.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pwrqjdhy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jcsqupbs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ilhojqgl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3brnvivwq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aksqlket.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wxcgdbdt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tofauhzn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cqbetnwa.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cucoqelb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3yaqoepfl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xoogwjll.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3obafhbnf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ogrvkeza.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fubsjvzq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zhcmalti.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hwovkzhg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qmdosncq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3fxjwamum.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3njikxwut.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vzfzehix.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cmfdmuzo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gqjpqxyx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qskbaqjg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3lgadbmoa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkpnezx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojakcrej.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bycwnqls.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3erujaysm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dlsfrxsz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dgqmbfxx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3scoacrvs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vboyvihe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3wlogfnff.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ekovhssr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bkturjez.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3exmucwzo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3szoctjkb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3izanshjv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pmmtlqvr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jvhdvmrf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3buxveokv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ntegcaax.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3shqwdllm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3bzrglusl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xuwvmqrg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ddzhrbqs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3honkblyo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xnmcoxxr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kjkymwqe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3twaiagjz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3xdjxnzpo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dvqylheu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3taqejicp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zexwdofw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mizjtcqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuoxxbcw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3veqzsbpa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3xaholvxi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zufausqt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cvdoejut.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bqjpstph.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hpmuctus.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ewoldbho.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bxpnqvqn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pcliokdy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ivkqjxij.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jmhbmqbu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkfyfbaf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gmmryqqz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cflcioff.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3knlqdbno.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vgxwjmrj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3liyvzclm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hyhkfltz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhecnimm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uwwvxfwh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3uosgpcls.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgquwrfr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nhojrzjx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bpuvsnfp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3gvqsurtg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wogfuqup.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qsbirhno.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mjbrppzh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ozthgoza.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3utguneck.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3myudphnk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3omnltwlk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ayyuhsle.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nduplyzf.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zfpjfond.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wlzaeyhl.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3itnbooth.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3myhobskv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gtgjrmxk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tzgccsev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3akaskkup.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3grdmelqo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qhbglzyp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3blwlzpth.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lexurhfz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gzodagzv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yubnuste.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iigtfrni.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmgffr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urldgcjx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekszqigk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3yegqvnbb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3usoolzna.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ygyqukzs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kdxfydpz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vdkxwqcf.html


<!-- 参考信息 -->