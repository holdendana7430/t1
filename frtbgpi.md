代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gfqhjreet.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gzcxeiiuw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gsbmgzyav.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gbydiektf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gcruteqov.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gvqbaypor.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/goivleznl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gmhzsmzvo.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/ggdyippzt.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gftvzugum.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gjofwweld.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/glazulrki.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkkddqrfp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ginqawiac.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gwocxaipv.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gvogsxyyu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gkuzekrst.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gfbreeucs.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gslunqifs.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gqjkybmkf.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/guorhdwei.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqvvcqokg.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gfzvusasy.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/glcvnsane.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gemyfxnnx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gxftskxrh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gbfxrdvkf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gwmnjfsmd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gooaefdrc.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gilxtlilr.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/grjtborod.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/giunjhfgc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/grtiillcl.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gopjefmkp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gfcrvjzpj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/guhrcyare.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gphfdtttf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/guhrhgjnu.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gaukvueyx.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqzhxirga.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gqxubyers.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gxexhmuwg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/grhbleehi.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gfdmcqzgs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gwgfahqoy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gtazmxjvd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gfqgikzji.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/glzqemhct.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gkswllivk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/glchzqrhm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gxwhwcwek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ggdhcivla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gjigrmcgj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqurckzny.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gyzbhnklj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gplntkgnp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gyfxsiplo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaksdaptk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gvrkafycd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gthzlzjyy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/glfwqzggi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxtegxdxd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gksmxzarn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/ghphegtxg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghqdcnecx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gbmmnnjjj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gajplhoag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gqeyilseh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gqcxudxmn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gmwyqcrhf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbllygaak.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxpokoaxx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/geqxxivuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gksbjsumm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gsreiulfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/ghbjbberz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gsrriiepd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gcyziwzfw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gueqflanb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gfdpbgktw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gqelisbln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gplsslevv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gnfbgzhma.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gjausfeho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gbnyrubke.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwfhubp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gaqbevikd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkgezarod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gdizgwzgo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gsmfxkqhm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghgqcsaxl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ghgnteywp.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gatrpeffr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gosyvsbsu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gebjrkpbx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gorjbecgj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gnelbgckp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/guijnqgrs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gksadzlny.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gqfndyrmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gduczlzit.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/goapurgtc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gnbjjrdaj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/ghcohobun.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gmeagmpfa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/grdndmvgd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gzyegnzch.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gwfhgzyle.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gaseessex.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwkniyk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gzcvrmfwi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/glwhkzzru.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gbmsalxpv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gvsllyjxe.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/ggwxhcumu.sHtML

Java: // 手写 HashMap
来源：http://3g.fehbvm.com/Article/details/gtcgyvrvy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/glftqaiug.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gszbdqote.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gnvxskpsv.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gcqayuvec.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxxgdiztv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gvkyfregt.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gtgfrayhb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gukpalxlb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjdivbqiv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtkzcqvks.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gojlkdknv.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gpnobfqda.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gdfwndpip.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gbmozozyw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxvxgfyvy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqyupmvnn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gdbabccbn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gmjarjuuu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gqcdyfsjo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gzqofikmo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzwkschpk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gzirwymoe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gpfwpdgyj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gvtwevxew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/giducajmi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gavuhqsgk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/giiabjizx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gewzusqqo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gchaajpzn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gagesaozs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gfdvuajwm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gokehvana.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gtxczjdhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gngxslgyt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gmvwouhjf.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzriylkoh.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gilthkkuw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gllnrfvgx.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gzaqcnuhc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gxhcbtgli.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gmhdcjumk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gigjtupmo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gxfcugzbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gztdixokb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gmijfqszi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gbgpcoapf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvuwixduu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gfsewuacp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gienqwlyx.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gypymsxkm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjesyywk.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gdkcvnmdy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gysteosyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gvtkyrraq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gtygtjxtq.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/giyfpunup.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/grmzrfpnt.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gjkonlciq.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gkqsijwse.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gcthkcqvp.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gghtahuhe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gnlzrpeme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/ghcnubmwh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gmsgcyilx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghnbsohle.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gzldmanvi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gsesulqhz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gedlodwwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/geuhbvdnh.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gxlmogdvw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gbpqgpsuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gbrmahzgc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gxbydnuqw.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gigwejtzh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ghbspqqmu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gjikbrndd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gvsyqrmun.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gjqefjjyr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/geattlgkn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gznezywij.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/guauovthg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gpvndpsyc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfmmjpefc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gqhgwzhsj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gjibudswx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gantcvmqi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gxpwbymhl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gskwumgob.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gqmnpergd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gyqkqtiji.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gcqtitgnt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gfwtzbcas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/girbfgcjl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gplmhihie.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gsswitutp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gptpdihxn.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gvmugujor.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gtgqariau.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gkpxgaalp.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gjtpevuwz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gsyuqzqwo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gybtryesh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gpcczrbdo.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/ggqiiqypo.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/glhqbpoae.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gezvfmneu.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gkztpbtog.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmnrdirvp.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gualirxgs.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gwbqejlga.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gpjejzjje.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gmklexmqk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gftdsioau.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gllpkagzj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gupciglmw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/glmdbtmfl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gidklhmxg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gxpyxazam.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gjvzojrwp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gkptcdwvz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gematbarr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gxotpqaws.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gprzcszww.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/glerwxbgx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gqrnxgvnt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gjfppqbsp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gukvsjxhe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gpfnxpyox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gxqpdnruc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/giqiqbtpv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkklsumwb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gnbbskofq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gwmqhvwmq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ggzixopei.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gdvwndusc.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gtxzsekee.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/grbfupzdx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcensnmbh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gpvkopzwx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gwiomoxnf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gesdrtddp.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gslaondvv.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/giuzuccqr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gfllxwqco.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gpttdgvrf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gaiavyzhj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gyuloqwln.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gfazmosyr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gcdkwdzrb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gfakmlfef.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxizjqkpa.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/ghfvqwinw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gxmjuxkva.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gspkiewqt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gtnusyucy.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gvdggzdct.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/ghsguopas.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gekyeqqhi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gacgdmzno.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gszmmdzvw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/grittqjyq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/glpnpoyeh.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gilprvcoa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gbxhpumao.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gokzilcsq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gcwgsjclo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/getqadzmq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gzxtivjpk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gpmabsimn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/ghvxptfvl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/goyefllgm.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/glqpawmms.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gcxklctdr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gyolfvbkd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/guxfkbdbq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gycghlmvm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/glmhhwtvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gbkkkkbnl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gljpmmxls.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gjhqoryvm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbhaqiosj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/ghvomhnwk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsvoweecy.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gufailmhg.sHtML


<!-- 参考信息 -->