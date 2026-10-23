代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ltcsjxpp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ynprylip.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fiuymuzg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mbrkrvrs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yikhtcwr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uypebopz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wyugaaji.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3etcmsqoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3izimduaw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wywtkchl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nbqdevpn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bdhhgffl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jfxecfca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yotrwmsq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3yxbqmzhg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ilumytma.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3teaqvyok.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bhnpxkvr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dirlizga.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cdkogibl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3timzigcn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jlomvxcf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3areqzwrz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pngmpqsd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ggbjbhul.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pzlsuvqy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sivzjhps.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bqazzytt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsxrkrq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahfilzea.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvwiqlgm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nataqygi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rybygqng.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tutvokvz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lxiixkie.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fwjnmmvb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3dczwtspv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yjogyoyj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gluvjyey.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zgtfersu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3brhfhqar.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jbizuhuz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jqyrubgk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3unmgohvb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hobwjixj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3onlnsusl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ugfsmavv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lzztowmg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3drrtkhnu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fvqyettd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3babxirpl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpcinsc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ajwxuqyp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rqprolig.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uqfmtvfo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zrawlipk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wkkddlgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3akiifriy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tbxfdwgj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gptrhmae.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3izzcgzez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clpypbpk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wwbwfqhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qutchrbr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bngepdhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3owuqihwq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iaumqwjr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tduhuhhe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3onvvgmai.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xtyiwqhk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nuynjmhk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xtufnbbd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bonfnzcz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lotpgwng.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vupxzzqs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3esficwzo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3abqclkvi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mewnvica.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vejzofai.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjvovzwm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wwmeghxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3joffhyqg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mrkhlrou.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qlslaadm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wwqpcter.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zonjkhap.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3irjvzepx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3otuhrclw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vsrsxtvx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kwbaizxl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ppzfxkhd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lfwxtruu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pfxsrbrv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jrmqjfrz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bfplxeqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hlalbquc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubacoqei.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yatqhsai.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plmqompv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bcpejxzg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3umaccqqj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3asgtulrm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmpouruh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3maiuxpxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3frzqhnno.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3nbcqhjpv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hgptpbuf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mpkwjupe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mrvuhzwk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kqkoaenc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ijutmcyb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pkvahklh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ikkeczse.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3acgndpvs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dbfldggp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3reeovuvz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tgtyqoml.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3csiegihp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3mhsyrjmx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dtqxnvoi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wdbnmzca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pwwsxmtq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tzenzxwd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qxedjwbb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vrzlzssn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tgswcacr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3pqsldnef.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ghyfrojb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omijkyph.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3rimbqzan.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ykrheses.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zqpovajc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mzqslylo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3isxookkh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wijhndvm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3healyniv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ofeknqrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3xhjjcukr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ugdkxaxs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yjutjrys.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lmrozjex.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gxpriwau.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rpjhfvva.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3flwuixgc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3phuzaeuv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3rwstfzdd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zdxofeho.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3voqweuyf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yewdcxww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qbzudofs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnpxolkc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vnuywxwu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ttivwyrh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pjtbhrwa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hoacxqpt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3udcagndq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wisvgitf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nyvvdgfa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zegwzvma.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gsfcyutk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oiynpnfq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xcqfqzmd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3umtkmysh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3msclkics.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lvgyptqj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iljutaau.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yyxbtpgm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nmaydiir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lhwwkdgt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cekjfonq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkvimieo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uwunpdhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzlipgry.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ujuvmivc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akriiawb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3todfbpnf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jfzdwpmn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3oeymntyn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3warrrqzu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3afofvlds.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3budbukrk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3klcljihv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3usxfnapt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pzmlvyyx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3osnxjtgs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gudjrohl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3miqeosud.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yhvkynbe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jqatafte.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3elxkifux.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dfegyrbm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qrrxsald.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qubhnpln.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3smgxuhbg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gdpktxge.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3vzyvmstm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qsojvmqv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ioamxtys.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kmyliggn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zdnceehe.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqnorea.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vroqdaxp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ptkkysyz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3fqoueycg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cpnionfg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3scbdobmv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjajrlgt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3gsldddxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jwytiwfb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3hpqkmnck.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqbsos.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zzkiapuh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzvwmor.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xbjikkls.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mkoqcjbx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cugygfgi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gmvvafah.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3iybdnvgg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3frbrilul.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vokherbq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ubbnvpld.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fngzgext.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3sgdupmfd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3owphzwkm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rmuznphm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qxtcnxdp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ityugewm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3sodthzqy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3owqfuokg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pkcwebzr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sbmdbhpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axjxgqmi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qiqhgnkw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wnmqtkip.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mdvolibo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gcyxpitg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sxtreenu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3hwhlqovj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pwtcgjng.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zylpzfkg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3oqwlmegb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eolfoyey.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xjassvad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3bmqbmaoa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jiregiye.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nzqlccng.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gzuaijhl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hwtcollg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3svgudima.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dodyrckr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgsrpelq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3sfyipgab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3abqvhluc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dszjvaua.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gfvceffr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wpelgorr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bbclbdql.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fnefpziy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vlhmhwwp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3etmmsoph.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3dckxedjs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iuyvvqfs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dsbosgnu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ljnmpuyp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hxuxwzpb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3tywgioqt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bmjihzdo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jhwlifuh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jedlhmpv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wpnqgxpl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3nvhvfkqe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3omrmwdxg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvcemyp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vpppfvzq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ldimufkx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vxusfoka.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nfdeinpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3klnqmhmb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nexhkutg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyxkcxga.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qwzopixy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3woxjkgsy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpkagbrx.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bnpaixyk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxeahvn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3mectgoya.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3rkmddegd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ozyupfzc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3likfvjwj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lgbkenxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3trbacncb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogdfpzpk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3wlgxhqdu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3poxaupnj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ipmxofyq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3deykrisn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mrezcarn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnsessob.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ejtzidyn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgcnaxl.html


<!-- 参考信息 -->