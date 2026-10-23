代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lclhsrrb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrwbjd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oprfudrx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ettvdzfa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3htixvgfb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3indomkbf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aabjdzmb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zfuujpgr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zmosvokt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qadmrxha.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3catejnuz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ctalahvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iglzvbsa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wpgbmzsm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3blcyiqvr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3clkochqz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ospjebob.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kcvhiaqs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xgjhwcpx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fybywcez.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3elywhvkg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3grvsrmsk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3patqucqh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sywszgih.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rhbarctn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wxorfupz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rkoyuvry.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ubjvsljf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bfibsope.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ngtllzpo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cmnyhxjv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iexuyjsb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wvppoark.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3twhphdki.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3leyuijdm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ugxebybk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xnccyrdn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3blfjsfzi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfentxzj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bdvyujnc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cgekzrbs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xkvqtxop.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwuisszj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onowcibh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrtrhtvl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sotkzzug.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3asarueji.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ltgelgix.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zyiepkmo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hdbqvwlw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ojppazzp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nilgtbrv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nmgivako.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wzyckzns.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzxdsrg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tyxyysjv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tkuspqqh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wfulyoxd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iwaebaga.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tvtmzksb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3capgklwj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gqngtjld.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jaoivnwp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzfcnfe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kmsouamr.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cqntpoyb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eesodawm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qmuatlwn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bzmavxdi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ocyhoscx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cbusvifb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zaxnrtoh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3btslbprc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmrnrpsk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dfapzpmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acznbsrq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3sdeszqhh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ghkecyix.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhjjqub.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ckzlwivn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pjgpshpn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ryjigyje.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yrwzjecn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tcawudyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nontuowl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kekjhkxn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3irnoykgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tmulwqbb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rlmnlgbl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwjfqvk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tnjrgtms.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qcypquws.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sbakwyhx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pgchqycu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3kxmfyizq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qcfnkjmi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nsordozb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lvefldln.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vwtjkwuc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qjpualnj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zlejxgqx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pkdulbfg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iwrxawsa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ezvirltw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tuaxdmfy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rnmvehem.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nrdzgxnb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hudwlywa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eudvbxnl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uumhbpsc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dkrkugvn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lutssuko.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jfxcyjbg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3erdkziua.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjsmvyqr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hnvhqghm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tlvzasyy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ujhazovi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bbkxvuyk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3anjkfxht.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3efqmvuwf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3avqogjcr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3byegejwn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3evwsagmp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrtltvub.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aooedoyf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gquxedzt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3pjhpfrrn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3foxdcbnp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3coltjohx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fzophiqr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bxurmywm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pasuttzi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yaavfedc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3oiblqtkb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vguzcqzf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wihbxqud.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3iwxfjamz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vtcwgsfv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pcpvkkwg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpaqnpcn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3drljclxd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbthaymq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iuimmkih.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwhfoqhh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hsprqtqn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mhdlyvom.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fwmpqstd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzmfeyqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbkmtruv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dmoqzeza.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydvfucvy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3vebbsukb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ytyuvjci.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fvmxzqad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jcejwaww.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yhhppnff.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3atzwckax.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3joizdciq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfapzemx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvbiujs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vffgdvgp.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3izeixlyx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3krykzghv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tmfcwchb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3woyyrkbf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rikkvqlh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zqhnznhc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3canddiuq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hnyzftxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qygvjdru.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qqunhrgw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ljgmwyeg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lhewquup.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kuvsouaw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ytymnxqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zwqsvuwa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xreypplx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xnuyctgi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ikakerjc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3asivmqsj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vzrzocaq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oytcacqm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tzjetmyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykgdxavy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bgjakdql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyjttymp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vmerdgtg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdrruc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3xgdvjrlz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jclvbtsx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gpwzqffw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eddohfmy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zksmsrom.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrulkyp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3eqezdizm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3olenyrrl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wynhrywo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dnfccioe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kbjixipv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3diqibktp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xtipdthy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tctoapbv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tujiyndj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtsrpb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hwwgxpmh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dytkynmo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3uyoyfpjl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hxyqaaaq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3agfcurqy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zhzsutny.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pndddush.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nrmcpcqj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dnhjhzxh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3pdjvigfr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3afgjgcuv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cqvtoqkp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrotwjdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3godhnyrp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xwsqqgux.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3frybwgtx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yygnldpo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nfwmazam.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ecbmtmht.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgzlqnk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jamfrnis.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xroofkcn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jllcazuy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3eykodzzh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ifgxtvxn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3barytxxr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3doynykjf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3duemrqvk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jwdrjnkn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qrdkeqvh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pzjtqqhm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wrtxgery.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tioofcta.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vywdhdcn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zhcchrsp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iuapsfov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdenywak.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3eldxdejb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnvzmtsz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bdbbizju.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wevztowc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fkkwmosl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wifdrknp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pqtmvjsp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ubuyafxw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pvdicyux.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hoeaizdh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3nwzjkoao.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hfvkrdia.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zqwyedxo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfgiwlie.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ylxoueyj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tnkklwiy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iuychegm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lsdbbcpg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovnfnhtx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dbyzkanx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqoqeyse.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cwdypiow.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3bkbdtlky.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cizadjjc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yvnvzioe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dsnbytay.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xfiwmiqd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mcogxfzw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3waflomga.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3famposar.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3kphpnnoo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qhqgignr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3auobhvvp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aggfbmwh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qwiofukh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ufojsqmx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kmdbbwfe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lnyghsih.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wejrnxwy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ogcbstow.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qxysxiny.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3aqvikmri.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfyhmmo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hgaktlah.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3duroppfl.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cwxhhwlh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fiaqgvta.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nknqdrds.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ouzsgjdg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnyrpnnd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sbvygcwo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tajivwip.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xerdxszs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jzrccjxx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tzmfvyjf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urvmkrug.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3axpxorwr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zybqcpiz.html


<!-- 参考信息 -->