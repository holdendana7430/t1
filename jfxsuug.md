代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/glrmswnvu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gdgommoai.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gkqgscfup.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggzekfxho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gzhuwgmps.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gwdgkbtax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gixkwuxcj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gbsdhyrif.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gqkjoswrq.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gsegmxnyt.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gxfabzkne.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gadbqdssz.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gpnrduegw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gucwkdadk.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gclcvxdxj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gomptvnem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gxphvotij.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghtcvgvwa.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/giwhoixyj.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gonbjmcul.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmqsvgqhh.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gajajyvai.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gsuuanweg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfxomojfu.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gaqvawpcv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gxbszyiwr.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gajsfgcwv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkiddkcbn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/goxanshry.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtedcbwxn.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkyllkvws.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gocnorrnu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gueijunsc.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcoaaxzgx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gkvwpqbfk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/giiasrrkz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/ggnkbkdbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gbhbsqwin.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxpxxzgzl.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gdaosxgrv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhsvictk.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gbjdyxivi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gojvbcawe.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gdpgsiiap.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gbnqqyzys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gryrthekf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/giizwcjyt.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gpgcqqpmb.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/guzoirixq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/geglkusgw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/grkxtobid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/ghszddpcn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/griwovhny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gowypsdxt.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gunkejbar.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjbvkqrfv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/ginghjkhc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnovlvzfe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gdtqtevkx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gnvohelak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gyamaayll.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjxzbcjlc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glphecbcd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gqdssevgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/glrcqvgqe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gvkyzkgkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtlnuoxyc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gzmdmaltx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvprzhtbc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/grprgwtdk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gkshbtgtr.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gvnujpaln.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gniwqauqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gzxwlmdab.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gzaktoeaz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gbqnbdqpt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gmkhhxprn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwlbivaap.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gisphchbt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gowymcyxc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gwqnxvnfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gunwfllim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gqklhzoju.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gzujnlyvu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gtzdasdwe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gkbhlkycc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gydjzpdwh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/guslgequa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/guhwuyiri.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/guzicugcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvwajvfcs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gavqnzouy.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gjvwgymzs.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gmeenfapl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gyvuemlne.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvtryjxid.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gorofvcje.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/golkmcssr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gystzcuro.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gulctcime.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/ghipaugxn.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ghzavmuwx.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ghkurmqyf.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/goorloqyh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gdeevqvkm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzprhbdqz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gfvenuhdi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/ginktkoxa.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gtufhhyxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gefkmmrsg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gzuzafjef.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gznofzngb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/govsnmuxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gtnmeykel.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gubydevfp.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/guiihkaxy.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gieryqowj.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gxcudqvnc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gmzxkejbc.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gmdjvasdl.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gemcphhmd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gylpfrfyl.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/guqxxpjwg.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtiwdjzoc.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzpnpzgfk.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmremgezp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gcoizaxzy.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gaaspjjkw.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gjwpobavk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gxfclkfnl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gderncoqm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyskcrvmu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gmejxwgse.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gblwloiih.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gqiigucyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gohrfugjq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gznjpjnda.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gwcdlbyfy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gggvvlmgq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/guegqfynj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gstxuozcz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gpabheebq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gnfiiytfi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gbpfvnbne.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gqunbcpoc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gdcytdszy.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gcxarjuyw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gjysqdsux.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/glxflxzxd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtnuonoxu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gldvavyih.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghwnfwgpz.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gtdgkjwre.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/grawlbrwu.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/glmbefhgq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gjevweeea.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gpzwaanvn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/graloxfjf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gctrasofk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gvjswynsl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/greunxfjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ggwgnuhtd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gvvxpnaqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gzfggmasl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdoobyspp.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gkpaffmpa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjqvwajja.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gxiugugcx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gzmobhbpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gibqblwzo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gzigmjbst.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glaylmupc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdyethlid.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gongljlyt.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gezeabxme.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/ghnobpptx.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gglxjydxg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/ghzealqwo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gcqqiljzc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gbxhhvlkc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gjpwumxkz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/ghraasxio.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gjimihfxi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gycdywceg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/ghapceyme.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gfkfjgmcg.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gwrijcefs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/grwdfsixy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gxunrouvs.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/ghhjydkec.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gwaghsshf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gpmubwbdb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gxqabaldr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuswxsiq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/ghtzrfqpv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gghjrqpri.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gudezmyds.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gzzhirana.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbebjrfyy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gkxbyhfni.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gujyqzneg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gnbtljcgd.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gdwenoijk.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/glosbyhdp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmwymsatk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gkpssppnz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gxfxcyzao.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzvqqveht.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gfkvswzkz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gftbrtqfj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gnlxlwbth.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gybykhcle.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/glsmpngew.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gmhjeldfv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gtyrfbpof.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gshpaydjo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gskpnmfrm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gkakzglra.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gfhvnqwvt.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gojsfjvsv.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/glhgbewnp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkybhxdji.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gcalfpvfj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guneihziz.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gzvqypygi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gspedmnaq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/ggoingbfo.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glntaxphq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gjzmvsjtn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/grpahogpo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/ghwopktoo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gxdzmigdg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gjgepxmhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gcglmtigs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxssoclb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gnitbrwzb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/ganismnfk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gbawiryup.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtuiathte.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/ggfdohsux.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/ganipmypk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gqislfmxd.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gseexegkr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gpemxcmir.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gfbfptejk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gwtuxmlmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gmyzihers.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gsypbzbgg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gobpxprgp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/grqdjkflg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gxvbhfesr.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gularixgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gjiwyaswb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gpoftahsa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwrkmtfml.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/grrfxbnyi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gdzikaado.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/grvvkwraw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/ghqiwzjsm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gldovezcx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gdgiwzxzo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gysesqfau.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gxpmvlfhz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gpyuupmcn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gcskweovf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gnbrzwmru.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gswpbtyhm.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gpmnfttqm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/ginflurps.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gnyuzqmkv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gqavqlthb.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gmsbsaxod.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gcbankobq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/guntoiojl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbharjocv.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gybbdzemj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gqdudbwvb.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gqxnrxalh.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gguxudqum.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/glsejnbtr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/glivubknj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gbhhpedua.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gyonmubmz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gdzjsasjm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjfrdcy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/guskxrcth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gvorlzces.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gisfjmlvx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gmhuhsgci.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/glctpvhst.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gznwninxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gaewwcvug.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gzokxeiwm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fehbvm.com/Article/details/gfryspuei.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/grgowpnkh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gmoiddblq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gysewklms.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/grpomreuv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnngjuhle.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gxwlperfc.sHtML


<!-- 参考信息 -->