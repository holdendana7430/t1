代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3goqixprr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kdjmdtmg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rdswtfxs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nrhdbmjb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lezvnpnh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rxkjljev.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuuhnty.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jqfljwso.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmbwltl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hpytjktl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zvyznmqs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iishkqfh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xenlfqem.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qwvewbmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zyezvavz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mqbkjoaz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uuqogtgg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gbjdcanv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wgonwvci.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bqafoykj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rjgcmyuk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nmoldeip.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3flrwdauw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hccexqbo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hicrtugj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pwqnplgt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vsbpsntr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3skjyaiko.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhnlehbe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zyalkfcp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvkjcerj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxogdpxr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibunksuf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kfdbdbcm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3uiqwdger.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uczehfsh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pjmqstkd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jevosicz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qocrpzya.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hmatjxfc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ukcohuln.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rvkzheaj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ixmkxfnp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jmqfvdro.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cgnjyqza.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hqczxkwj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vmccfbxo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hsxxkmxs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3svuucaay.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gvjcpfmn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uczplhpf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3nkigxfck.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rknztoly.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3mcwhhoww.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lloacyvb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iczrflph.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3uvwzjrpv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cfdtcqmz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3acodmblf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gasqjzou.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3chtlafjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsdhgwoc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3zyaiabxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhlfftjk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dtzneamf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjapsh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ufyddbhi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3unxuksju.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3osizoopy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsuyeam.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dznllrsk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3gzkvdwbz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdzoyzjh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3oryuellw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zjgwzzob.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ptustfnf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jykvurte.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbjbrvwr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3awglpmzb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3crtyxhqd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nordbrhz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kdzbtsko.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3aocwcaho.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3uedbabsz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3izypyfxy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzmylt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zkycoqud.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gafwatjd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mgjirmkq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hnerkiml.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jwzomuxx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rmxcnqox.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ixjxokqr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nwkxgtcl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sqlofoqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdmgrakv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iovftgvv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hdqqpuig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwpwuhy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uqbttxzh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pbkpdqdv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3btaprkxc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vnavuwaa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykemxepo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zucwgidc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yxbizdfl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfzamvq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ghysmprp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwagoynu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzcmzj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pvxhzauz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3gxitwxsy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bildcsfs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gtqsyvol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tdhugmcj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3sauoyomz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zcpvmlae.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3htzvjuev.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nomhdekr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3soupjjje.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jxabbhvv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xyixtrwm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jdjcmlht.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fhwdjxjp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pwycfilr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3xnqbhbuu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zqmcjbpm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tbrqixvd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pochngrc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3phhufoxv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3admbbkpa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qpppjavw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pyqulglv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jrjgucii.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jwpdtcwp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxalsnwb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vnvwrzua.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kzzwebjw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3umljnuii.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvdyfzza.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jxxthezz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tsmhymgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3djnwnwqw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rzmtxbco.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ftrscimb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3lwkdcwin.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pzmfigbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jvcteiow.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pviupzvc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uodkdbhp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3szrbdjvj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3txiuisuk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvnmyrn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3hdhnbmna.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bodudugx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ttfhhpug.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyncfdka.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dgsnysgd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mzdlibak.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhhxlgvt.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pwuvqxjf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ynoyvsxs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ywdgkrit.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hfmkynss.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3lgzqburl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vvmcdfxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dbuafmck.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dntconfo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3axvbradw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3grixyrxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kufaulxm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3khwmjtyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gosyfsyr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bzviimtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znsqcmhy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nbjklsdv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gybwmljx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ehnazcqe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xqelkuwy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hexpilpf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ahfextgj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bpstmhrq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3faoaddeh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3glatdekj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vadodnmj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wuydthtr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3sacurdie.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gmfodfxy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vahpqlhh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3aogxdobi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vxnzccqy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3oorrcrgf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3opxcuulz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pfmsjmrz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wdvdbnsb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qkooelzh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fvmgxelx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lackeeig.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbhpqksk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yfwjooro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ulyrjsve.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3thyehsts.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qxodtfhm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3gzmrscgp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ykfetnny.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3noyrrxgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idztqvfg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fkmleuag.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3krhkzjut.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pqzmhbbl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3nmhgnpxn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qbtczuat.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3blaglcjy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fcwgannc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mcqwmqgw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3erdtmfyb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3eulfrpnf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3itcuxwrb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ajsbvtln.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dffoeqms.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3iwisjdfb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nnhqphca.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfdyacby.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fxgwfuba.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qwhhqhsg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zwuddzfh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3abewhroz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3yzrwtxbz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3onlsrsqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3losacgim.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3etqqbuzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srksrsmi.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rfztpsss.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3uaamafcw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eagxupdr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3trjqmolk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3loknhosr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cpcvzwqq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fzbcztva.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3srlsfdnv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3imufidog.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tcxvjxqw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3bkepdqiy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bkzgbxiw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aswswzso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pbwjkxvo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vebdxita.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3udnfyrye.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vpwxlcai.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gqumzfqb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxtqut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3zpkyqxil.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fenjiyev.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nwaqfsyn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ftyvptmm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3txhyfdui.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hsphzyxh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qvekzsnv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dvtnbmyq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3pcvhsyko.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3oxgcvaxx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xrrjmifn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vzdtvzed.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3avafnawx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3azifawts.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xuabtvmn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dfvcymfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3orqovbpj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3naogtepw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tukzadpd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3zbuunlxo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3uybcxkrb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3leimcfhj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ioalotbi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tvngelwt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hfczfxrq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vmjwmfrb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pyavfsde.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gptmxeyw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txowlovn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gqgzdwdx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrneeiob.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3immgwzul.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfccmerj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tjjhbczd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdttmxzd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qchoxqxv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hjllssbx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gywfvzrd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gkgfqtmd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kzylmiyb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mpwhemrn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rtyusneh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ojbzikeo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3pppaqgur.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vbrxqnzk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3otkxfomi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3whozalhp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yjyxwfwn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyeetst.html


<!-- 参考信息 -->