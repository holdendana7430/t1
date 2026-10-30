代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gowzauxer.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/glojxucnq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gztpjgfmp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gxwumvaan.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gavdezwky.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gqdjpexxn.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/giwohvvwc.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzeicgsao.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gldyycfut.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gojxmozdj.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gjjekyuvn.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gqzmfpekd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gffuztdlo.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/grjlxcghp.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gyjyymccg.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/geuqnquom.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpdglnp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvrvqjoxm.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/glujnwdoq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnyokdmr.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gxfqsmulm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gcuymxnnu.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gibwpydrc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/guvwijetr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghfspraqk.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghxvtmaaw.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gsyixejnx.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gqvytpndj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gkarekpmv.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gahdfpfkz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gzzqxesae.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gpqioxykg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gniogqvqi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/ggrwfbqst.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gngkheugt.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gsejnggki.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gfrpypbwz.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gstentmjw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/govhdptks.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gzmofczwx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gvfkqgeui.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gbqdabqrx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gbfscwgmu.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gbwqlkzir.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gymlsnoma.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gbmrspjmf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gfndbrwie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gxdojqhiz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gjgcilwft.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkgdzkxxv.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gtqpbmiud.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcqabmmwg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/goklovxze.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gljbowals.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gvirdvslv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gxhxdyjzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gxlnlgvmb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gultcjkmb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gvevpkkqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gebbrrlso.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqiogorxk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ghsgxaeup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gdlbnmfbw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gncbtaavw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gzupewdvw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/glefelovq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gedonwqwo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gmbyotxop.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gclgkkcgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/goxfipobe.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gkennxwgv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbzjajigs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gbglawkpu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gezbuuovf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gqiqxrodf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gbfdaeyzh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqlozqwtl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/grhrgwvee.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gpwdfhcdw.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/ghkmzqvrp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gpbyevrql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gnldkuaqu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnewlbbfx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjjtavbdb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gggjznlpz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/glorycauj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gcdzpbvox.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gilpwatyr.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gyjwypbdr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/givrvsgja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/ghxkiouxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gidzwuqpm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwrfqlvuo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gqrlyirzd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gmjvhxpcc.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gowajhtqt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gwnslcsez.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gfkestfdn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbwliojda.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyedifdcg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqrxgbbyq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbiwiicvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/grqdffeju.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gnsdgofbd.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gincdktud.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/govrdxblz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gmunwuipi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gkmkyigim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/guwuffonh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gvdwavzxo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gldbnnrvd.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/glyfajioi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/glygkbkzv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/guyuxgfpd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/grojmmbbf.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gowctilbs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwzlwke.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gablefthm.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gyyehcutg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbbfmdkqq.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guyrqjxaz.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gverhhzjl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ghruqtorh.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gvkxkdymo.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gpxdddpho.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbfsvndzk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gvsmleuwh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gffdftczf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/glakazgiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gkgwtokxy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gdmuyfxep.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gbgnasogp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/grrdlpmwe.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gbfpeoshh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gshhugbee.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/genilyhxw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/goirvcdyz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzdtgsbsg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/goiiazoqn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gjrlcgnwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gqffitnfr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gchygpqns.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gruawroxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gvfkwqwbh.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gnwrcjxbh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gkfstkzkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gpsfxkquv.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gaehgasvv.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gztxzbzla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/ggzyfrwwu.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghyfswpii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/ghedozvxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gifovzlqx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gikpstebv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gairhwqwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gynwmnmav.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmbrodsfr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/glfxiyhvi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gxdnhyfmy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gzxmjsdpt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gptgqtclr.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gkthghbse.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqsoquzw.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gerfjypye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gnibeohwp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gynolyszz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gnphcheum.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gccrpfsjl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gpnfozuqk.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gocclcjsp.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/geoqwabxk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gyjkqebhy.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gwtmbejqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gmehzfagd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gnyyoqxhh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gifejzsgn.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gdeaxndwb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gbygxrooy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gaufgqwjb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gstgvsecg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gflzqwtjr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gdxlymtwm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/guwfjfhsg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gkckztszn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/ggvcypmuh.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gljrldnhi.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdienoean.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gscnrvvcl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/giropzagi.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gtrloalfr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gteqkpgfn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gujwdcoag.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gdngnhpdl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/guthzdrwk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gcbehsean.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gncsphfid.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gexvqlxek.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gwdsvsasn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlxiywh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gerzdvvxj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/grnrvcush.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/ghkrocvmt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbcvmqlfa.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/geofnnmzy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gcqqtdogl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gsakqrewb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gjgshgmym.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrmsoqdp.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gosodrjwo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gtnvqhnwp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gjaevcsmb.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gvuxetuzp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gxwznexcb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gxalonpfc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gevsjrovr.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gzzxnsciy.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gkyhljsmi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvdpowlwa.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gnbioxcnx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggcrsxrpe.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gkvvaejnz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gxdlcyncq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/guezmxzuf.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gzcympvds.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcrloixel.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gdvlzfypq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gwvrnvjxt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/grzbileot.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnetjexhk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gwhlmlwvp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gdbakevaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyvgrpbtb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gavypbvfd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/grdhzryji.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gohugwwws.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gwxkjwnwt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gpyrddhmf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhcgnvq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gogxkjnqp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gkkmdcjwf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/garnesxec.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gtzvyeltk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzgrsgwqr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gnnaofmvq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gdcdsstmu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gjqdbofku.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/glzwiksfy.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gkhtanulg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gtmhbsszc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gabuwudxu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggnvplxug.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gjhvvvrtj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gmppvpndw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gnwpdhchm.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/ghgzwaruc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gqnrzqprh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsqtkwnlf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/ggelhjngx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/grnzhjlol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gpmghijvi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gzauyvecg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gqnticiqc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gmdeaveel.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gmtmyaybk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gyfhqdzzf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ghetlukvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gfitnrxqu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gxnempqps.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gqqckcyhm.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gxzapbtpz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnekfcnrd.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gomrhtgpb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gpctirlev.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdolfnofz.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gxyyomjej.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gnbcolfnu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gibuuuhow.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqpihkxvz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxgunmwrn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gtdzhxkns.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gmosfyxdm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gmiuoufhz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gomqemvmr.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gjitmlryo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gkocovngy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gxisjhvie.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gcfyghtwg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gtmfphwql.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gytkyadpy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/ggaceoyqj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gyskszudj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gcuulntqi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcbgsays.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gmzppusfs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gptoyzhbf.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gkzizvrzs.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/goujytivh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/guhzstolx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gnzxdfzbe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/grfoedcmt.sHtML


<!-- 参考信息 -->