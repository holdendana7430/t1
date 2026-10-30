代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/glhbkaend.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gxkwwebse.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gcgfsdxag.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gujdigynm.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gnxgjioec.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghmtikupt.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gudkzlolv.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gflvktibh.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gzohzwacq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/guxqlxmqt.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/glatgyuhn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gigpfpppo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gppbfialw.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ggijgltfs.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gzkocidbs.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/glurngaeu.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqpxwbiup.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/glausgqdh.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/geqnnlpqk.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gaetiathr.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gorwqwyrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gjhpzbrde.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gygbfwkcg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gasxtprkc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/glkqvnxue.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/geffhfkhj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ghzdamqta.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gnvwhsvvn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/ghoiqzhqt.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gvqfmxonp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/glweawmvq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gymtwcedi.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/glwopaoet.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gsqqquibx.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glpusdteu.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmtlrkapl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gpozqazad.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gdxkdkxro.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gntudukmd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gbhekakbt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gsgrqrznd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gclamqwdn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gxkcwehqn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gtrttwbhi.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcmvagpbp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gaewuaxob.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gckwdxxid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gieoqkige.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gimqfeydg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnshntcqf.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gkgtmavdu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gukeepftn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/grrmraldx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ganoomwtq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gzyixvbfv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkfymmfmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gmvvkxamc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gorfllbbt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gudxeyaza.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/grujijxir.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gkrxjskvp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gjndtjasx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gfuzhsblt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gnlqhzuwb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gwrliofpf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gapzesefu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/ggnmefbpu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/giwwyqpvv.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gidahmolw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gxqesiixt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/glymatgoy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gjtshfhfi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gbpfjiwcn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gzndxtgco.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwgnadhyp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gohiaruwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gfnkpoxem.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gvagroquf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gztvwbqgq.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gihlpqjbb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/glvgwkxpe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gspshhwms.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/geskvrdfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gytwhdttw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbquenryb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gfkoxzpxs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gjekdpiia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guixblkpb.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/ghfxgejxa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gevcldksd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gwmytczmg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gautxwvru.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gtcohcoyp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gigfjretw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gytrsolrk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gzroyxmwm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gjrxmcbxa.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gqzxhmxvq.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gglftgupw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/ggeswloid.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxeaubvzd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gfnjusqar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gwipnibey.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gxvpjzrwl.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/ggtsqxvhh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gopcsnngu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/ghddawjgm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gewmerhar.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gvfkuytmn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gmicfzsnd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gcydhmrps.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gkxmsvecb.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/giyqpazft.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gzdizliya.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gawwfuhjo.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gzlpwwtgf.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gvlwnfbhk.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/geviwzjzd.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqgdtznec.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfbyzwgrj.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmncesagv.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwczbvvvo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gfwasbkrc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbezbxkoc.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gjaxxyfhy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gamqkpqgr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gznrhsyks.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gznulnggt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gplcpdzkm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gtkevfhzs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/goapotvai.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gevzmcgpi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gdnlchzmz.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gernafhyb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gohtuzchi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gzlypcchj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gqylzkbcx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/golobhimk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gludthnrn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gahqxfmcl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gflabyuek.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gnanxayqx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkcgqjptt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gpnyuvlus.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gnxrmvlbl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grhgmbqhf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gpictasfe.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/guevygfvl.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gyfmygmkg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/genzljvtm.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/guhhwsteb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gdqwxilex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gjctiudin.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gcsmzzupr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggjafcqqv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gpafvfecb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/grvwlvnli.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gebpgpnao.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gfhrolrbi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gecprbvxh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqizoypjf.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/grknhssip.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwfuqpose.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/ggfyqkndf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gdmmolkuz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gqbhqsjrb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/guwdtirlz.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gasmykkpj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gxiimgkeb.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gbkbprfhz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gfbfppztz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gbodwijsb.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/glxgxmdzk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gduvrxsqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gmlqvjsow.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gijcvxwll.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gybuurtze.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gmiykyjgl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gpcgtzvvy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gbjldclrr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/grgvpdcwo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gfnwuiqmh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gccgcufpt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gdcdsqylr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gofljyprb.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gakbetapc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gwxusldmp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gnrlyuaju.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/glugwmvrm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gexlptoxv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/geuoxkulm.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/grlvxajuf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gkoohkdwt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ggqwgnttx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjtunqjfz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/guswgkecd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gbsfddptl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gnsjdnxsb.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpzyurlwr.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gmwpvgcsx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gehlhgixp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gatlsgpgj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gkvqchxnp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdapucipx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gqxuprvnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grrqwvjnb.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/ggpshhpjo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gzmpkjtam.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gchfuguci.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gvpyitzuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gbxjzwvwy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gcwpblpnf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gvxpwydtj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gsqrgpule.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ggucisoeg.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gkvjmgnaw.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gtifhxzsx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcvtcixlp.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gkifwplam.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gssiffttt.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gmkoxbchm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/grpaxakuf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gnadaogcr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glivwfzsi.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/glqeoqwbi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gcbjygozg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gszmftcrs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gounoweak.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gkleaxuhk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/giqgckyuc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gpimcfvlk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gugdsjvdw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gmdfutkwk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gznvoqsdi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/glxgdjcgb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gypjretnb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gfrzztmig.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gdathviot.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghkcmwcoy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnypxlpre.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gigjbiqkr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ghfrftpqv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gixmknspz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gvuccboci.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gvedhaezb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gtgkdpepv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gkuxzrrzt.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gdhtlgoba.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gdwacteca.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gllmnddjc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gwhzohvvm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gvyhhnilf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gmuqwpaiy.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gmsorrqef.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/ghtayfkic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gaictbhtm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ghavbouce.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gqhngnoim.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gjznckrnu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gejsgetiu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gtkcuetii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gqzdmbwvq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkrcfnuat.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/ggczdgxgi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gfcdjjqve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/ggsujwttu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbgplun.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gbmvtqkgv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gdkpqztmb.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gmtzbnnrn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gzuzczuin.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/grifbfcnu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtxsplxsx.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gyypszvee.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gvvomunvm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gryteyifi.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gajuxrnvw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gafzlclhe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gynyiiidk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gdbloniry.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gyyqxtzzg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/grywwzwru.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/glbuwtoad.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gccxnsikb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gfelqunxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/grviulqji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gwedeakzh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gegyfdhsw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/glrjckeve.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gsrtofpdl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/giyucqdyv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gaqykhiic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnsgcbrik.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gxppsgzde.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsfgddimq.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/glvxsfock.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gkhnlfvzh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwqxducis.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcjapzwca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gznwvuitz.sHtML


<!-- 参考信息 -->