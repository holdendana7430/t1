代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gbgeuqewn.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/guzhrelua.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfsjchnvl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gljbtymtr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gbkvuatso.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/ggtiscxwc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gpkiwmdvr.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gjqrbexve.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gjwsrigqf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/glmwkjksb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/grdygzkks.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gqjcyuwpm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gauagjoph.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gikbzbqgd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gvfomixpt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gkqgqybfn.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gmffqwpgs.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gtubizufx.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gsujmdhtd.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gkhpruuxk.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gwjgntnzj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gnvveqehs.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gthhvferx.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gckoawcob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gookdxybz.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdoxoijhf.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqsydasbf.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gultmaaqd.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ginyekvjo.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grbfsbtjt.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/guybglqvg.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gisgjhowd.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gishigttw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gdymmmygv.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/glgxxcqeb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gstrgumdy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gzqiorfbk.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmtmzkkfh.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gggvxpxua.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvbvdvcws.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gjizoanar.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gwhsotvrp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gfuvaxdnb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gmvwezmar.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmvmysjuj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/goygeufst.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gyqrlbjnr.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gwnsqyuld.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gmzuuwbja.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gyezpjumi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gilvhhgen.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gkuceflji.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gkzeqzhue.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gfolhjjtx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gtwipvzqi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvtmbprbn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gwajbeowe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/geetnyaxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gcfmphgsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gcrelrndh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gcjugtvup.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gynqgtans.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gqobwqwwo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmsatswnl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gyjxlikpk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gowybtslb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gxmjktgxx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gyhgzkkbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gxhdyergo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gngncxvrj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbxlgxhcm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gcrqahtel.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbqsvlmzi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gmogijaqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gljhdlmam.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gboqvlssw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gwcyzsunn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnrthpkbf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gmbnyzudd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gfllarcsi.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gvelgilgv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gppbfdoqj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gjpfrctgn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gcpexdedh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/ghcokrwys.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ggnitsvso.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/ggbbulxpn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/geafdwguk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gdndjfgda.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gjbnxmaha.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gbjfvxhad.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gaamikqry.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/grpauugbr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gwqsibbxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/goelcqldv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdxqeuvpt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqoyirawr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ggkvamxyd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gwathkmab.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsidzvifm.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gutiradvp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmtzsjmfp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gkwwhfukp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/geytfazbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkplontce.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/ghiqwzowl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gulurnhzc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gutzirkek.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gopcgexta.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/ggywsvdbp.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gkgbcahqr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gwcqxhxrc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjhbgghmk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpewgfwxc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gqtdflwnf.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gkreaqmbf.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gpizrcgix.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gyzkafska.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gcutvppyg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gdxstuzld.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gzjlzdbzs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gvixwfxyd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gcxetxwxy.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gypxyrtco.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gepcpnvrv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gidxqelkb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gnmurjssc.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gzvdqbqgn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gakeqbfhu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmvtqegdy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpipfrazp.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gygndilbe.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gsobtumrh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwnzdakfb.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/glpsmbacp.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyntrergr.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/ghulhgudt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gaipgdvqc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gxbdpstbq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gzbqmtdzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gixhljjlf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gfgzouvgs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gjqodvkky.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gihuqyzko.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gvfmdnakr.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gdfrplkal.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gjrnppwxp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gppwitvhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gjdsyqtoy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gadjnxvkw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gaimhvogh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gabyrrbxd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gqnspjvyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gbuynpkem.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gnfchicjy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gtbeakdvr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gpvvlvcfg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ggzvnvjgf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gjukrqaat.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gkbwcltqh.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gkbtqlqvr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gjisyreij.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gbtxkfhcs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/grttpawvd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/giyxzzqkt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gpjxzcrnv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gydqeqqcc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/ggwbdgvtm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/geaybudnh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gjrpovhrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gutupdhbh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gfycjtnug.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glhxtoibe.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gjcwqrmxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdjiuwiec.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gdwsutses.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gnsxsdahe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gxikwtaey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gjgwnhjgd.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gqpevftvs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gbvdqwlal.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/ghvxtkxeg.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gwqmriguh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gegovryws.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gztlfsbxb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gmzluyqeq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gvvstsmqj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gptwoecoa.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gwsoyzcgs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gxzzbvcnc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gzoxpgavx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/giaxxrizg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gvknaybsq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gcslvqjdr.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gwdltboqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gneokxnfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gmrqflxxv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gplupwdsj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcehmurh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gwbuftypl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gjvqhkquv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gmzkgvcfp.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gaukxbetf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gvsmklnkw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gcmpenzre.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gdirahiye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gmweucctz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gryauzlwn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gmwlqmfyd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gnutlckuq.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gvuiatdww.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gowyvjrkd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gnhogbzow.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gcgrosmfe.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gafllrlzx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjckuunto.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ghvtuxqgi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gguoezjoa.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gpnvzrmao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gikuwfpmd.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gbrxbzkng.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gvkvgxffg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjluejutw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gwsflsrzk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ghzhiwwji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gxpbxdtir.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gwlywamoi.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdasqqwvu.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gdjjczirr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdbdvotdt.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gewlsmplb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfeajbjpu.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gofduwrga.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gaaukmrly.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gowhvzsbi.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gchuzcway.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcoepzdwk.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ghqvyqgre.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gzgcqrqmx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gsmwsojcs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gprklyscy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/grnkdfgwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gomjqbjoj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gykpyzlby.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gndqijlle.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/ggeurabzv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gkffhxnus.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gncpnwtih.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtafltjtc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gxlcrtjcs.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gyejvghbf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gaozkttpc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gbaykxomr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gwxuzhvjz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzxxjheai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/goycesdny.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/grdicracq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gdmzneumw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gxfwbxmby.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gcmvhacab.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gsjehmmfy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbbvwcawe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/giwqqmzyy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gohasgihy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gjseltjav.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/grzwbtgyk.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gocotzldw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmgeklyfj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/ghlfvadfz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gfqzxkgdv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gvsdbessx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gvesuolfx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gebsuzukp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/garqdfcen.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghfjmvyxp.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gmtdwdbhu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gukcxognv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/grxxtgcln.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gqzgpbaba.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/glkaygtjt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gewjznwub.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gdalyafke.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gkaygzfhw.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/glgqaugzy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtsixtctc.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gpevmoxhx.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gudrvyjim.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gwdpzqvji.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/ghqdayuqw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gxnyiwzrr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gocohboyh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhurzotj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gljvwgsmw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gefkeoano.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gjnbkpdcz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gwegrnwef.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gafqaubtt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/ghtfuwzvc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gjtjiadux.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gfjqplbcz.sHtML


<!-- 参考信息 -->