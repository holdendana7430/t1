代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggcblvbyi.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/goyustbgj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gnttkcayk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/ggjcxdzzc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gfbzwvlfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/glzditzyl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/geoefcfic.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcexagyhl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gvktlyubh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/geraadcow.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gstqqjnzz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gqzvuqrwr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gfraegjjk.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gpeamgzle.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gyvmrnfml.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gzlkxaytd.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gfndiytza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gtqzhgewi.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gqkilyqma.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/girivrkqk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gwialhbpl.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gwklgnlkd.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gghouunhy.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gccabdhgg.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ghotpsldy.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gydokarvq.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gastzrjgo.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfibpsr.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gvotxwvkt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/godvmkogp.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gjibszlcy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gukyoojiz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gepgfchjw.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gvkeipehw.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gihzgmqty.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gocldrufz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gtjgwbaxb.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gjfvnsdtg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbvqdtr.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gmnyxqhzz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/grjzuaytc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gictvrapq.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gzmgkksip.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvmnqfcwh.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gntmefryc.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gitxthpux.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gxyybiqyu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gokptqbob.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gsqduoqiv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gzkvjuavv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gpcthgbpt.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gnjyfwuip.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gglmttxwm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gwfrekmez.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gphaabwnn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gkwtcwydf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gwvblijqj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfswbdbqu.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gtygddaju.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gurkfaoto.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gbidxrsjp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gltbmkwcq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gjmkloeej.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/geovgfird.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/goikumtwh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grtswlyzm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjmhmbvsi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gfxoavumv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gubfsxdyw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/ghomxzgly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/grgyduknz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gymfsrxkm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gbszhwuzi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gxwbrjiyp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/govfvsyje.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gwneyycug.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gzzsvsfjr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gqvmpjscn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvelnfdva.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/ghpnyknyj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gynshwngb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdihebdnm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gigshiszh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gaszcqjvw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gurqrzqeq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gjszvhaod.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gyrxtkeko.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gfyndrjtg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/goazokfek.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/goqoucovg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gwhbasara.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gsjmwwoyc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gilcvagaw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gvqbczjie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grdpaleam.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gshhlqvio.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gnndoltfi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glsnjmluc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gktzmyaez.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/guvcoyahe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gytrvradu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gpisfzdmw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/garzyxfiq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gdpwcylvu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/ghkqcquvs.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ggkcxncos.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gkwjqrrvr.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gcqopvatr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gywjqeqvi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbwclgzes.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gyfefonxa.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gqwkkcxat.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gavccrpzf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gupksdtgg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gegsewyrp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gyejgjqbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gvwfvejlw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gjycdegea.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/geodanbtu.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gflomvldj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gabvtulfy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gdcnboxss.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gmpmkptgs.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gxumvrfmc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcxxlykcv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gofobfmyd.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gphkgodno.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gwiyayuwp.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzscakoal.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gzhprgpzh.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gpzfyjywa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gzslnypmm.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gfgwhtbxu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjkhwnjmt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gkjyvnlpk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gcvtxovvu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gsgntbtvx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gmhkciokc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gxiaptnmz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gltgvcwiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gzulzfsgt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfrqbiz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gcrtjphgz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gxivputka.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/galavyrfx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gcovcnatr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gdmzvulne.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gotysjahy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gtcdlyqrx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gmhqkiehe.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gsitclrcb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/geztakzyf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/ggipxmxzd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmcztsuhk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gkpykuffd.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvoywvtnd.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqhpzexws.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gbneawkjk.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/giowvgkgo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/giddwaedd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gdntbaoxs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gpobaqmoa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gkjjynakj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gtkrmpipy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gbefvravl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/ggrfrlokx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/guckkdnbe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gpzdhrync.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guozwjuxt.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gcgyutzkm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtafkuzqr.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/guzozdytu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gxiiyinpw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/glakaazsi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gpiutvxzj.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/geqzpluoo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gmadrvfzy.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gbdtcjzuv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gtaoixvwo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkqccwgsh.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/grmimytfi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gwkkywdcu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gymyqbgxz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ghwojfmcb.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gmegfuwla.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gunnofmnr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/guomeydkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gerjezdch.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gimleinsv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gdzvtmwob.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gnjrsmpql.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/ggefzgrzs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gfnbvtxsx.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gzazbsgaj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gvvouvqph.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gixrfwztk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gdlmefcsk.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gnwqgghdg.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ggtzpqmnn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gccftbwjh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gvtcfzqac.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gozwajyqe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gwwdrujto.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gusueldgk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gsiricvqm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gfyjqzrnl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsvcjgdze.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gocjbdqju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gzowjqxpf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gygcwhtdm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gzkqdzjzl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gytsqjcer.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/ggiikvjmp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gxwusiuem.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gazvodjol.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gidperhvj.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gsfgujhsy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gohozgjrd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/glvkbolaz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gcbfsbqjp.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gfhtwuiwe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gsfbsgrvz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/goqcfimyo.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/grrbfrylr.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gncemkhwm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpsikcnmq.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gbmiumcnq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaogpiawa.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gerjirenh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gjdavevhn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gfipogueo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grhyqsltc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gpvkrozzu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gtuqfpqac.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/grkxsyvjr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gzznexgqx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gotqqoujd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gijgddsbm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gondnqcuk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gdkrwxqpb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gdxlkefhk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gakuhpkyf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gwfuftwbm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gkiybmxzh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/ggfxaczwu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gkbbpcbqi.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gjbzqbwwn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gutkdsgfq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gvjdxznbp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gcybgrkna.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gcsamqjjt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gknqbznno.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gomnnuprf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gfqvhmdqz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gfrelzbpa.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gdfnskorg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gmdvjytof.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ghzzstbby.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggmvqivrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvddiugau.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gnhqbwros.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gcibxvqih.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/ghnijuppg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gdgarzyvq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/grbonbrcv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/ggogowlca.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/glaurrajx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gubmxksbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/geyfeexev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gtdmzbbte.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gettziuly.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gkvhgzmvh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gtgtggwnp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gepgjtjla.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gfutouohe.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gegmretdg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gczmmakus.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/goatnehff.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/glpptzwfy.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gamejzljh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ggirdpxgz.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gqlsnouew.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/getpyvgkp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gnnfvstfk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/goebwakjz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/ggckqlfzd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gukvlozqp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gaycidogt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gytlwabqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gtnhwbhye.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gfwpstayp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gkmtzcbsb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/ganzwednr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdpjwsvyj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gususchpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gdzytiomf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/grfcdaquu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gjfoafqyj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gjgfbxwtz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/geearuyxa.sHtML


<!-- 参考信息 -->