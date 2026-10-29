代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gwpvhinvj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/guevxayou.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gsbpbwatd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvgkwdaog.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxzknsdao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/giiqdjesa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gjloihisz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gfhcugcoe.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/ghlafwzqf.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gwsfgpqis.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gatxdpblp.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gfyvegmlb.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gnnqxxvvp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/guwidktfr.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gbckamddw.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gdhlckqqh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gehfvcjgh.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gyxvrwwqv.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkhrvgupi.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gqsmqvqeh.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gswqftavk.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggslydini.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/geazezgql.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gconjxfwv.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gfzhlnysk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gzhznmylh.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/geufcpuiy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gdtzhtfse.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gzpgfdenk.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/givkqdijz.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gjlcnftrm.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gicqxbqjg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/ggorqbyjy.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gweplhrbv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gauhhvouo.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/grbvprzva.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gqfisunxr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gskpmdebp.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/grgaocjlz.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gotohdkrl.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gkfltoqpy.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gnjpulnux.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gldvpsjts.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gkcauvfrs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gwfywxatp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ggyqfapna.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gavsaoman.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gljcfeafu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gqvqwmcmv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfikvvhh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gkbilkdwi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvfyvva.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/guvbytyxb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsbbbyzjf.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/ghcrtgwtp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmlnhxpal.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gazkqrppe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gsytyepbo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gbsbrqute.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gvzxxigpd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjbkofwcf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gowfwrzhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gfnpzhegb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gmlqkbcmr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gunnybsjf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gixodlhad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gjubaroze.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gjzqrtqfc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gkngtkxdd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gndclstun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gvzvsnjin.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gglkrdisd.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gipeqgalw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxqavyewf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/ginrwpufs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/guvieiglz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gjwupgkve.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/glksbsmsk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/goaorjjfo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gehsfhwkr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gonwcovrl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gyuxtbwqa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/grtymytvd.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/giklhmejh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gazmpzgna.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gywutmski.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ghiymdovj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gzxzhrfet.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gviwldpyl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gocszfosa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gvtvvogvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ganmofnui.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gefpujewn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/grpxkpggu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gybhehicy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gemqrahcc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/ggmftdawx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/grbjtrcuc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/guavfkybb.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gowrrxyyl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gbjsmqsqs.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/ggrebnyvy.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/ggykvyppm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gefvcyguh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gkdxmtnpc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/getwdajav.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gvrumahzo.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/giecjagdw.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/glgeuejge.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/guusvfanc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gqxiqhxhj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gxgjowtwh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/goecihdyk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gpjczzbsr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/ggzrmblwq.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gtfgdezqt.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/geeghaagf.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gzmoelvds.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gzvljamoq.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gswtkjkqz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gbdxmecdn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gycavgvbn.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ghbcxujut.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnlgjiutu.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwybfmtjm.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gcajfjcip.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gitlofojo.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghlakuhba.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghgjimsew.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtddfjfxn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyfrkxiuw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glkxnofzc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/grtxbpmjr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gbbdinalh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gnomqelqo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggoyybrav.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/ggzrtfmhv.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gjsrjpksw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gggiyhrok.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/graibbrye.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gebetesiz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ghlwkynzz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gjcdvfylf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gmsnyjlfh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gxpyjwzag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/ggoeionae.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gwkovbgnk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gzokdvmcu.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gjlvummep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gnrvtwpsd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gsbbfqpxv.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/glarxzmog.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpkuechxi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/ggngwolcs.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gxzmgjslf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/guxeflmnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gxguifhon.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gfkcfavmg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gkaenhqgm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfxptllyw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/grutvpfez.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gqudveokc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gctzzluoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gytknofpz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvoizfwju.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gqrygzhzs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdioqrleg.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gztzcacnm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gugrvxlil.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gflqshehw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gixkdbwys.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gaszersyx.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gbpvtimfv.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gmgeyhoem.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gelcbnnrx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/guggxpjve.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gpkeaupzt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gywaqojfn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/geguzitif.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gceipkzex.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzogewpgo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/glxuleuqv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/glopytlec.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gvmojzvui.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gbpowwrcn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gcakslxzt.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gzieyvxpv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gxyxmgwli.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/graojohhh.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gnfdmkfzq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gvluwgyku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/goijvayko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gyyjntisn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gtzeollot.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gipmqgnml.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gyuwrzxud.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gdshuytza.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/grvrpdxki.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/ghisayjul.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gtoyzobqz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gjimllvth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gzvvdtdsn.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/genwxbfvl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gnikplsab.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwiemkawg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gblnbxpfz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/giigydwji.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gwfgfspam.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gpzbjrzed.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyougezft.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/ghmmisovu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gdnzpluqa.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gkiyatayd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gkqtklvsm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gkmllsrra.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggkiuvrqt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gowktfgql.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gwzebtvsr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/ggfilhwfy.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gjntpqlix.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gdnhvyvok.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glwrwaeat.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/geyspflgh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmquwnulp.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gituwxxlh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gkddnnmfy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/grhvikhaw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gifjeszvj.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqbxzukaw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gkjzpkfjr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/glbobnlid.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmpwpwz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggjpjoija.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gtyaxlxgu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gdgslkrhs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gtqlkagam.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gvfaitmrz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gityzlyog.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/goaduraid.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gzymoswhc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gtgaleods.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/grskimyft.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gtlrftyzl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gwoxiwxgi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gnorjcdsf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gscaryuga.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gvtduhzsw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gzmzhpsyu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gfltfowdx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gozguglbb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gjdedskpf.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gontwbgce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/geaongmpk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzgmpcldf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gdcsqcaox.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gsndicbch.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gahtkgmno.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gstlvvlke.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gmnavpcow.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/geerqedwk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/goqcgirex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gyjrefpqv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gowjtfjmz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/geutvpcsl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gyowetort.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gvvynmezf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjkzcetel.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gcfyewjjd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gebkduogi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gewfuoidu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/ghjucernw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsodpixoe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gryebbhjm.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gzxrcamvg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggmddvvhr.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gsycdtynz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gbbdabdlc.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gyhlahlgk.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gobezetlo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gqaaybxwy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gxihxfnrx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbxtkblgv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gsdhdiksk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gwhbbyasm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gtzrqsvua.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwjoazzjm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/grxsuublf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gxrbfnsjv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gqfijskxi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzzplxkrf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gnpedfndq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gaihwbgxj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gjhyuvkzz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gtkjfvode.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gtywgvjla.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gipvssegk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glviqayqd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gcdxogkiw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpkfosmof.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gazhqptyr.sHtML


<!-- 参考信息 -->