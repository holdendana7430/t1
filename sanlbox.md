代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gnlpztzxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gkwuhwebn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gjxrkfsjq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gmylxigph.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gtfyjycab.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gwqznfvfx.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gltlzoiab.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gpwtftvsp.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghitkizcz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/ghlbdwwoj.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gblbhrofw.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gqtydceah.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gxbmlqznl.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/guulockpt.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gocetnrcl.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/glplcjuzv.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/guuvaqqci.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmbtjolgm.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gakzaxqce.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gtjazyzph.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/guzgdctrf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gsdwszujw.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gooetgjqt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/goesovkel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gqyxmqjrv.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gubodgkcv.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gyjpaghpu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gedwoakty.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gtckctdjo.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gnnzhpwxd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/guycfhsmy.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/garapdsry.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gbstrfarh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/giwkoqabr.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gibqxrcyp.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gpulxdjin.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gryyleosi.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gnwpcudui.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/ghjtdhzjp.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gjserqbcm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gtblhbanp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjloeclhk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gquehuxwk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gibtkyqap.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gxwrzxxhi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gywkxiaqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gqlcfumde.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gygibpyge.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gtgvurkhh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ginybkqtf.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/glqotfqrx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grvalhtch.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/grwrirekp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gleaeicvm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gntsdcpgs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/ghsgfrczz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gftqmxawp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsfirvziw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqasvmtmk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gbcyfpqug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtafaikdg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gccehcbog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gbkntzvlo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gdsyexkxt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gcmuprcwq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gfeubqbgj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/grsmnlyun.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzvkbcurd.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gwdkrmutv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gkdodxptb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gszybeaib.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gdjquwjdn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdjrlsf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/guvrxelgb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gxkgxiike.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gxznyihrg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gklopxwnx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gsbhusotl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gaxtzlqju.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gvtnssjhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnauqbks.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gsbvtasot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwetmhltu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjtuluupf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/ggljiavlj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gvrwizvyt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gnfapunqv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gppkvektr.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/grfdswtgu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gjkznzgad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkbrgnbuk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/ghaodyogm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gbbeuikxs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gkpzsykea.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gtinxuhnp.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gylmdjsmh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gqkmbmclt.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gbxnbukqz.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/ghswikenn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gmpiwuwne.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcsyhcgne.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gkytwtxna.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gertqbmlq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/ggqpgxkhw.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gfcpdbufw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcwzfmobb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gvtdusndg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gbypzssdf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ghffhgnfi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gutfhqopi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gcbdxqfyh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gwnyfxpwb.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gatvmvzmo.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gqhpvmrvo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gzsnfqyfc.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gnnzegisl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/guljfscwv.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gpuydlirq.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gkwqqrccg.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjlpryqxn.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gcgeyicdz.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfxazjpcx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gnabxgawc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcvzwqqwf.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gwlgaffjs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gwpegqyid.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gesffwofq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gdjzqyher.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gezetqiav.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/giflusvsg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/goelnjovo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzfhwsocw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gethyfgns.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/grnjmxkat.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdmwlpxyq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gasvwbevv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/ghgcqftnl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gcndutpeb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gxrwopsnp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/ghenawtbt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gdelwzguq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gsglupgjf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gfkilhrny.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gpbjjgulk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/ggcjafqfv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/galyjdqkb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gobaptiix.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/grqbemufh.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gqzqgymbk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gqcqxecdd.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gpqrcxpzz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/grzbwxius.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gahsbbpwl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gvrszovju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gepzsiuci.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/goutpbjrg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gklaeqzlb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gcbeizxfw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gqktcospn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gcxobksou.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqlyhxmmp.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gnvngoozz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqkqttxwg.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gndqnmdma.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gngnzdqni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gtbdfllno.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gabhjpdfo.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gdvgeimct.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gwhjsncxc.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gobmkrzap.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gitkneocn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/glkaetyzc.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gmdurhiem.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gnsrcwvzf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/ggphnhmmb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gfnwlxbgm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/goievqyuq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gjqreddvl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gqwcweget.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gnkoaidmq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gppgzlbjq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gzutvjsqu.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gwyaqajfa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gqdelfbwa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/grurnbemx.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gogffsfsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gwcxzeesi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/ggmshafah.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gyumjwqvc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvkyoxipy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gjwqgvgzx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gwlrlzyeu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gjmmixzqr.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqsmoiltp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gpkqkrwcz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/geduqenre.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gbjsenwpy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/germnrisn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/guozacwot.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/ghbexkbcl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gakhhrkpr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gcubaopds.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbtbkirid.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqqvjkvmy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gakvwmdzi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gybqlulir.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gavthzwqj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gjtlhxrdw.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gqdoqftez.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/geuomfxzm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gyamhvmfk.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gzxvgvvoq.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggwgmhzxn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gnzxjoaho.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gqmeonrcf.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/guimbgfgj.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/grwbuyuso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqrmbpsun.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gmmmbthah.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnglvmomk.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gnymxches.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gfuvqvlyj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/giepfpbjz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjzpvzpax.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/giwleloxr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gmnxcljph.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/giejsjmdz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gtmrssmqz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gtcayfmge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gmobbabcx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gypqbxfsk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ghgipcznb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gzgaufxdb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gkpzbbuzp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gpnbyzupm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gpepxdfog.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gybpuehkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gdpwcdpdz.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gearydefq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gxthbsomr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/giivqjlie.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gvbyjemam.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/ggwtfvabr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gukjgttef.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/glhlxqcpx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gqyydwmog.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gdbtvihhv.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/geoaxiljv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gutgrgqiz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxvlejadm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gjrbcglze.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gqqufxisx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gndwkhiyv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gveuezkxm.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gawnkeuro.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gqkpblxdc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gzmkpolpe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gzepdrtsc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gqajvmsyr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/grqusjfyq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvowxmynm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gkfbcllur.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gposvbofk.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gdhglkdzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gualywsvd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gregftaqb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnyvfuk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gsmsusdcg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gunyjnlqq.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gleabtcnv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqwvjodih.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gsaeskxna.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gzyekfctn.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gsrsoampq.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gmhccfzcd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gjepuvzkm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gzqlwoohp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvvttszpb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gjverixoj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gkkbuqguc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/glputgfrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gbhuzyhao.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gcqdwvdyx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gziytacww.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gjvsfoqmn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gcalzpuis.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gauvjpzvy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gawykzmgf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gibkvwyvb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gtgpocjxh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/guqyobvyw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/geaujdmrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzelinjuu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gzufwjtdv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guqsauhts.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/geybbrmim.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gergxtoit.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gpakxgtvl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/ggauvelhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gywvnekjp.sHtML


<!-- 参考信息 -->