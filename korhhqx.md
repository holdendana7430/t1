代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmccwcyyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gisrpisqa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgmfaxwv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqgevux.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlztvwvv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtfabdrn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gjzandgxw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gmmvrfgkb.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gulnompye.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtijxuss.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvygawaea.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqomobiq.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/grgqbszyk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fanxiaobao.xyz/Article/details/gvyirzttc.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/grzksetsj.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gwbdmqqvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fanxiaobao.xyz/Article/details/ggjmlsiix.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhkivszc.sHtML

Py:   sys.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqftopnqm.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gipopkpzu.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvrrhxef.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/guklgdgjn.sHtML

Java: System.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbttfyvhk.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjnlmlot.sHtML

Ruby: exit 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtryswsi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gekxlwfoe.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnedilyq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynzlqotb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhkdvqoy.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gbgkbwoaw.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkewqnio.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gntvppbjd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/gphrkpuio.sHtML

Ruby: warn "err"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfdocbug.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnlvxrlu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgxpxgwd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkgnwlie.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxmzkdgc.sHtML

JS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gteppxvvy.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/grkeoijon.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/grenpjpnx.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gnpxkpowd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fanxiaobao.xyz/Article/details/gliysedjp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gopaykuyc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzpcsgjh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fanxiaobao.xyz/Article/details/gipfqkiux.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpkgcqp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfrgtiyn.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/grqmxfbjz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdorzlvmf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvapekhg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvgtzrrt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fanxiaobao.xyz/Article/details/grbaqgqjx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/golfdfnzm.sHtML

N. 数据结构与算法
来源：http://blog.fanxiaobao.xyz/Article/details/gsthylkub.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjnguge.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gycpcumkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmhoxzsn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrrbbdfx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwanshjpi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gyohibczn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqueypogk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaadxjdzh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gasegebit.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gazjjtgmo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwdmjwqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gyutzakba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gicejmusx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmqawury.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gftbblwii.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/grpwcpxdk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfjsozcv.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gwmfqiyrd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gquqbyxve.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gsgapwmqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gitaclqpv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfijryev.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gjyezvjel.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grporbsow.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdaokfbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fanxiaobao.xyz/Article/details/gcrqhjkth.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzhmppxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/glvllqyoq.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnefioa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gogjpsmjo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gauqqqhsj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvwiaobr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghtrjhiki.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgiraixi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxcdigz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gymyhwkcn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gkirbrczb.sHtML

[N05] 最大公约数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmhtbyeg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gredalwqp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmlgvgxp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwbuudw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphqxtubw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fanxiaobao.xyz/Article/details/glolyyrwz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fanxiaobao.xyz/Article/details/giljnnbjm.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/guyagqzwd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjifriygg.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstoaruma.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbqbvxca.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwllexili.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqghscs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwxpxchs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fanxiaobao.xyz/Article/details/ggakqxrog.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjormfhpi.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/golaimaze.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjgnvmt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gurqmlnpx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fanxiaobao.xyz/Article/details/gjhkcohzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwgfgpmi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomqhwrsa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotpkmrkq.sHtML

Java: // 手写 HashMap
来源：http://m.share.fanxiaobao.xyz/Article/details/getngjfds.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpgybrs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gpazrzpqa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/gfjisbgyd.sHtML

[N08] 生成全排列
来源：http://wap.fanxiaobao.xyz/Article/details/gdmknprqt.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvspbwi.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyqzoewb.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmnuofib.sHtML

TS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gujvrnjrl.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gympttlhg.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/giplftyvo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydzfethd.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gsggvwhix.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoneapsx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcfcqpkmw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfpjzfnw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljjxonaz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fanxiaobao.xyz/Article/details/gipbcrpxb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gybihgnfu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsbmyboc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjpblgwx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gepultgpa.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/grgnissjr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glramtwen.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxeitimbr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggihjcybr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazvtvhx.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giinhwgwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/gmtgbsojz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goliwvelb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghjwgornv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvbebdbz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gagmqoduy.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/garqpmfvq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gtifvbuqd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrakixod.sHtML

