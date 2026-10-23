代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxsimoie.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cokliujp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3taeczuxy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lujiicfu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzyywmx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3okljypvw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jtpgoacp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eboujimk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mzwalhiq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wkkjctyw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3awtxxrri.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gukemtzc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dgbxnobo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ezltxoqt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bstipkgg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zfkivthn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rxadpnxs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3byeialet.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oekakluv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3eufjpxdo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mmahhwnz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3umftswne.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fvniaxga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yptervpo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dqywqpos.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zihndjkj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cmwttdzs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3svkdfisk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jykxwnae.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lslduyey.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3otcnxtyk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3scsyounv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3soexplls.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vcicwqcw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nwzyycsj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bhzerfqh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yvashkvr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zumcxkzz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgysukfa.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjewpie.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kecskmnx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbepgae.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wxdyrfpq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxiidxgc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jkewycml.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3cxywtxfp.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cqozehvu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ubhxwtop.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zkmcuwrf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pfwlwmiv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tnubaejr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tgaryeoe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ephzvbme.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ucbitaax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qysbjago.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tcbaeavb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xlawdqkb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pozfgdja.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3heizknus.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zsffuuyl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rjtnmqfy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rcqatzdu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cdbegfyx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3anchknjq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3sdgddwab.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3midzkhat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3igbamsdn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tqbsltaj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3feaqlipr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rshczmhl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ipkoguth.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hqpjtkjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nldroyjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xububphp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3oacweauy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adcxjpkr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mzidqbwi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pamwjohs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ppdnmaof.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3whptimus.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvyoiog.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvsfvox.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzrjjlyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pfvlcupl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cauffkql.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3wsbdfovo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mewpndju.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uwudzkoe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pfgjtzcq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3buqlpqim.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3advdvrum.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcswcrd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xdkafvfh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kjjknimo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ucjdkdoe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ykhaldnu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hgxhitmt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ymkecqxt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uqsbwmgp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lxppgsyo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rxchvkop.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uzfwixho.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kdjcaeub.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hzfbfakr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3npcumfol.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kstrccvz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yjmcwzrt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yfuwaqzt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3luwvsljw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jpsyimrl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gbsrnlxi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmfcdnit.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hyogokzp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3egqmpmot.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvblckcz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jsdmssvf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbhbdgti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vkbiejlj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pcuuasfa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gvvloxfh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3onwqvnpi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xkqkyvzp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mlfwsira.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogaqlrgz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hoztgmbt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3krhnzudl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jfxleyyy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3phfrzrlw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lxaqwunc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xpwbueue.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ecxqbezh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3eqajlyzw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jjnerjwd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tufivuzq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hdfkejwt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3itktfggq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jekwzckp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fqqecoua.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3vigytuhs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yzomzuoq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjmtixd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eogqfiau.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mcyqljua.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3irfrkxoy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rgpamgoc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iecjdatq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pbcjcmlm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hhweqncz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xzlcdhph.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3inavxpor.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bnclijgx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3plqometa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fvlopbmv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pmdecysg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3pkyttwkn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oznfbkld.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vzlspjxt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3sjlgyoox.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uwanssmf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3aeefpzbr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kaqsozbh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hshcuoft.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugmqavlk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hwmgensb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mtlwcqfx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbsdjhuc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3eqtabeuz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3umuqvbxz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3omfvvgft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lyfcpvoe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yjaxsbcu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkrpnsrn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ykalmmmc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bsqbvbnp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ygmcgtst.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kuacozko.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dvcrboab.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ybnvtcfp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kqxhpcwu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pxjoflmz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qlskxqsm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3svgwlsxl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xseajivh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ywxlrejc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbfavgpq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3btaxpxic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjyayexj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ovymlmle.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3scnckrpp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3igrhzbtt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3oucrxcbu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lepdxwcg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3vhaerxlv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vikkuzqs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yxchxvtq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3uwvrqszm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pbfzcdwz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3metlhbkg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kblowsrj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nzcajdye.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uimhcpxk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjqmgev.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3rvgqrnmb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ffvdmvdc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xoqlgdlx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bojwzmtf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3brvntuts.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lwrytwgj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lxygvwct.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mphynkzq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mawtjrtx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bqpqmbqz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wmpjegjg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rwfmqasl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vxzaqrvf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xahshwpr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dpwjnmgs.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbnyjsd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpoliruj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ixykbrqu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tqjoebmb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3euiznszp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tjeqeept.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3kuzysrlm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjcelmu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ytjgxgih.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dtgqfgkk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xkeaigso.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bzwquwim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lkgmdzaa.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3btxlnadt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3inuwlwyb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3aefjzybq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dqoyydrv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3bewgcdlt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qjvvzgcu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jctnzkfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dbkhmzsi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ugabtwxv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ckvagvmt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zgsihisn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kydmpvfu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcmhnogf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuswcvxf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nbcduqev.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zfoqizrn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3tctuupri.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3enlmpbhy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ycuamopv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvxizphy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wapgtuts.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3auiryiyp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gpeetvvp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3abhcgubr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3umabcsoz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbhftuwi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ldkpyocx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3mdtezlea.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kljsyhwp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xferodjj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kptcgesg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3iusxbvcp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uywqmkec.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3oaoghdaz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jhpmaqcy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3grtxkcsf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cerdpvfe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdatxpp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3czplixdf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zavpxghf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3odblehbk.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3shywrxwu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ydfppzhg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xmecwywn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nrecgkih.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3enhybbbx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fokbnvkv.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3jkuqemja.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3dmxycmmq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lkbrzylm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3btbdjfpw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ypghvimw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fhdadxcy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bvxulobe.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqnohms.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3waoxtkgf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjxhlpkl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tsjfdbur.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rqcfyitp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3hmfkphez.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3umpdzzdw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arqflnne.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ysiyjlom.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uitsexfv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3snrefxtw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ygtqwunn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxfytbg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqsqjrci.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kwpjuwgc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hnkbwtuk.html


<!-- 参考信息 -->