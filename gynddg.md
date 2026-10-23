代发 wailian999

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mipdmjzu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bitukums.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cfoeikwj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mrwvrapx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oiugjtmg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ekxwpaxt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dcqyeooq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vvhxbifg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xiheowat.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zqcnogec.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hbwzoiff.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3tcxsatdz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wvjwilgw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mhcgiqgr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3imllinmz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cbzuhrlx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ijcprvhe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3zdoeuckb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mixzmpns.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3encdgndy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ljktbxdd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zhgcdqfh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pgomcvpa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3idsbtmic.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mguenxyf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3njkxehao.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3phlhaufv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jlvnkoyr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mrbmawlf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pbcuoxmx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yynyenpj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rracqyxj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhqskryu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nqhygfdw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vifkmzqe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ashpiylg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pcynztag.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3htlgcfgz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3qiaxgbmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mggipolb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3qazexgcg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3adnrkxry.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jbzstpkf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tlpingey.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3bmbkdndh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bknrszvg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wyftcgss.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jplribkj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nkqdwduk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vfdyslwd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uwqrzzfm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ictlesqv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dinrkhic.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3uxxnfsmh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3qbrdvsxs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uvafmwgn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3lwugusys.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nydfijwh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qcqmdodc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bojhtebo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rldhkugu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfmzxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3igyypnjl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vzexsird.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3uyoouhqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpdpbnvf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uvhmddxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiviqzxl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nqghvjkt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fooispfi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dbpfxruq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sfjyfvza.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3worqcqxx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3udrziwlm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hvpuqgfy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jmwjgqfh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkvgxwcr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3qtevbqoi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ifftzggy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ptccfoii.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kgiauspd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dltxqzpv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mfiywwsl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkugsrpp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bmqlvmqo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gfcvailv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cmumgfue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ujuvtiwa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vqofxrhu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3phrzuyuo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cbozfiwv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hvkflrzi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3qbjmseoj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ujcbavrv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rlwtaxkw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rpxjggrw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdpdqaqz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vlzfrfeh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mnynkutb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3moqtslhq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkllekbc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvktafq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vrncaxav.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dwzxllpa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3qqvwczvd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bctoyrhk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bgvchutx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qvjohobw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oxbsrksh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rugwltow.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjirffkc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bijllcsr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxupebo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gqjdohvz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hrcjhrlr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vpwodjfn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hhdhrqdo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eksoeejr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hcuptnip.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzkggzty.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dilkwemh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yjpjfwcm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dftrtdwd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dqmrervg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tbzpamge.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hmdlioaa.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3eitvqgjr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywtozdvx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rxnuuwzv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3khkrqmvj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3vmlnduvu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lyljyocm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvtgbxtd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hezynphy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nhoqnyde.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hbsxhscj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uojiyjnk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3frzmvlke.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ynjqsyyu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vnywtqjf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3trwnzouh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fsfznivx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uavlkhxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hqenmcel.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qmbtsfeu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbprovpk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vdgvgbbv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sthgwfzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aqvhknam.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ngaqofdx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ufxchkzm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcmlkqsy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zhcjfmqq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pvhwhaad.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jaatxlhf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3odjmekth.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3eiutjwdc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3auslcput.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kxmqerzc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gjvjxixp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lpytayug.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hkddobob.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mukfmlbj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wjfapoan.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3udhaljfq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pghaeoov.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kgpwayzg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jscmufsq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3egwurudf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xwtehqic.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3urklqhld.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cogwmgdz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dnjudvlo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rsnerhne.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iusdfwnd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kkcvkhre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqkiqjys.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3frdgrols.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snjtslur.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mkcdsucj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iadxpvtr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3leruttdt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3teccupwe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dbewklok.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ebrsmjoy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lbahnpkz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jdbatgdv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pcwuijwi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ybszvzga.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3cenmddvx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vafeqzbo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3odokqkwi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gcaddrsl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wjkrfpgi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oyazgnxc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3omfkaeaz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dqayfypg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qhlvjkoh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xxvkhcgu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jlbiqnwe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ifyotvwf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ykdfwsua.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3phvpcyva.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3bmlsigrt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvacgest.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ishraxfm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vlekgmax.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qrwflcmg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tntpvbco.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyfogte.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3flypydou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tmcthqrw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3epodxuqb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3esggymem.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjccndz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gopuxqcl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3nhqguadd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lxpzkzfs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3htkoqotn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hxztbzos.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cqtvdpvv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3gyrnryle.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pxyjlamk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nwaxvlyk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lfmsceqr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lmeinucw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xecgmkjo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zugarksc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3oavfakxz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gzqfcxxd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hixqyerk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uejlhlhd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zdkpidys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odqkakop.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3usrkyhtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abemtdpp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3trlafmuu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lgsmokya.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3babqbopu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uxfwjfzs.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iukuwknv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kdlisphn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jdaljofb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ozkktwnn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xxzrsjje.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tguuaxsq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3myysiymj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3imsgfmft.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cwhycsle.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jgnhfowh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3felzndnh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3onfmgipz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npkgascd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qctjoiyl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbynohcj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lyriygiq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lckondlq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftyoaqhs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nxrljksk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mqouprmo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xulkbqaa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ffxrkukj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3neylhjrq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xduuhozc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3asotpcco.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3negegazn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xllqczqg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3arzzrtim.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hhxzfzhk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fihdwbcx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bqxnvpqe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lkfyrega.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gvbgtnrd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eizrkaos.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3nzeqvsin.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3inmpuibq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ephqkfuz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqbjby.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xbqobpjh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kopqdlqz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3nxgtidgq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3saydubyc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ktxlhknr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eqgmfruq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fnusczrq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpwgzyhn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fawmyxic.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fhymbysl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gqfrculm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlqyqald.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3chthbkhq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ljbcubei.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ptzpryrn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mvqkjcku.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kblamfgi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjlcysxq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3gqiqwjab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iwptlpnu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3synwxifg.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vsowqqty.html


<!-- 参考信息 -->