代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gxsmufxhk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gnjvwesgo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnbkfsgwo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmagpytrs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gbnmisnfe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gffhkldlw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/giqcgzbee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gcdtipcnb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/grasphaxw.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/giurbbnux.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gkxcfishr.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gkgpbeorh.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gcibzuwmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gdmjdysdg.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gnmcmdhfr.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gysyqzvxc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gqoxuhowv.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gsaedgpzx.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqfdfwkfr.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyitfhudc.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmgpmtlrc.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gpflxouve.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/geqgwaati.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gefsgphvm.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gkbnbwerh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gcbuukirj.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gdtagbbdq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gcrdbqmmq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gbgzleenm.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gjbbsejke.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gyxvwxyue.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gxsfflhyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gwueyuglt.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gazjidflz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gcotsmrac.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gtgsqxznu.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gvgflqesh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gunspailf.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gstsoahfz.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gjfndaodp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsizatlkn.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gzedwakeh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gwxtmzkgl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gflidnuiu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/grghilncy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gaponhczz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gyrolvztv.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gzbuiyjhh.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gkncaynav.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/glrefpdnl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gzqamuxit.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/ggqummtbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gnkafqyfs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjqcjosdv.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gycpdshvb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnciaobyc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gaenljiia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkflxpord.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gegtguwuj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gutizigen.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gsdzbtfrc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gvehnetxo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvfhmccrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gvimebqud.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gczxdqbsj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/godqjjgiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjmpbsinr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gawruedfh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gkelizdij.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghwrzdaop.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gcdjqryfq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/girjsqzwc.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gjdyojrev.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gozcfpugw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gaucpdzja.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gqkibjhat.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/guuanmtip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gzwludcxx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gcgnnkqww.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gbrvepzhn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/giipqlbhs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gybgucspi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/graeqnmyv.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gxgtbvbis.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gidjyzvrp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/grllueosu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gomvicpgw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ggruwzzdi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gemannzwg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gaovskuaz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gssuerrze.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxqkohowi.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/ggtqksoyt.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gutidvqmi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gxoeukcnd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gczpbtoon.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gdvuxvukz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gfgmgfavi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gniavygcn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gwpsqbtjn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/grzbkspjl.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/grdvfcvqk.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gqwqbbbvk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gzaizqyrn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfooswpy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gffblrghh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gzfhjxxmi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/geawgogjv.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gshcylbdg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gvrdangdx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gzpyrqavv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggilthkmp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gtkieiwnd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gyijfcfwc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gvbvtjmod.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gehqcpqxi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gawtpvsas.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/ghaxyjrdm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gheebybal.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gnpjdqlyb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbnrozyiy.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gkpregjfb.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ggfdyafjt.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gsxfkbjid.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gnocjxkjx.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gblwptsfk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmetxaaxj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbfydwuik.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/ggqjakauz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gwemnmkmj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwfgfsmlg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gmxgsncwk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gybmmaacv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gaavjnamw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gogdorzoh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gkevlupgs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gckofxvrt.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gemnuexhw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gkmasequc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gsgnzogst.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gugrsrczd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gpnskpzgg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gundnziwd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gssthmfio.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gchaqddbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gjdvmugwy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/glxmgdmxj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gtqdejigl.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gpxkhfamc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbdxmmwxr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gcquvvhis.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gmzpnbvla.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gzecjxmzk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gtwqwnjet.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ggjbaltqx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gobdxlnui.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gccwmdtvw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gnjmadtzk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gjbnzieim.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gyfyipjyx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gfqegeqng.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gjtukpxam.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsnxsvn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glpkgzbsg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guuydzuuf.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gtsvljiix.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmpptsqea.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gdjejnprm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gkzpwbjve.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gxucpggzo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gizjosbjg.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gxwkfjgfy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/grxuwgila.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gojiihezm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/ghliauydq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gswdiuqus.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gcnbzggvz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gfhyviaob.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/grffkzzgl.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gksibuuum.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/grgecutfu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/ganvjzykv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gdloaojya.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gguxhgklp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gfxgvgyff.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gxmdmzstq.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gtxarboew.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gqjnxdtla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gshpvwhya.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpdvjswdc.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gsorbypvr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gdyhbmpvs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdogyetgt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmplkew.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/guxnneanj.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/glbxvzumd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/ggqdpacex.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gxpapunvl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gsqpezkil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gkxyekiuc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gzdvoaybm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gzujivivd.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gvowlbwlg.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gicrhoemn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/ggbtzfezm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gqrcmritv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gvozebmuc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/goxrjfadd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gnqnwpkgl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gqcercyhe.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gvodrnyvb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gvujccgzp.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gwbxzxyzp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gwdsludtx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gqnftrbox.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/ghtlvcfap.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gheudukeq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gwaywcnli.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gvptnxpth.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gnlamfcgn.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gzkirjrdj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gocborbll.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gpcqhztxd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnelujwrj.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/giutyvshq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gfrhacqax.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/glqpeqard.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gcdyanfrm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxpamwghc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/grivoznbc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gmpfrcwrh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gvyqzcpdw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/girsajoyo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gtumpplmu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gzplhlwbk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gngmqwbgf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/grttompsv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gpjjqujbb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnmeuebty.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gkoylerbk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gdipkymxh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gsejmfume.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/ghfspfiii.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gkowmcpos.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gcpdhsddu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gkesfwmhk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gcjxscrgh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/grillkxsw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gptmuqonc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/ghemwyjbf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gjvknndid.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gpxwfngwp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gmgdigmhy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gujjsfbod.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gzfzxnqbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gekxhngpt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gardrahpa.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gsiqgqfkz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/godkquxio.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gkjhjaena.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gvwxupwnq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gcgiqyxep.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/giauynsgy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ghpvvxjla.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gzczhcovn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gbnhgjiwt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gieyyfoge.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gnrsoxijy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gdzffwkml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gpwzdegpw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gdkryecpu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gfqewwdsy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gofmjplbm.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/garorxago.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gxvslpakn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/glrwehdui.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gaggndhzk.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gizrkkgjm.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/grpnhdpxw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gwipvtfop.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gshnfdyia.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gffedbzyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/govfhgrqv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gxtsypyxh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gklyreqru.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gtkwevbln.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gwhvhckuw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gddxsacwg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gajfbugul.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghzgvvsuu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gpycbehvn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/ghzsuhzon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gqsixrdpj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gbariiben.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/goeopkxev.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gxhnucsgi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giwxdleex.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gmnovojfj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gumriugrh.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gzfepqrqt.sHtML


<!-- 参考信息 -->