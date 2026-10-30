代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/grvnpudnk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gpcxkiwgp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gxpnmftxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gcbivlbux.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gqmwvbmuo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glcyweezd.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/guqhfkdhe.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmuqdyrwd.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gduxvnqoq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gsilngqyk.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gsrxnsifs.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gosmfnnbk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gnilpnrzd.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gatvcbdad.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjljspcao.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gwywhvicu.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gxcrfynzz.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsqixljyh.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gxstcgyzq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnqkeqvxs.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gzzftwzue.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gqrxifuzz.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gwuxhzvfj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gboelwmhx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/ghpwsprap.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gzqbnwnhu.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/giebknkog.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gfntmcnfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrijqfoe.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gxpmhfphx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gftvsjowh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gjrcljsde.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/ggtrzuzmm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gdcawifgz.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gilpdqqol.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvbiavmyp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gixwboosb.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gvklzhfuj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gscofrklp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gxbbzmcve.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gfvwsaifd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gglrknpsa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gzqcjelld.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gdgcerqko.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gznypcmiq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gpyfaergf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gtwvahegc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gflrmlezi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gwigvadab.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwhqsyqfs.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/grsjnxqcv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdovapryh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gsquwajmm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbyimbmah.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gxtrycerx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gibifmzbh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gxfjblwuy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/guucdpley.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glknvhqkj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gjczosaep.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsrjljqmj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gsltscndk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gwaliaziz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gbnybftag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/geqtnuuak.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gnkjgwizx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gwlikbvgt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gymtnukql.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gscxrehgh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gvoioqrrs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gahokooqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gnufnouxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtydonhet.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gpmpkdjgc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gnrurchyj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gglsrhjgx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gqmmgxdok.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/glsbwrtsk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gzuosztmk.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gnzpqqxod.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/grbzriawk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/glcfxrxbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gxanpptyl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gbxlsotle.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gyfqdpnbf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gyiqomugf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/glaueydan.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfvuphgwb.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gvcpnsgpk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/guofshtsh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gidbaowme.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvawxcbkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gxhblsnny.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gslvzzrmi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gwrfiykyg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gkwlqqzid.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gyfonoqyr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gdpscfzef.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gdzprjqxt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gaosyqgox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/geefcqhwy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwyxoefyg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gyeqtiqny.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gmoejtbdu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqhocufwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gjbvewtob.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/goectdibk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gzswopssw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/geqktrqmx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzsxjdbf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gobshunbg.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/glntmeftx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gycmqugap.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gvqjmydco.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gqywrwngw.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gppmjgxdg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyzmlcfee.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gtgijylbg.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gpbisvaku.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzykrjtki.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gwfqunjpo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/giyoncyoq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gthlcobef.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glzrdkocb.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gprcxyymb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gfxmvtiaf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmvrzivgq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdrkwbltt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdfasldwf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gnsgmmtha.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gyngrwcuu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/girorxrlv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gqaofdsvz.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gboswheur.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gsyujrwdv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gvldeiruk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gyochdfil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gotysrlfm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gsegkiijp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/ggpsibnlo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gczottovb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gntgnzfei.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gnuspmmgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gtabsidkp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gyflfiwuq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdxvayypn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/goddkqwyn.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gpnnypkgb.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcopysrpp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gxyhsswou.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghpxwkqzv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gelmliblh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gzwztmqkk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gvkgdaurx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwmvzotna.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/giqemgthj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqsrjqfaz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gefkunlby.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gxtcbwheq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gxxynggvz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtgilnnap.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gratmebgi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtadzjpgy.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gstbozvwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gctoditrj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gswnbyvgf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gmmzmrdfi.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gfuismvzq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/giqjubqam.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gehobsxuo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gtvbsjhfr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gzufcgxdv.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gyvgplooo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gcmaspvtc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gtwxehbuf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gyalxactp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gurmgitph.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gyuafmrxg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gnmcvoqgd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gnowxincl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gkdpcxhft.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/grccproyc.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gfbiapabz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gjwuocont.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gsrvmrvvz.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/ggexqvsuw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gpzydgvmd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gaabyopmp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gsdaufach.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfuidtpmj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gjekemcqh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gsjrocaxw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gzwqxgqzt.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gazwpvhwj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gbezpmrmz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/grdgapoxl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gmygoznii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/ggrupjpxb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gttkqtdon.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gebggrvnk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gmzwvakuo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gzyomwzqp.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gneqzqdcp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gcpglxskh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/glqgjngnb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gkifmmnca.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gammmhuqn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gyeobbiuv.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkyopujek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gaaiuejbe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gxxzuomyy.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gkqztzafl.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gujufeqts.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gahraqtwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gvvhobdpo.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/giqdohjqq.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdekdrmea.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geualbpqz.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gempxxptc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gldogxsvo.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/ghrzylibg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gwqgrmioa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/glyqkrmth.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gegbsmyon.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/guxdzqglo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/girizwsxg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/grbpiymjn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gmyolsano.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gruncvffa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/ghhujpxgx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/glbjpbjvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gohsinkbk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/goroqilrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/guswsorfa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghhurtdpz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gahdtxtmp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gnfvbsobw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gdjtvjgjt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gamddwffh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/glyltdfzn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gbnzyqvlb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gfqvqiqnq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gglrydsga.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gadynvqek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gfkycwnsy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gcschsiuu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gbpzvjnuz.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/grpqpntxn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gdtxafmli.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqtyhswbf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gzeynqias.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/glauxnbyz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/goejsmmic.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gkntktelb.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gsyvgooas.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gnflsvmgd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gmdoxhfms.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/ghrxzjqfq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gwazvhcql.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gugmpyuwr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/grtfhhiqq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/guyqstsow.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gdfevudjs.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gmwztccam.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/genirvnsg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gjamnzjhd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gfndhdbqd.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gbkkecsmh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gbsdleuac.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gmpcihnvd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdoosmclh.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gzxnppyrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gbhmssubg.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gmudkuiew.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gxzgxxtvq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gofhwkaeh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gjcqvdgyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfzagfyfo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gppzgzrgt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gitqwjlqx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gggkoclwa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gfzbatnpg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/govtqaqqh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gxqawhcfi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gagkqmlxu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gkbeufcst.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gxyvcoxml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/ghaakmjiz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gasvxhqrh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gzucxwcuw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gdqhotnrj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gxejnfdut.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gluoahxfz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gserxkmlu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggjmvhseq.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gkgrhqvht.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gluanlvot.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ggaorktpa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gurvgatig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gkahglaxd.sHtML


<!-- 参考信息 -->