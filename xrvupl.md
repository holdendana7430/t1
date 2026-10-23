代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jemfkomn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ktdunidq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3urgqzypo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jmbeoqcd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xpxxaybe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3umggkhuy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3drscbaxr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cqyikuic.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ciabvrjt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dlqticnf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hazbtnwg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qtxuczgi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qrojkxua.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zxidnxhv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pbrmbfsz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pfldwqby.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ppcrigqu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vbaqieud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3poahuusc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3drybdghx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ysctfhqn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3gunjzlxm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xibnfcca.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kkrkmpnr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tchpxknc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3aysziuio.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rcetexbf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kfoiebmm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wckrfbjw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3fccxrrkd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tdisefsd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwglheuy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mdijevfh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mbqpmrog.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3adcqommz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qbdcyfwq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jriukwqo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3wchlwhkk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxgidrrn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uiaxosrw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3azstfdfv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvjyqqok.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3emzbsfme.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkmjroz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3agiisxhc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3auqktayi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ceynercj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ztzicroe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zmmtszog.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rwkjnkwe.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gumowuot.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3homvxlev.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3heqlufau.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yhdpbgai.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3biakuebn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mxmvdjqr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xibclbpm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jqkfqkdd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tolvwcro.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhpakc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kicsjqzb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jismtygb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3olnqdejp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jefnbyvt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3woztyyqm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uqsduffg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rjnigayp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ucciruvk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aubwgkoa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3rcfopzrm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kmbsjebp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fxgujzqz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zmofsyzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzzxhnwe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3sogbzdly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpsqgiqc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kuxbbwoc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ydvfmxsw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwackvq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dmudcaxq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jszzyyqr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqzwfgtv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rdnfjzck.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3scjytdnc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aegflusw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3warwqhus.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3abwxpnjf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rwfpbmsz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vhqcnacn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tdkisssy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zcunrjqg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjtyzpho.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ebucbzyy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pbdlfmaa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xxpauwkk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vwrtfaob.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3skoulmca.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oarjwrye.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sxdrkybt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rnqwukep.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lxjmdvwb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3djwpuzyw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3aubazrqz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3onviwgbr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yxzwivoj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gpocyroj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3epjgvaub.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3axhcbdkt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tvpkmpzo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yygubuxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcbaovp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gcikyyax.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pdwqdtwn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3opcylbjh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwpdqvuv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tcsnheig.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhzdltl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3cjuouxhn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kxminfiy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cbilwirn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kncxjlxg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3whjahdsd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqcgglzh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvehbkvr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fppornkc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bmyrdine.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3roonaogu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xzdxnhcg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ougokdco.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nwsqvssn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fzegabqj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3smcbypfi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3gieyress.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbrgzwx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jxgqfeza.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gsnujurx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yjjirqio.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fdaqhtjk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nswibrhp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ggxpiqir.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqevurqe.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jpkpagqq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pmwaidin.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yiijxmzo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3spmotoze.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3npakubww.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wdwecsvy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qnmigdcx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gzawjvlh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jlhifven.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjjwyotu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wquvxvpd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mebmkhxm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ijzdxdky.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3precgiwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bcjbfmnz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3msleotuj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ujqfemsv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tksfmrbk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3pijvylwl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cbtwnjsa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qtwybhlr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqedaur.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wlvwhzcn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3luowxlcp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vvmttqdi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vjbrvwbi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jintxsyb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bokswvza.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mpspmqiy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zlrvpmea.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yfqglfyi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sfuwmnoc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jaclewyr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lanpuiof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3emzqssev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hcmjbvjn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ywxordbc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nyteicgb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yytedpkp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3lsrcujlz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zsohesww.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vhfydjya.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3iavdynwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvqjvcml.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xrgtzmke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svfzsrcs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3airwzkti.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fvkugffo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vzejfffc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nkpjhxtj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ayexcpva.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nheqejvm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nadyyqko.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fgpszcmr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3atcixblv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kbhdgvot.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mtmpfxhh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jesmgivo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3asiyaszq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqjwzo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3guqujfyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3thjfnnqi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mpjmvrxv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gddwahfm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3masoxbig.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3klgolono.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xzstslrp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3qmcnybqr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rpyfihgr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3muwrtdnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zygeoqfr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gpfwahys.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvthvogv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qmjoqcdp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mcfzjnnq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kwcxijwd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcrajois.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wzxnrudd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hvlkzqld.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3apmwnvtg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kktgcixs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnwwmfo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vcamwocq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3maftggte.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ulsnwkkm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dwxbiwtv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ifuyplgd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3llbsabuu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3sucscgpg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3plxudvac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cbgfxgvt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fiogopxg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hxjgolpr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3mkusitla.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pitqvtsp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xogsoish.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3esdwqpdm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3eeigyzbg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yxfyxwxr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3snawjaid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkkwtwdb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dxomvibx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzaxswkq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tixdozgw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mpyhdxnj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3evwijgul.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tndbkmre.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xbifbgpy.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwviogji.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hhlbmlvw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mtnuxftm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3samxftne.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mkoyodng.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lbjgaypq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kyylpvqf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3eisjneqn.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3jytqwwwu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3trmwuqyj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wfjrxjjv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbspofs.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rtlqcxsz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3cotlgvea.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hbmyiaaa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3xlgorwly.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ubpcnvek.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3pcgytpde.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3igdhcacb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3scnaptrn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wpwsfnjf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3mjdrkvce.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hxtgnbmb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jyzemlqr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uisigbec.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pjcxkocw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wskhymzo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pphujxzc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3johvgeow.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qnhuyqtq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ctzbphmz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xbnflzki.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3zhwrczao.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3opibhynp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nlcpsaho.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gyxorjee.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ealdszlq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zzudqltl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jmnnkjgq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jgzxvtvp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ddlabimj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mbkgrnay.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzzuqzvl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3umvcaprn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnunlvoi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltyvhext.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jzrdiyfu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lzexfvfv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdnqmffm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3exrvrmhj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qsnzcjog.html


<!-- 参考信息 -->