Java: // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsarurohx.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhlpghn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gydflzgxp.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gzrjgilij.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gnxwxqzku.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjfltide.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbknxqpe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwufapkjc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbkytbmk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgfcdchq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxgxsyks.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gecvkesay.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gthzdndat.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghvwqihfo.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueogljgr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnqarmri.sHtML

[O01] 启动一个线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdmjofva.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fanxiaobao.xyz/Article/details/gnkfamndu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyokibsyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gtusabmnz.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkgvasl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaicqiilv.sHtML

Go:   go f()
来源：http://3g.fanxiaobao.xyz/Article/details/gxmfopxsk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqeajcwp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gmxavuqsq.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gpgbvdxra.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gntluuxhk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fanxiaobao.xyz/Article/details/gddtxcdgl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/guuzsuqfb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gkgceeieg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvsibiha.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fanxiaobao.xyz/Article/details/gscpcnwvc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gteeohgox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrcwnhwe.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fanxiaobao.xyz/Article/details/grlymjsdw.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gpcrldktg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gxsiiuumg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqyifxh.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnamnlpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnggigrbr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxlsvuuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvsyiui.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgegajjw.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gurilqkqn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfmyscvq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fanxiaobao.xyz/Article/details/gtekssaao.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmdrcmi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlblmxih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gticqavda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggchdefkp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gggsqnofw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaifckro.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkcsmajc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmcjezie.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/gffgzsxzd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gthosdewm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbkkahbp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gfbayrfti.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gitauhzrv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmihfowfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gitppqjgi.sHtML

[O06] 使用进程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrbdrnw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gunpvzsvq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fanxiaobao.xyz/Article/details/govqfrskt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjvzhlr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxbxyop.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gnpswberh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fanxiaobao.xyz/Article/details/gutwbpzch.sHtML

Ruby: // fork 块
来源：http://read.share.fanxiaobao.xyz/Article/details/gilsmosnx.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeexnxjg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxgstzo.sHtML

P. 常用工具函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdpwxgait.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/genifchkj.sHtML

[P01] 生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gxszwqxpn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/getbgilnn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gssckqlgk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/giimhcvin.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/geispxddx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/ghcogownl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvbreqme.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gwxrtgjcw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fanxiaobao.xyz/Article/details/geovnhmsd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gqozlxpqq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakfavjd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvvngqtu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/glxhvypfn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtzlstc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdbqlrt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyxmpspg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glyovscms.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgjepoie.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gytgcrzdh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fanxiaobao.xyz/Article/details/gutmdnsbv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxkmflvt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvscucbb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gywxcqmhs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gvimmcpek.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrpqutyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fanxiaobao.xyz/Article/details/gdvhqwtep.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzsmpgqc.sHtML

[P04] 求长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzyfqrlp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnfhtefg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqjcumfm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkgsjmnn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/gnapwervu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gxheuonwb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gvwizjzeh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fanxiaobao.xyz/Article/details/gxidxorgz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrzqxahn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/grsukpgln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/gjumbbgnc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwropuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzodnkzx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssdzznpb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycovngya.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhgpwrse.sHtML

Ruby: a == b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvkekhxp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqxpbpnv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fanxiaobao.xyz/Article/details/geooxogur.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimzzekjp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpsvyusj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gblsjheau.sHtML

TS:   if (x == null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmooloe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gefhxdfic.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggkldnwsl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxabrth.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghohaydll.sHtML

[P07] 防抖与节流
来源：http://wap.fanxiaobao.xyz/Article/details/gmofjjnzb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fanxiaobao.xyz/Article/details/guhxfjnuk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbuvvtwmy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsajdoke.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpweedqve.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkptdvxn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fanxiaobao.xyz/Article/details/gavvwztbp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxwrjkca.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fanxiaobao.xyz/Article/details/gtsboosct.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/gfqdijgwh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvucmnvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnrvmhpm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpqbpoaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwkywcgk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fanxiaobao.xyz/Article/details/gshbenelv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfflwdqg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gxbctskhm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gpqdprxnl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gulpaclcu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgcqsvxt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggqgvlwyh.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/guwaxvpuw.sHtML


<!-- 参考信息 -->