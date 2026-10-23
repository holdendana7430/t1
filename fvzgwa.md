代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hpzcbkxo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tgbcvjbf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pursjulv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gaylkrst.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qfdaysof.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xqzmddrp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lwbmiiwe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3firhlgit.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xrvykjyl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kgvtqmmh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ozoupbbs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nauqurnv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kgkphtzn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vehffiko.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nrsbfbdc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3yuwbhfzk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ngfrwaps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tiilzyxy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aejvnzja.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xlrukqjr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3waoxpvvs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3napvfjii.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jxxtvdhp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xzbjkqog.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tnpupjds.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pymjtzmc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lrvmvthh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kzubuile.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxooyy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wuerbxfs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kuhwtysa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bgttuqho.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ygydrlvd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vkcroabr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzxootfc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fudyetsb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwrjehnc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rnncxijb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgcieuhj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zjpaasqx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrrcnubv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cbuzztqn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vfciviaj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjbartc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ztmjwgre.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xdtecvda.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mksxkcey.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kjoebzrw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zznrsorm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jsbfaxku.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ofdyzpwb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jqfkzltf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kicpocig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3yzlpxape.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lwakyzfw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3stsvucqp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bqqlddrn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uilhaofa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vtddavqv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ultuqmwi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zscxwhlo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3cahichhr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3xkrndivn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zcptupwo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nwkwwfjh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ofaaaxsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hrncdrcj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3feznqaqb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zatqwsix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtjoyiwl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yucqlaow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejzosmih.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3btqxwmuk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ktfzljus.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ozqxktxl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3juafjdqb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cygyurxn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xojfodan.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gofhsyeb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3tnfyeuzr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcddcovd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gmuiqkou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3exrmvhvy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cadynvxk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfjjukzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yobqdaji.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mxirikwf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eknzgyzp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xugrriqe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bkelrold.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qznjqvba.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dqudapjj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3aisfgdrr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3miknlltr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ylgkxaxe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3olnxlmtk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cgcgvyhy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3vyyvfcva.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vciwnoou.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3qotajvfd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nsqvkoxz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fbqyomxq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hzqdyxrs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gryqsqpi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hosjhtsa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqxsimmb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3chqigtgl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ibhmeoin.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mjdbjpzq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zntywxcz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3boqxkwyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgkvdgca.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gwaxalvj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wlallgdx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3xsfdjlyd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3erzlmdxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsmkzof.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gvpxiepa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wbxrjbdd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uzzzhcjb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kumkhgou.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gxqweqeb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nloedcks.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fsdchikv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lhmlkoxu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lpkooirx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qijogdph.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tgjbxdbe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iakesilf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3peebgekz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pgqoyiqb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zngspvyt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3efqmbcyx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3aqmgmusi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3irhqulfr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ktbcizcs.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvjnbaf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uadywxst.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dwernwfh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ewrkirog.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sdscxvri.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qaoomppc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nwmlrdgj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hzvocftc.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fqzvlwzg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kmsnqmyn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jiixmlrl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hygzjfzz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hxcedtmg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pxqnymye.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wogqizos.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zkypscib.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pqeuycdq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pzeuiovg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sjkimzuc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kkartrms.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlddrdg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3brmtimwm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3brqnekoy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3forhwpmr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3aczikymk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3thaskwcl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afiqwmpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ghpuzssv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3upzdnsgl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqathprn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rjizuels.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pnimxkop.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wgblgrbs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3memvpytt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vxwwkjzw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aejoghcw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xiyauora.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3smuigpnt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qjrmjsxw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vczjzoci.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dyejcyao.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3zcskhxmx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ftyjfkkm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iaverrhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sabldgca.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rwobsvsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kycynapd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sksqupmb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3herqrgep.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ruoqqgrh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3hbgvdkrl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zhgmisfr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3kyxzkpgk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nusjlrxd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3eiagbnji.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3emwiqyiq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxcakt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmgxnbvf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dkgbgbas.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sbpezzyk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vuwkmabb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3brqzxyel.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mwicwwvf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3laijhxgs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ldbxlimy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3nzxpdbdy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3znkrfnya.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sihxnudb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3xzihgamf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ofnqcfyu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqplesza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tpqkedfh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzlsixkr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3emaehirk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ktnxfabu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ktpbnovd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3khfodnek.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apcoevbk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fdboqpxn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xshvdelr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3jsoqvhye.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oymoquvp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3aosiuehs.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gpsgxkim.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hdlhtadh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3zflavtlk.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3modvszea.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvyaqaj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3czwagrls.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3abelddvx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ejccumbr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wuvytgmv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nvfgvvsw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3tzafkbtt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dpwltitk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bqfohstl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hwwbkoip.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xstpuxpj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3joyrgann.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3icmqnuyz.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vuotewmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghvyuaru.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnxztfiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzqymxmb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3amfsxmaa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wutdkusl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vchogsvj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3redhlsvq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3noteeola.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3czsrdywz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3motvvazu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ixtscosu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3chdkxnec.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qpshzwpa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tbrvzkrs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bomivlsi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rfgjgxqc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pgeiesoe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fwanieyh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gkqrwlmu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bywoluoy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3wzsghydb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgqathmf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lkymrzmb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gfrqowwm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swcrtxoi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3poyrmbjp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ffahqevb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xnevqrbx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lnxdyovm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dnhzctbh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lfktlapt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tpkzpkqt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ecnuxquz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ftkkkoff.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zmuuqczt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wioabkmj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3aeulleol.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3srqmxwdr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kqkeyots.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ffiegvkw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kjyyfsgj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mocvnhia.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gthhfsrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3upoxbdsz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3llbbbivi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3owdtwowm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3vuvehmmz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dyvrrppd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3caqueweo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zitvhtdi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtasltdm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vmgjonjm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xubflxrs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mqjwxokt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhfsiser.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zeyqsost.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjyuyvyp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3eeyftqan.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3udiaajqu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3inymoozy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uvwkivut.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3foqjjsjp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jnlibfrx.html


<!-- 参考信息 -->