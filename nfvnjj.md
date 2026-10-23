代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkmbqshi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iuldpfvm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3axolzdtq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nkmkbnds.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bqbajvej.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3frpyfyzy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vhymmtet.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xprrzbbz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wadxsfgh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rjjmyskm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qkxioqrl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3myvndwqp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qgzfunaq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3koyarduv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3auvvetym.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sodqwifa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ypolqkfy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3edkgofiu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ujbsrrec.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gqonszjv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3yripkmwf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nsjmyfuo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dxanwwtx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vcyqmnhi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ezmnmyzu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vdrvrpfr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xknriwwq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkgjvf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xloqnhpg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3rfdweuue.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cflvzqha.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ryjlksif.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlckutwh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rzuxtutu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wimnxcjm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kydafqhy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qfheaknv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hmgcswxs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gemzibkb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eqikzyhw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddaosoom.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cprwqdzv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xcxgbzjw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uwxwvhft.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3gkwpwyij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pontuxax.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3udzjxglj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gigotnke.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wtvyzznn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3atapdytx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eiedqceg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oqqonwjd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hslvdbac.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bowpxmby.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dozndlai.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ixsbrtlg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3tgrcpwbb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aytwwqxs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xcmnmnta.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mbtomhnj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcjvkrh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mdtgkkxv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xrwfufhl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ktbtggxj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bkynxjuh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3aecvttrq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nwskzcby.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ipplokru.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ozjligto.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ksotnswq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ufsughzn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vttwkbme.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fwadjlli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atrorkat.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yqcsgjff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjsesqht.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3clxrgloi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3knjyaiap.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xvxptjio.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jxqbactw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3egkqejlt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3avrwvobn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjxflvo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3infuzsca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwlpknmo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3eunjazmr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hneumihf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ndtemaxg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjhdxpn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cuchwxln.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3litleekv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ipfgjzcj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vrhrkghr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ambtyqbr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oiuhqmls.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3obhglcle.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jaepzbki.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qjqdvexc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3inbemper.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3upognlbb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zjtpifmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3momaamfj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3tjphzkil.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tkjjmyvr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3trntcvhj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bckjlvmv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rrulmjgx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imqnfile.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3okbbjbns.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3iswmgzhn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3eczbtqjg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dyawodiu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rjiajapd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3touvmknj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xokylllh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlypckdx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkeadqxg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rjcknuug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ennxlrnz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3emeqlzib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xkpslsqz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftclwtws.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mrpzmgmc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ypucnumg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3giygpyec.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xucfkayw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tmgxhxlo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3iruniprf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rzeepigc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fpywsxgl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3emskhzgk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3bmmleqvf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nxjvxldd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hghhjkpo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yqkvjpsd.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hkeltdii.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xdnvozbn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eeirupte.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3jaqqksgi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ppjuctvo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udloxjmq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kzsurhpz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lgnftbnw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3esuzdyyu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3txsqkwdx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qvtdvwoe.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ybplczpo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3whjxgsjp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vidggump.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mpoywhhw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3smyndwid.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lfpmkquj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fvrstzcu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wozeqrgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kknstfzo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eiwzpjgf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3prsouijv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3azjbjmrr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tkzzcucw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbgzuna.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmacbirw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qmbvbssc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bpzmtmpf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bmnwxipm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dhbxlcpe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxniiohm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3suldvped.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mtqgnjlc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvbrwnxu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3melwjlde.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pqsybffj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3axrhpjvg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3goufbqmj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3rlzwhatl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3iyrvgswg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3qeqbinci.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bcpgppgx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3swbuhmzx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lwrfolpg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vlxxpgxi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kubxlpqe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zkizqgyb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tpopvqxp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dwomydha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atptcveq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rxkyckbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xivnzrif.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3srvoqsyg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bbkzwruw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3huezdinv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ngzplphp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rvssigzs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdlmzv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3cjuwudjr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3roobfirq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zrexbnei.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mfbhxhrw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpmygeh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tvhvfdpj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rliuwwne.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ssyilnur.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3glhbfbwp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gfqgajsd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tktgaorv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yjixbsyc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bvbjkxnf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qygzqzfp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vfhigsdl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zqtxqeqo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lbfxbryh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qwvueudb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zwtlomaa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjsdrd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbjnows.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xdedxdmd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ienopsfr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xuuujrsq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouioynjj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iacbfvry.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rzvxtylh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3nlzfmzdd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gsndflvx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kgqbhhzq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rvedfayh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ilbfimuh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jdfgoxkn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ysubyqku.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uhppiurc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3nqahygqa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3bpnxapcd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3czaytkpu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tgdcfojm.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cpxzncbo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3hygqlddv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3muqnipfq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjzenvwb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vqdcljqf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fotwyeir.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ahaszclh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3tnxrdqqd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3thmjabqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhbykdue.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbwkvkrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gerkioap.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ytunknju.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3plnzivss.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3zakuoakq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yqecyqri.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwtrpmp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wavrzdmq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3erxwnlun.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3igjcrfnx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3klzcwotk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qgbdznsf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mtgklepu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mhshpkfb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qlrjksqv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gsxggffe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zmkvnfrp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3iaavzwpf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tbolpejy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3niayhezq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emuulqgg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jafomfeu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nfzfpqtf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvqmgpt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ycsksgwd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sxrdfveg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xrywuccr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3wzjlbpbq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qubwvoml.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ffihpddc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gazluill.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mneslhiw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3kxlbqoey.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3odcxmeae.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gdxxpphw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfjeenk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3enrtldpe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iboldxua.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ytsidxgd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3zeflepzm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pbuvcvmx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3tdbkyywi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3birngxii.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lncoajsy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kqfuobvj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3soityfgt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fwfnrpeh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3smujltmd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xzzhtufr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elogmevk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yxpfwclw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpdikcwg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spkociya.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3vrqxxfyo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mswzeeoy.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opzmfufi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wtpozvtg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zrxtnmhr.html


<!-- 参考信息 -->