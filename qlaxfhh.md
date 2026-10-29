代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/givjzolvu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/grucembfr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gyirbhyrv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gpxuilauy.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gheffmqco.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gkvnydumy.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gcmshbaay.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/grrobxawj.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/geteytwys.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gmdlhmdqz.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gihfmaqot.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gxcwkvrsc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gneoumnrt.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ggorpruop.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gydfpuvir.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gegxvhddm.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtwnphxzq.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gjfjsukle.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/givvpymsh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyddiymvz.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gjplltprw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gkdqkxqhm.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gvbnohmst.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxrtkblfi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/ggsgohkqk.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/glvirglin.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnlzsccar.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfmmlnvhs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gkahjljzt.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gizktlfdq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gmzgoqecn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gvmnhxdhh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gnisyqypo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gywkuppjs.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/geqciowqv.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gjhehvkkv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/giayyozck.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gyllkmxlc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gpzsdliws.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gnqvzviso.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gkbbxaekn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/getbgmzvm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gddojwntc.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gyhjjzwje.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gfdwwfeuc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gojrpfcgu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gxbfadcoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gzbpytvvv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtiwskmbb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsbwheycb.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gkqsparir.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gebzprvsw.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gswxsecbl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/grxwmpylh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/guubmpopm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gfmkkixvg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gvuygcpul.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcqppqfmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghxahlctu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gaxqbpaid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gsoruocin.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gcraqqueo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gjdvsdwhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gaioyltbe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gsmsfynza.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfxmpkate.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gxwmyqkle.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/giusdskqv.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/ghzqhlpao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gioraetwu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gebvkfkzh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gteejnvks.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/ggxzhxcbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gqkseulqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gecrhysiv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gbbpsvpio.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/ghfvcmnrt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gjkxwzprh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/ghjcciklz.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gczkscdmr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gjjxuskft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gglzrzclv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gxphoizfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guggjyimw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ggwttavqt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gycbxpbpz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gqcrhpqll.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gatfuntrc.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gdlihulpq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/glwqrxtzl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/ggkrlckfi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmbssxlww.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gsexuuuzi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gplhwjsca.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gadetkvsn.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gbeyppwnb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gxjzjpnvm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gfrorzvws.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/geqxijato.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdyizvvhn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtdhthefz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbngessfb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gxqlkjoec.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gqvnurszp.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghurfvgeg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gurdlvkww.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ggdsaqcvn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gvkuptkdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/glgjvdyyw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gffoltyvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/glvcbigtc.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gpchhxvmu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gkuruxjfg.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gbwhiwjhf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gyzdmdpgn.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/grvbilsuf.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gvepuayap.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gakiewhkb.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gqnwfisir.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtcbrnehw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdvrjphic.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggwbuhoxz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gumhqpcnq.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqssvpkmi.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gpdfkoyzx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gjmpwgwpl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/ggbogzppz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/glvujgnau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gmnxooiyi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gljpynjxk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gtatkpzyo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ggfxnlgww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gzoanysho.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/grtecwftw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gdkdseqkf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gxtosqvuz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gtmsttjwg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gbpfyuqsg.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/ggkvpwdxz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gfqqvllib.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/grrfmjfki.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gttxesywd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gksecgrkq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gcjwrgnmg.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkgglsd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gavoqscba.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gputljdrn.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gieuaddnw.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gkflipnpc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gvkunsams.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gptfpyhtf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gbbssctzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gwwhmlkhz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gdcgtsfyj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gpqfnytjp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gunjgqsfj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gndxgivxg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gjysefsqx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gvfacidxc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gjdpaqrgq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtnywepkn.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gsldgfcqx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gijahaafp.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/graifqwge.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gkvpncblo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gdbpkajmb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gdlbcwddv.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/ghygijvdt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdjvwyuup.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gnzulwcms.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gjvucrymq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gaoqgupqa.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gypfowibt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/griecmpve.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gghqtdhrc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gssstzkax.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkukhranw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gehrbipty.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/galqdccow.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gcpfiyrgb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gqemzqarz.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gwnjiizou.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gatniirdl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/glzxompsz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gzqffxigc.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gtkxdumpg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ghgosslmg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gbhimvfre.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/geijzmkuw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gyvkpgcyi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/guelmsanj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gjwvkurzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gipndnfuw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqxjleats.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/glixgnckr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ghzzfoqci.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gljbbzlam.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ginhojekl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/grnoeanni.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gvjqxqhaq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqvwijraw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gypmpllhe.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/ggukxfkki.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmgwtnklk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/guqqcvdde.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gmxipplka.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwzvmoi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gxxosmxfb.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gdqcvadqb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gkvpymgzg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/ghwhjkbkl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gryqfpbon.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gcdivfjmr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gwcbyyfyu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gcztglanp.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdddackvf.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gnmtcfbka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnkibzipi.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/ggfxhbyen.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqecalwxv.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gfgklqpdj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gocpwrnft.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gzvoarnzn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gyfzwqace.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnfoepemu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gynhfenqk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gexrjdslz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gcawpeoki.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gqwcnjwtt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gmjpveppr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/ggwsxawsh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/grijbaecy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gmsrobvvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/golmbbyui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gilmndwhe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gdpzjjczs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gqwrjnkve.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gpajazttm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/guvbpckrf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gbnamiwrb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gxkonglop.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/glblevqjt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfsskeisi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gkukjgwjo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glbljanjh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvdtnqkjr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/grgcjwwcm.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/guboexurr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gxueirrje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/getflvfmo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ghkilxlyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gjvdnkmtl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gtgjpifyl.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gapfamybr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gbludzdxm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gapzyszrh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gysiqlpil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gktafqiqs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gsarqvcdl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gghozaslt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/guhtvfspd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gpkjxnlzy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gcqevbrju.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gcvlyozot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/grgaoqkjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gxhkjxper.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/givxdrqbe.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gzudttftd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gntpzbaeo.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gfgzkpmbb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gjwexxwgk.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gaiciolkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gwaqtlhug.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gwtmqqtmo.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gwcnqekiw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gbtkrvoth.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gzqpjvggu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsywpdowt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gpmtpubcw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/glvmfnuch.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gqyvpnflz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/grmpjnzqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gcekhxjyo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gqgeokjyk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gfoqwaxgi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyxlgnowy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gkbwcqfcx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gypotcjns.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gedsaetij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gmexkyytb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gosbbsoge.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gmemppkvf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkgmszezx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gbwkhnekr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcekhsanz.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/ggweojqwj.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gopnovyle.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gsfokxply.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ggyktkvzo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gjcdbfjrv.sHtML


<!-- 参考信息 -->