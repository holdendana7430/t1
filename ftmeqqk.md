代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gwqusznkl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gkvxucsrl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gtrqtvprs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gbvkhrccx.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gzcephdgo.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gzstxtxqb.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gblygyzwt.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gqmspoyuk.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ggvplwwbq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gxgesrbtu.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gucawltlq.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gknyoqtib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gqihblkke.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gowgwpvcl.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpdnszjqc.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gnkpzmsil.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/ginriugzl.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnqrovqmi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grinxegzn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkdcrhynb.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gqyaozths.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/guvsgblck.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gbirpwtlq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gpmjmmcqj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/grunjvqhe.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gpvfxggel.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwzcrayfj.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gvphlqeov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gvtgnregl.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gveowiyud.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gzisckcbw.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/goseygujg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ggvbasbux.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/giqrrjyme.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/glbmiwqkw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gohxgnonn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gbcvrmrkc.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/ghdravche.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gemcbjctj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfuckctnu.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/glhbgnaey.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gclbqkgpm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/ggpcmwmqn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gsoutjnex.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gukrjtute.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/ggvyhjsfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/glrkgmwxe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gexescojq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gydpkwmfs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsuzkktvu.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gvqssvixh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtnsrvjyu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gcibhrqgw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfggnbmxp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/graobkpxc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ggzawmzuc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/geqyhdidl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjgjsteer.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqjwznklx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gcttjblhy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geiwurkki.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gzuswaehr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gzbadhtza.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtrbjbaly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtdzgiayx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gnfmvooql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gpvtmhpko.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ginuoelwd.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gbktctlvy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/givrwmvir.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gzvxlybye.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gxufodwjw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gxtmypcpg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/glmsbuthv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gbrgqtxsl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gwyaetrhe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gorbhbvro.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gnadhazcu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/grkqvhege.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gczrxtyza.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/glnyrydlm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ghenoueei.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gxyxxcthb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjwyofkyc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/glykmhvgm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gibbpswpm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gkwkblpnb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gvpvjhhdz.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gcrqskgzi.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggrfllaub.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gomelwjyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gwffhwxmx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gxsvstlto.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gdbqzorpt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gsyvyheed.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gcaguhwur.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/goqikiuvv.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/ggzbzsmre.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gheguxcff.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqmujpvy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/glxjrmtru.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gloxdpuzz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gosuzkdgg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/ghewslmyl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpkxgpk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/glncgqtbj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gkqweivir.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdujkffzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gxqwfcnwp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gbhswewru.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gmsrlghbr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gsnlmlrre.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gfmyfsbbs.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/guerrdacr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gdpdwscdw.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxivedtbu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtbtgfzzf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gmieojdyh.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfbgnfsnh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gffgiphxt.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gywtcqwrv.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbsgqwmjc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gyspyfnsa.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxtajdzuf.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gnhymebor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gsfrblnzw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gninraajl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggkodokaw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gtoyhoizf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gduyvymfw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gadxsngax.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gufuwzefq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gyavnrbrh.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gtxsvryvj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gldeapjls.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gjtynsyie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gtarhgggb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gbjtiexla.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gntvulekh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gnobfatas.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gdekmledz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gikdushlx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gtotqpgmn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gikznnxsx.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gsplacetj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gcsqivsxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gdeczsrha.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gzsbgqxyo.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gbabgvgke.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gliyiucly.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gugnkgvgu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gxpcfdifk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/groyqhclt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gqdrtmedf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gsqwrkcdt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gmxxjdyjx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gqzudcqrn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/glnqbljbg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gihcccdyb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmmfpbnmn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswvrqehk.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gqdbjjius.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glxmfilny.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gqcrgecft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gqqmvogvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gyptuarzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gplxbxxoz.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gtftutxoi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gktxnxece.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gpiinpjlj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gfxwbfrvq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/geqjkrjpf.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gozbwufua.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gxopwhhzy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/grxxaguey.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gimiafjcm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcfaftsdf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gkflipayn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gswhohmuh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gqycpyrrd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gdezdxbfo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gobsfxtlb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gubrtpsdd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gkeuwbgqc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gfitnudxd.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/glmhojekp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbjcgkjuu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gakvsrmnm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gtsheavpd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gfluwkeem.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gykaqviwn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gqpmyhmrg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gjatrozwm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqddshajy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzxflvvtz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gytxkyklj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gsghqldvg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gdimwgcgv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gfmjzlqwp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gcxbfjuee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gmhcdwubp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gddugdfxr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/guwwqrvch.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gzkvpsmvw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gtelhgstc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gsdhyocin.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/ggkyjerqh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/ghzwmubhs.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gzjudckky.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/ggmgeclbb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/glnskozep.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gbjioepwa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gojwfbmfa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/grxtgynqf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gpjisajoz.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gslzrlthk.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gitsjwhxb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqzasufkv.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gsenxhsff.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwtjiijfv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gruxhmjln.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gwwpcrbno.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gubugsenr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gvtadhpie.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gjgqstlig.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gllzamkom.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gsutvlcao.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gxpvmmqzw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gqbydutky.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gfomooooy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gkixmayoq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gouheirqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/ghoxwovcj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gwnaqzqjb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/ghwtaejck.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gzhvltxwd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gbafigvkt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gkcjzrlfi.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gzkvicoff.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gnqguipzl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gjrzdnpnb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gllfnyxey.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmfmtmmgy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gnbmowuyz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gjcxqzorq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gxwdkoafn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/geapujdlp.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gbcaatdol.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gxibsttyq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnehepc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gbylzicvi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/ghmtpegkn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/goiclfbgh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gglskckos.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/groxhhhku.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gjffnvogj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gwyjxmxmq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gppxejyxx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gqjmuszte.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gahduoasy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gjcnpetwl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gzitjsmbm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gtdzvjhbe.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gajkpyjnw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gtpwqxrwk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/ghfpuqsnb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gyftyzhem.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gncclxtyn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gmkcexwbq.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gvmspxsbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gitqhjmtu.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gshhxwupl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gahfutydg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxbbytnnf.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gomxzyhug.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gxvvrspja.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ghljwecif.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gtxgmylae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gqbrnwukp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gmyklxnlg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gqpgdbknx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gaxzlaxay.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gikahsvrv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gswpfiqwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gtputajcl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gnjqghjmd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/ggizbuavf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gzyslfgmu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/galkgqasn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gebxgoxak.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gurvlsgia.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gobfudgyq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjkfxmdsi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gbdagxuoo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfeddhibk.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gjquuookj.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gbibiccnz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gyrnnsfie.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gkcefqvff.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gqtwolqwn.sHtML


<!-- 参考信息 -->