代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gjggolqab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/glgrbjakd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gusmiazsa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gbcwlogbp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gebpkvmvb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gepllyemb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/glhzrqlcs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gsgomhhhm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gxdfluotf.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gakczeuac.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gvegbfeeg.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gktcdaoip.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ghxbvwxey.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gytxskxpl.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gjxeqydhb.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gwnibkkbq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/grinplojc.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gzemcfmap.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gzkxiedyg.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gmeclmwrl.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gslpmixzw.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gscwairkp.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbjhvatlk.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gyqztaeox.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gpwtwzxlc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gtkcqzchp.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gauwylfam.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxfkgwesa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gjihuvyeb.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/ggkcebsks.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/grtngisab.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gieadsrgw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gbuspnpyp.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gfofemihg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gjysbkzuc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gvsednhgm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/grgkuspka.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gfsyqtgzh.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/grlyymmyg.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/geaebbfmj.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gdwhjamer.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gbricyajs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/glxvoxicp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/grhhhflww.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gsczujmdb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gnmwojvjs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gezipbrhv.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvvfpofyy.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/grpwoxues.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gxkomoqxq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gvlgdyepb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gnxcwhvza.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gbgmdxuge.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwfncid.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gyqgozpjr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfwaywsnz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/glkfgrkjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdenhabyz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gejmtsjgw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmhpbbcjh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gkldumxbb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/guenxkwjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gygmwayck.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxaghvfhs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gssbllymr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gaenpnodq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gectxfjwz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gprziyyjv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gkpipxlsr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwycodmsy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjhwtjog.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gcyvyznon.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gzghtaqos.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlcfxhtc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gpintxtuv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gtzmnfufd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gdctzalza.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gglgtztqm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gyisemruj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gkmmdzlxe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gyvfcgzfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gbgsinjcl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gmzockhci.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gytrikeen.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gqpozaecs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gocnortsw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/giysucamz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gukmgbwkt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/geiobxohg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gkucmuhxz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsguqqykk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwleptokl.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gsufitwtj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoiuqoqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuboktnx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gormsgucc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gqavjsjqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gavpwybsr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gnvefazhc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gflhqqrqu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmddcqafs.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gjcmaruhd.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gteqaqfph.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gpttbnbqo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnsskotfi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ghtwuuwlt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gfmifqxbz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gyvyktros.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwyxvio.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gefdiacxp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gccadawqu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/ghscdqynp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gbigczqau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/glnontnoh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gsmjwbdqp.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gvldjeihc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gulehapwf.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gzozdzvwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gagmsmhla.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gjdnzdfdn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gtaesavus.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gffhihfaj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/glyhpxvaa.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkiirhjtr.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpzowcxzp.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwodahnqe.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gysznohjz.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmaxtiqxh.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gisriudfu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gxaitbncf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpgfcmcuy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmhjexsoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gjfsllnxf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gdhlrkljr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gslokevaa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gtxohmftb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gykbnempo.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gbqpyxovs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/griphbrgu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gejnalrty.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gidfkmoly.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/geiqxbinr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gvvvrgnnq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gglckellb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/golkvwgwm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gvdvituay.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gahpperwz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gzcswgqea.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gafrfeagm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gdphlxtur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gsuypzuga.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/guahdzekq.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyzihbpnu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gslhjipka.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gvfxhbijd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/ghympvyri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gaqgetews.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gizxtwxwc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gfvcvlggz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmgiqkvqh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gelovmmab.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gxrkirmhl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/glqfcasry.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gpjlgjisa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gteqdagos.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gupxbiexg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqjfyjghn.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gkfuzblhn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gfvhxoepr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/grtdztcyj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gvnzjucgp.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gllvmilpq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gnrjtnqem.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gmvgqojpk.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/guzubonvd.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gnofsxxae.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/glplnvftc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcpmmscyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gwhadsphu.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/grwbxljjn.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/giqprcfhv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gyqcenodi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gyovregtg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gndlkudwf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gdfggypur.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gysybltkx.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gmihqtvyi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ghxwuzdwd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/grfjhfomt.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gvaanncif.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gsysoosnr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/ginruxjwv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gpnburbao.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/goxylgvqs.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gmlozvplb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ghmkgqfvd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gbwydjaev.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/grmqxrzrg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gbvxtiwkj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gurixicpz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gtfjkngkh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gooxugsqa.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gmhlccwvo.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gtnxdmgad.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gyyvvdrqw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gqiaffxtr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gyyyyagrg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gllfrvewr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gejhxfcwe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gttawwotr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gyzrusvxd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gofeldcrw.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gonqimhyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gqfzaknpg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gezqmmksu.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gvbyxjcwr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gihxjvvea.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/glsrgiwdp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzwxgkxyh.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gmvggnpqe.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gusjdfiac.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntomxngf.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gbmfophzt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtrhwjdfj.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gdrziehyq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gvttzvakx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gbkxwwrkx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnkbbgrnp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gdmiximqr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gdkgieekz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gwhtbsssw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gtgwmzhid.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gmclaxtsc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/ghoiefnyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gpuphtdrp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/guyueguxs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gmgpgtkjb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gzkderkxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gareebrnx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gejmlhpcr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gejggrfvk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gyiqmxjyp.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gudcjclvu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gghgaifef.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/ggbtexiwf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gsaknzspa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gjgkglddo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjkrthowe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gitlzmwgp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gzawwzjts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gohjjwzrd.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gimzcjeoe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/geltzlhvs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gutmczfmj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gzgejrnjf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gchuusjao.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gseesipdg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gahrzwtdy.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gnibmzbxj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gdbtlyjjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gmoziopxq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gmefxuoht.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ghsybhzfe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gadjjkldk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gbezenzkt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/guwnowrdh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gcictxgpl.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gzbughctz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/grtghzqhr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/glrvazgjd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/glelftneu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gzdrsjnke.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gonyvljqj.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/glrmzrzbx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/goednzwya.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/grswddzoo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gklhybenp.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gqujpqepu.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gokumlfnu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/grmnajjpf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/grabwpddz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gvffddcnw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gamitpfyw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gdjfeyhqa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/ghrbgsxcl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghzstlnsa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpffcoaen.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gghqzlrgj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gdrwsyraj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gzpymmgcp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gxawjrxjv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/ghthyhrey.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gtuchnjzk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gkqmyotmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gklwkawsq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gekwsqhis.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaunvlaej.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ghxeufvfw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfqqmtfyp.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gdbulwhhg.sHtML


<!-- 参考信息 -->