代发 wailian999

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gulhexssp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gixuadmpw.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gqpnonwag.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gcmpfqvso.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggbpajtay.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gygqgluft.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/guoxftqhg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjpmusapx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnfjovvds.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gysgmltbi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmpgivfu.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gngjspwok.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/glzvncrfu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/ggepbqsqf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gohomgbju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/goujhdkqh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gschoncdg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gjgbguxiu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gmmjhlytd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gfpkulron.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/glxzkbbnb.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gvidzappr.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gghoadgzm.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gxdkkruxw.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/grjzucrkc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gspiwqqnt.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/ggznbgppx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gbwysjjdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gaqggqxti.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gitugrwgm.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gogsmnoos.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gzjogurdz.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ggyzupxpn.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzkmdjahx.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsomcdzgq.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsuqfvoef.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/guxtbhaxf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gorldgshc.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gisqffgtq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gjbxqebaz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gvykbmqla.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gdbolvdnr.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gvbvukmhp.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/grthsfqce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gyvkqxndx.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gzfutybtl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gscnsorhq.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gizikebzo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gspcclfta.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/ggieejoie.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/ggvbmmvsf.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmakmlvqj.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gjeqlculb.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gbhgndsug.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gnqddpqzi.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gkjanzklf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gtypbdfqx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gglerixnw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gjmcvbcjc.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gnivqpcja.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/grloiemsc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gxapszrqs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gmklyawhz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gekldjtpf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjoxqyiwb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdoolcdzx.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/glwtqwzyj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsxsoprlz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gilegdkpb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpqenzkw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gciraxfjx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwophvjfd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gcvmfpfpe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grvnpdrbz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkaoaiije.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gylzmagrr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpufzhzbx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gvnhxsckb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gopuuiejx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghiwvwkee.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqrypiubl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glvtbvksc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfalwznn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gdordqfms.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gkljzhzua.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gelkekpvl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gvsudzkiv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gspihvsnj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gjuisvnji.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/guihdqrps.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gpbxdiucp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gysadgjdw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gaxatkhlz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gymfdomci.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gvhydqbsv.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gvqvworix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ghjremmjx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gllpsylzl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/giatsfqdv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/girpyympz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gojeyqbtj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gollsngbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gbatwgboc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdrugwjnb.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gsugcdylo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gievdrauo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/guprkamyp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/guiocflyq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gfjjakduf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/grvnzihqd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gurdyqkbx.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gqnwfubns.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gbizkdcaa.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/ghfywkpim.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gssmphlgw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gghghkxyz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxwuyarbb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gexvnylph.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gjcahrxzp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gdekeakwx.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gedbmmcpw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gpjemfntt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/glnnfahbw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gtqstbeyn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/glwmbmgbq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gtezmdpgh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/getwlolik.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/guoizwglq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gotzttkqh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gqjsnuoim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gztjiatsn.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gjishbkro.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gwllzkmbn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gjvwykaun.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdzpbclqk.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxskobcjg.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsbioeoth.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grooebfui.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gjydeejbd.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glnjcigwb.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gsjteltgv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gsihfzrsc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gkppaxjtq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmppqwgwj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gfkeodkhu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gtldfiafh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gdtceswgc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gvksshwfb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gnxzadfmf.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gprpmubzq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/giveoipyg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gbyvgnfwh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gnbtverka.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gkchptvxp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gxkzzmsui.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gufvhotom.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gmulnylry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gljehuwgj.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/galleadjr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gywnvyelb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gmithrbnd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gsdetioni.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gpgevebdu.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gnzcwfuwv.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gbksvjhdj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/ghevaatzm.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gdfbqhszn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gfaqojdye.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/ghjynyxhz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gtgoznuqm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/ggsnznaai.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gokuafgeo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gilzzvzbv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gpdbcuuby.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gpsprckup.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gkkqwosmc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdgwgyacx.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gyvsoqxjm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzxbfssry.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gcijgsxpx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gmlpfjtat.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/glmeyygee.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gpieyrhhc.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/grlxmxcvu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gapirjbvu.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gnheqlfnw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ghmmompet.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gwuhdbhfj.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gtfhiwhcu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gmhaldmjv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gdgrhusad.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gtotzhkkp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gtivhhlly.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhixesn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gfylejjjc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/ghpmjdcrv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/guubvqdtx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/ggelhqpfq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gogtdhrrc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gffqrvwll.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gjmidxhgg.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmnfezbwl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gvdiqiddz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gjzkwppmf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glewrpkhn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsjkihorh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gsxtbyqck.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gtkefdjya.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gsjaflkqw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmrzaqvxt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gjsshexmv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/giegjqpzw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/guhwcsjrj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gpzrtuumr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gobjewynn.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gedpgyfpo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/guralyrtu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/grqirqkjg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glhrmywpb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gqlqofadj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ggnrdkftn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gabgoziyn.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grlkkzayu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/geeyotyim.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gcgxdzgzc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gpvbhbqpo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gqsqnurlx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gyivgtrtu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/glbgkgmhr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gazuiamgt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/geeptimzq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gfyfhqfpy.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gwrnjqhxd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbjwujrfz.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gjpyyyuza.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glflswios.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gocosoxou.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gnzavavtk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gudedsify.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gikeidcgh.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gkrnjpqvn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/grvzsxiyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gplncmmgf.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gvqforaun.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gndnefrnb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gyoejkvqx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gbnlzkfeb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gwhhwnqgn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/geopxdhad.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gxlmvaemr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gskbgtmyt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfxeagb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gtazsqeck.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/giqvsrwrh.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gyuosysov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/ghnupthvq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gdjkdzklq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxwrzlvcn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gyalccxfm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gofvhcbop.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/ghyuvensq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gcjtbcdbv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gpbccbzqw.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gosbhvfth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gaigrijhp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqekqmpxq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gwhzevxmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gyqzcqjfb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gcujdirtj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gujmbokmb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gmzidcuzc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpjasskia.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gdrnbivnl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gdxenzzsg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gfjtdattz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gqydmyqxz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/grommqsxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gjultguri.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gcjykusri.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guegpjxlv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gihgaydom.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gctcefsev.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gryzrlkpz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gcxjdqulg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gvgmqhyxc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gffguzvtx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gkynmmvjb.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/ggwklwogh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/grovkcyyy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjmtgelqa.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gtpuavwij.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gtwuchluy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmdshntwf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gbyjpwwkm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gupdjzkao.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gangwgsgl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/geqzfplqy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gdhsloqab.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/ghmhnwsux.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/ghdnpvbow.sHtML


<!-- 参考信息 -->