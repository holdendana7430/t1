代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggymimpjf.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gmfgsultv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gawuygheb.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gutbjujno.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gvviqvijf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gpbgazuts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmlsmsdxq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/ggmhgrlhg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gcqfonoko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/glxgfbcjw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gxpnjsguk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gtlvbsxdn.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gbtcvhhff.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gvwbafwuc.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gwnkgdxfb.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gylgphgqw.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gykarqggm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/geyhbihgy.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gkekxbedx.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/grdwbnbzc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxejxexa.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gjhuytjhj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grcnpkfkt.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gemcxklhb.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvcahtcgp.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqyexfplg.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gmdnjklgw.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggcjangtw.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gustmoaok.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gyctmehnr.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/goyoocyyq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glzqgxqgc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gqruvcjot.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gjudwbyxs.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsbexxwnq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkqsrmwdc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/givtokvrb.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/goeehujkw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gwfrtmmem.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gczzuttgp.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gczdkfwnx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gjolprbdc.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/grbywqkeo.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ggchyzbrt.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gajsprppp.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gixpnekqz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gxdzhyzzw.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gvijhgscm.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gyiwaihyb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gvtstizrw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/guvhpxjjb.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gjivajbvg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gejoydsfc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gumchngfe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gvdxvdkkh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gpnrrkixa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/geszygzfj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgioyvow.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/ghcjiymxh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxekolzuf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gspfqagyl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfrrqdqjo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmzcgbow.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gfsgderzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/graubfute.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gruwxdihv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpoampfyz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gsanavqho.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/geflmezzb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gvcvazdre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gpswixiqo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gcogqxbfu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvifikbcy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ggogwgeat.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/giagmqoum.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ghhkjoohf.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gzuonwaqs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gpqpwqzef.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gsjzqhchx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/genqbbawf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gcstiaamk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gnecqnaxs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gbfgvlbkb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/guygtpgrz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gbqukfqeb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gnpldrsxb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gkrwmcfsd.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gignfimqb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gyaerkjfv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtdjfldoa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gnpjjjfyu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/giwzasquq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/guttnfhvi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/guaqgxlhm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gyjhdnoky.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkillzxhc.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gslflbokm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/getvmpmdw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gtjgxjgsp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gqdzayafe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gohhrfcfx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gjshjupks.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gniixudsj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gfagkwgtk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gzjqzqefc.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gpffeyqeo.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gutiijpfg.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gbapnzhgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwsxrxagb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gltyvlgoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gysxdymce.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gerxdiejd.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gaerdjrce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gkiyffuej.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gsfgoscvv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/giymyencp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/ggvocdnjk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gbmttncmw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gmcmcnmlj.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gswpcuzsx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gbampekhd.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gsfeamiaw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gcwjjsspe.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gzhoqmjxc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/guawegope.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gmltfseux.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghmextkfg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwredegaz.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmaxnatvc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gksmzdfah.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gywqufpgp.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwuejzmir.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gjyrydrmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/goixpciws.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gzuivzkfk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbpgfcsyf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gckaburjb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gaeaohmpk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gijamwfqi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gyiflmhih.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/ghsaodeqn.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gevxtfbhe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/goiznqnex.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/ghnehogwj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gmgibsokn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gknuizzom.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gojgktpme.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/glbnydret.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gklkatvoy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ghwhwskik.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gzcxbnqrs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gsxptcspw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gaajbxchf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gxhntxdyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghekjgbug.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghghuwbhv.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtzbrntbk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gzgoyuqtv.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkfxahq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gfrvruuqd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gqbowatjy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gcmmlmmer.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gzzyirtwk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/ggpfekdpw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gdzpoiict.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gpwktcjic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gyakmuuty.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gstyhrwfu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdwnjouxj.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gncarltgw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gobvlffam.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gomsghiah.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gisnomtdg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gadhedndq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gvtizrmhc.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxkefzkwa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gtarvfufn.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/ghqdpheti.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gwvspgthl.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjekvqbrx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gpaynakue.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gclvymvni.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gfxrlfmyw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/glkudueer.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwjfphiiy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gmvvgfqxt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gisflzdip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/guhatvkdo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gobwpvput.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gkolvgmnm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/glueziimj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gmwuepwye.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/guusogemv.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnuxyodom.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gxdstspko.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gpuquytkn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/govjxtblo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gpcdgugmy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpjwqqukf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/grnupxqnw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gvyfrbxgf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gkzwoqjnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gqdykxaor.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/grvnbcdhz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/garkxljna.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gnclwiujm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gwtfnzzqk.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gcavegzps.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gvzfjliyj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/goaxfbkgo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gcereeqrc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtknumdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gtpqhpala.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gznmmbcup.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gahvdtagk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gtrczwswo.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gvstyuawm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gcnltoctx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gabkrkckg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggrgvkurs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gqtkujpoy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/guzfrinhr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gptmdybux.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gbyvaccrk.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gqlgmohnd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaktpqkty.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gjtvedbnl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gahyjdpvh.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gvjbqypdd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gvczhkqdh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gfgbuxssv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggqckwrds.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gbovwhtxk.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/grrtdpzay.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gujtriwio.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/geqcvsjxc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gujzuyezw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gnuxaeewg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gccugfpnu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gmushladq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gqzahhqez.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gqmqkywmb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gswficeme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gwtjhzzhy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfyvavuoh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/guaxhraqy.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gcpkjnxog.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gimutzclj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/grthiyvmc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmtyqlapu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gwuytxjyo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gxumxsyib.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ggfezdqwr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gskxfoaoz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gquqjiajf.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/grweckgjt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gmqvrbser.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdodwljkq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gdbgvzjje.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gwiymcjtm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gpyztytda.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gyzrajdqm.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gsqaseswd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwxrudciw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gcfzpbljs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gzalqfter.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gdypjvcsb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/guidavocd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gobezwrql.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gigdmvssc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gufdzawyr.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gugfngkjr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/ggadhomiv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/ggwnhxuvm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gwoazthuz.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdczcbjox.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gqpsyauqh.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gispnadrb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gqstdkpep.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/ghlzpuhrv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gjprfltsc.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gjytlzgcl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gdhfeules.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gnofuifqh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gfbkffzsi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gxauuvpnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gdmcwzydy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gmxctylsp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/grxxqzxyy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gsukpcuqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gqyuxdvqn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/ggstcmesw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/ggetgowrx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ggfglhuju.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gdmgzpley.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gnwifmibe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gsifrasnm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gufpejiek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gryznujkn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gennihqxn.sHtML


<!-- 参考信息 -->