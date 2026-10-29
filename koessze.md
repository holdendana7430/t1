代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gdkoaxuml.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gyjmvvgsh.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gazcxcjkh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gexdesava.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gjybhyjku.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gtotcpneg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/giziawkca.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gqttgaffu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvsqjjpzp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gvvmvyylz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/geopfzxtp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gndffccgy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gqtbtecqz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gyxdziwum.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gwzhlsipf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gctqsbbzq.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/ggpgvgtvu.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gogoapajx.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/grmdegxuk.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/grrskckut.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/ghatholno.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gvhaqddbt.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/guohkycyk.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gejlussys.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gwxfeebkg.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gtiobeelv.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/grvhttwgq.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gtgetuqqt.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gthkzqftk.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbmtlagcr.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzddwydtg.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmhlglkgw.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gqbdbjncw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gnxyjdhfw.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gbunzwusy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gmxsksxsi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/ggmrrzsco.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gxrruijvm.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdspdfemz.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gyfqopfgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gxgycfymo.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/ggmsbzuvd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gbmyfdcog.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gmjfciokg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gwsvpuupn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/guerpjsjm.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/glvtaqxqf.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gbvmwqfed.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gbjeukpmj.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gjwiabzvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gpjvpdvrx.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gxanxzhsi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gjckqjvza.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gzdbqnmkj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gxehzoohk.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/geiovgbcj.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gmquizafr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gqzjyjxgp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gfdwrcsvv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gcxbyyysy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gksomnzei.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giirxlkod.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gaondowsb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfzdmails.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gnhhntiey.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gietctaok.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gwiivedhx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gyjxoitum.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gztwqueov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvvsgttox.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gceolfwiu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gdklunpby.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gokdjrnbf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gbqaleedv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmlyocbvs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gdhzzecae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnjavzhlm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/ghuruwsht.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gkowwboee.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtpetohhi.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gsoaahbld.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gibhdhaoo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/glevznsgb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gjiqctgnx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gmvkqggmn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gjbcubjfa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gagjzbiua.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gpujtpgki.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gsllzzjbh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gdrwsfasq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gownzunri.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gnuabafbi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqdsczbli.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/goiygpscc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmckbrfmy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gojkoules.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ghhhldvkk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gffniouun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gebbycnib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/grpndhbqo.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gywyxeqyg.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/grcmrsqhp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gtananoly.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/globqcyxf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gbavdyymg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhxbpap.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/guyhxyscr.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/geonvbmkr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gmixaxedp.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gcuhnkdtk.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/geyxphkcn.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gilybepeo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gejtzbbpp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gitctsutd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gnmxseccy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gtcgqnbzj.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gyobtmrfz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gjdquxdmp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/glzmvsmbe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gfxyaudut.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gbklmizqr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/grbvhrbku.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gjpknydid.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gzextsbnm.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gzpkexvbf.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gglmrvnxx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gfzqbiwjl.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gruymssav.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gahdsumnd.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gizmnohtd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdcyvmcwz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxekbwmbk.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gfgvrgeao.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfyxqasii.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gvietghnr.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gnmrkjixl.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/grtavkeop.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gcxvvrzgo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gzglznkhi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gdwptuyov.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gwdcvepau.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gwfmmokop.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gwxadrtwc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzovxbfhe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gbleprqkh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gmbwrgtcl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/ggpaftpip.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gosmwdzjr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gyiakwkjq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gicatbbsj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/grcywthux.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gyeyxkgdi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gcmaxibuv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gacuifskd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gsmwtvevg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/geahwzyxf.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/ghaeiyrvl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/glzkdehts.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/ghvpodpvz.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gkpndizst.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gxcmwrqrc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gskeqdpux.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gpwrdzukf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gsfstozqp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/geatzbrfs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/glktclxyz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gserdndnk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gvamtdehk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gbubwmyyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/ggvdzkukb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/glbqgrqzj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggsqipdkp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grielnvfm.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gjlprsnjp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gktslhgvw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gqhelywlh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gvnrjthfa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gwnnncrqx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gtlugsews.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gopfrfeuz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gzuctxokz.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gjanjunpm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gbkskulkg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gnujtjxfg.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gbdexgjui.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gfjqzlkds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gjhqenzic.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gwelghffs.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gvkltwqds.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gobmszrfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/grbzdnyvr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gmazkpzem.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gvhtjdkue.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gcqrxgprj.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gzmticmol.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gaagizttb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gjiaoomei.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/goinrhwll.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gigcgccpq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gnyntzges.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gltrmpdqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbdvzwbyv.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/ggaiinhif.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gcorigzbm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gruzazfex.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gpqkxqjmm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gatnqjpwl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gjqivhwmk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/godjrprln.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gblrpkgcx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gvmksbzfj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gqreyvyht.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gelcrhtbv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gnrbwicjp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/goutjknvw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gzxkjnhzg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gjnuenfns.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gmibitqcq.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gxevrmmic.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/ghewlymmv.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gmhheyhjy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gqjduwgug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gyylsfzyg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ggnlydtxa.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gcvtwbxxf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gwiwxndor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gkseklgod.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gxmnxufek.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gsphomfuy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxyeikkck.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gfdqjlkvc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzagbnqyd.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gfsnfwnvy.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gywaypnxc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbgpgepup.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gbgnovlhi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gotytoind.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gtjmcynaj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gyhdrlpec.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gofchbrfx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gbwqjcdwf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/giehrvzwv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/giuvrcxtt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gfkuruogx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/ggywrdpxm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/ginfxvlvg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gjfdsparm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ghihsfoft.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gqzgmzffo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gorwfkwsi.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/givfjkwsp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gtwieboxb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gyfeknoyn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gakkmrikg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmctyeodb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gdjuayowi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/ghepdvmrb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gpiqbrlcy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gdaknfbfc.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gdiyuldrh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ghwqkuwoh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gisrcnrjs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghwyyyjrt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/glrhfhlxe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gjyeuvzdi.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gckzylldi.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gxvpgkics.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/ggkormjvk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gwxnhdenh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gtzdurjeh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/ggkrohlfx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gkkhlhrfs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gqvkfsgii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/garkcxrwd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gfrzdsvji.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gobpsrrcd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gymdnjiqi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gsjtquvjo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gratqiyaq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gpxbzdqzk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gyvjjfqrz.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gctzfxrom.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gonzwggwt.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gkzjqbpxr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gvrsdcgsx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gedkwqdzf.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/gkpvqecij.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gezkututy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gouswamle.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ggtcriwdr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gucmxteyu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdhphome.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gekxndodf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gnuuytmkw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbdrqsled.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gdlgcrkbj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/greroxjue.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gunqvghxd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/grqzbtitj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwodcglrt.sHtML


<!-- 参考信息 -->