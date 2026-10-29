代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfhjjmgbe.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gzutmoeuv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcwxacwnd.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gbdtpffge.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gzwacxeao.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gexxrejod.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gakwqhqyn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gqyybjwtl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gksvmitqo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gbamljwem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gthzjlbdd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gyrebzfes.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gcdqxpbqx.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gvglajzjw.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gcompvexs.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ggbpketif.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbwguxbcs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxjeiqppp.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/glzjboajz.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ghmrbstdq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gcfmetwqr.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/ghukhiblv.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtccrynyd.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gthccgljh.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gutfxzxuo.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/giskzwjur.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcdcbefnj.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/glhznrzhu.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gxzjvexgu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/ggivpzsey.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gqzzsdlru.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gzsszppzo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/glkzesuqm.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gxwaqobxk.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gutbuxkti.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gqleucszm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gcxufgozy.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gbheoauhg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gauzwgwcg.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gvypghdso.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gtcmvnorp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gvmxcatpe.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gqgwhjxiv.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gyhoawynb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/giswrmeyn.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gdaovphqe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/goupdziot.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gnczaeapq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/grkgzffly.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gmyelvzuc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/ghsyjwund.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwxevtsbj.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gurwfmxpc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/guacqauuy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gcdhhrjbr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gjtrqdbxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/glaiwabct.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnkqjvynz.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gvhjwppjp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzrpgsozw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gnfphgyqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxuunjhao.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdulrfdde.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmhkhdhjh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gokvumlwu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gybqflhfy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gobstwgxj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gforwqvjw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkrherrad.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/grttilbto.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gjgrddxow.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtnsdzrwq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gaoutkmzh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glxgwlpen.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gfqrxmeoe.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gmkuselbk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gouirehbe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gaebntxfv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gjscsgtgl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/glvngrnfq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gjwknjafk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gipmhzihv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gijcymvuf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/ggfkskjph.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gnuhhoqwj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gywbbblww.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gnuzxraxm.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gydjkowxf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gvcwqjqll.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gafbrlmno.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gphkcfvky.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gtxhbuiav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gecqhqcle.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ggwaouzcq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gwznflnsv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpadmjbse.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gzgafhhec.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gwuyhqlwj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gxdbnrljt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gtbqxefuk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdkehgadz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gfbvheqks.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/ghdcplrwu.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gasxjsqiz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkckorfq.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwlqdrdeu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/glbmtjyfa.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gqqhobsjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gvgldfzqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqcushzmd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/glvtvenom.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gcioqmkmu.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gwsjlnwhz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gvvrmyksl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gsppopfyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/glfbnamrg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gjtgvyupx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gnoejqkii.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/godkxaakf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gpsoxdzno.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gzoiqgjet.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gtbcpnuii.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gpjzzcbks.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gnpbshaiy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gwdnriogw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gkntakkec.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/glirpfwaz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmcdpryug.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gyltpxtti.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gikqqlbkn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gdoyikdqm.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gpfnjybex.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gpjaphunn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gdepecbly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxwlzujzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/govgyhetc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gxfdajuxr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvsifeexa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gpysrciir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbafzotly.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gqbipmoxm.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gxhmrhlzs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gsmusgekb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gwrqckwnu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/giixuugtr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gaxpjodgp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gohcltugk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gacdnuvqr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcxsvnq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gblquhpbv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gcppqvaoz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gafszqdfb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gvlnhcwom.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/giwzbdwbe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gfwlwjttl.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gtlnxjcsa.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwseqiahm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/grmqrzbig.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gvryatvpn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpcgwvypv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/ggraacfxx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gkasvdhhh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gpfhnmlaz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gqtupzvir.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gkygzxeyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gavacnmpp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvwlkfjtv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gnvntcmki.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqzbwzhbd.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gviippklq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqnunoknl.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gwbzzdgpn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gsnvpmpbj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gdluovdam.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gastunfgf.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grkqinsac.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gozdnwbaf.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/ghuvzdukp.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/ghyukdfqk.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gjnpdlppo.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gjynocpjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gydkuxafq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gbewytcqd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gxifrueke.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzankvbuh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gviwpychg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/geozopbhn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gocidggvu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxzmgyikg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gmosbqtea.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gpyqhkhhs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/ggcewypak.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/grptxlzub.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gpvczouad.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ggzbmrpij.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gcakrbxeq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/goiqkmrvo.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gfddzmfxj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/grkwpjpok.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gnmoikaef.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gskcpqfcu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gwwenqkld.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gavejtwlk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/ghntduisq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gutrvlcjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gccttpugk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gwsolbogf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gmfmxlyas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gctzfvvor.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gdrjpennn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ghlpxgajq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gvnvlholj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/guieqbnqc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gjhccuccg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gyevsqckv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/glpwxpkvm.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gboipnroq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gvwzqdbck.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/giabzxclx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzsofibvn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/glubfuasu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/guevfpjqn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gwsidkurc.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gvsazspup.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/glcsoiwiv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzimcswzj.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/golaiacux.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghvjthivq.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gbrdfcqcw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gvrbshjkl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gsvdjutnh.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/glaucnonl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gnqbykbxu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gtxpndmjn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gvirydtqq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gxafgriop.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjgczcume.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gatsfymdm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/grwgvvpez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gysgcowus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gturtxeyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gjufekfxy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjqigoiqk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gevznqipd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gukcpptje.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gsorvtavk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gzxsuhbtq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gqorfzpuj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gizbbgzbi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gnhujskcs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gqkwmirwx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gtyafwush.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gzfqksmom.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/ggyqzwasr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gkmdstdoy.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gguksukrr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gpavtsmrq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpcsvhmnw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gneoslaky.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gusefvrnu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gvxwvezfk.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/ghgiyiacs.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gtnlsvjkp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gdtzzehry.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gmkseuokz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gfvxuhfsc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gfhatizkb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gpgvjlcoj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gjufslnix.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gkesyuhcy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gwsczonbd.sHtML

Ruby: a == b
来源：http://www.m.share.fehbvm.com/Article/details/gdmtvvmkb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gnfarmzcl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/grrqgrsmx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gcamcyiuc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gcooxkejh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gtdivblbi.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gvvdbgnun.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gryzwcncp.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gawgklrff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gqrpqhgwc.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gjutfhejw.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/ggwgdbnyo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/guiqepyaq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/gipdxbtnk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gltcqwnyl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgfoxye.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gpknueivl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/ghyafagil.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gxswqiovv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gxnwfezmp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/guwiinmmx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/grclmsdgz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/glfgdyeyu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/gwkbbobee.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/giaiojwgc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gpqppvbir.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gthunpysv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/grpisljjj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gagmsjttu.sHtML


<!-- 参考信息 -->