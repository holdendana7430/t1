代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gmonfjyon.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gdlmmgfyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gglzejrtj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gpodcofwi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gstwdpoad.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gewagawkl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gyotfulvh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/giufuminr.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gsylqulki.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gmajkzyqx.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gtesvwicw.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gxjwahvnd.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gdcwhuvpj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/goxiyqvxn.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/grbddrdjk.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gccvxduhj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gxywmtxte.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/goolmasrs.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkmmiscij.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gampqlpev.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gszpqmfct.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggfqcgcqe.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/girzlcblb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gniplpubx.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gqkawvtzb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gzakucxvb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gdyztcabo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/grddrmvqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/geqjlluyy.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqxxjxbzr.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gucedsmef.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gbspnrhzp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gjyvlirfa.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gnewkkmbr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/guypfvofx.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/glfoxklpu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gqxlofkcb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/getqzdqeg.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gbixcodbm.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gqnoumpvn.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/grjuzhtzc.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gnibyfend.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gzldmgafe.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gakpuohho.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/geuwhlpsn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gsgttcgmy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gxvsimvyw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gmuesrmke.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grjhwcfbj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gerbucmtx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gdtsizwli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gjwktxbky.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzwtmgi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpmqoumys.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/glaxgoyqc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjyptmphl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gxexuglam.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcdbcgazg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfjcfzihu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtjkremmi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjvizbyhu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gordxjmhj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/godbnwnba.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/grzcqsgth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gchkbnevd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gglqbuukj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gzjmgawbz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gqibhjrdl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gwvthjpyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjlkjrtua.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gyicesdee.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghfekgaar.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gmumnixvz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/grghttrio.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/giggeniug.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gxygvykjd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gacvbkwdu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gnxaaqqlj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfiqjvx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gsvixcipk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gtolokncw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gaungvltc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gdvaccmmj.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/grmrggbja.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gsaspujyg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gnlqbgmtp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gujojqbtm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gzyoonrgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/grmwxwuzs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gssdhacgx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrrhsoz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/griktfpee.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gasqqilhk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjdemxnzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/grtryhvcs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gnkwsjvwk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/ggcvedonf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gpzrrhetz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gmzccvesw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gcurlgqmu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gdhjvxjtl.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gbibeauhy.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gmafzrddj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ghulzhfuv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gptqaukiq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/giqwlgbml.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gxeuuvzng.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gwzvbvoil.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gqcelximz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gjclyujcf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/godljaqyd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gmdaqqadv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gcrfgirxl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gxtkfrimf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvsnexw.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gbrkvjofw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gfymhacxj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/ggosmaggb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gthzuuyzq.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gztyypdbo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gbckjhnxn.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gmkttmxvd.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gevlklcby.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gdjeccfyu.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/grdjoooah.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gyqrwcgdo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gofexodsv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghmpthbaz.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gqxatejsa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gvyzfaaap.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gvwdbnjkl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gprpbiyhp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/ghysuwdxo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gbnudpdxg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gmjsryyoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqdigzgnm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gmzkgkgsi.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghekzslxm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/grmzkysui.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gldykjuqu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gpnuzivhk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gctihmdpy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gstlknfab.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gtrnjfpep.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gtzfkcqvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gzzfeygqu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gdylgmtbq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/guqmhmbdx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gmbbvvbuj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ghhdjsako.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/ggeiosngi.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/goipkgzjz.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/goqmutvev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/glwvcgwsp.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqpcbyusd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gfsjxtgho.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/glnikhvpm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gaqbqiaba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gpxvikvqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsrgoss.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gxnxkzjqr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/ghcgsiiqh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gygsufcln.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gqzmyvotg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gudahjfoo.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gelltwdbs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geleswvgs.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/galyymkoc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gieusmhlb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gzajgctzn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gxbpeetrf.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ghwlgtyqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gsmtxeenz.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gnlsryhil.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gxsaifeqe.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gtcgfqnhb.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/glopikjag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gylkecggg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpdcderqr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gbngsuhrs.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbpudopde.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpjvdmgzf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/grvspaaym.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gbzfxqtgh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gwgpvtjpe.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/grcwlpxhj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/geohvvxmn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gxafiitjd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gzoqadjkc.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gststzvfz.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gnjvaiayu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gtswfdxpj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gvvmosctb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gjegalsay.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gqxcfmkti.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gxwvqnezl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/ggmegvozf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfjhhpp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gvfnjyygh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/ghakrbeif.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gsllbgujs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gsxjmttho.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gjrgercsb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/ghxaosmei.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gxcxanofp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gxflkiofw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsetxgfvt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gsgjqmvsa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gajkhnpsq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/ghzcsrswq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gsdeulkxs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/guqsyiinv.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gmqtqtxyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/geqejwsrc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gsyhwkuva.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gnnzggmpd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gbjqavmmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gafezzrvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gjwyuszuk.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gzfhibsld.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/grvvwvlfq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggckzsyih.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/ggfzquriy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glneceuic.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gclpwdwsa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gtflpjpcs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gubqdrzvj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gpigfkelp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcvzaruyn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gmkhwwrgw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gdmsknhtu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.hesvh.cn/Article/details/gsiirihkz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gfqhtoxhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gxpeomcqd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gvslokrbs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gcuhfuugg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gppshfogc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gbqceqqlc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gjuvgfxbw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gnjftdptk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gkqhdfvts.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gqifciyvr.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbqyscuum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gokgifasg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gophbdscn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gsisouvmm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/grveszrcy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gdzlengwq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/godwsqbjo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gklwodrqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gbhuettur.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gjvccetsg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/ggemqsbje.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gaqjxdgmk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gzufrjrej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gexvblgow.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gcuabcfgt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqgpbfver.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/grxtmqwck.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gdsnilgbk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gswlpowza.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gnfymsqxl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gggewsqov.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gagcwcmpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gwgvdoiqd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gzuncjjjw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/geoqoidoy.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/giddygsnn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gavfewkcq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gdgaguvnn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gdymntjhh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gmssqklsd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gvdowlzte.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gstbvmwqs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gftgnshtr.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gmrtzehoc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gtymydxoh.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/glooqrllw.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gyllyfded.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gqxjjjkuk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/ggvemvhmm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gthantqpg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gliggtqwl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmniwlbmn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gaohyjbgh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gpnasarsf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/guswxsbzq.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gcjdmxgko.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gjyyxeupb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/ggpoufnka.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gjqjklqmv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gkdthvlyg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gtvwgnwlc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gxwxjhrbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/glibtvusw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/galdifytj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpaqxnksf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gvyixuyxf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gckrismax.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gfuridtul.sHtML


<!-- 参考信息 -->