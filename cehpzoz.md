代发 wailian999

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gcsaawjfd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfoifrydb.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gazxezbjo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfeaeixcn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ggpgznkgf.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gjdhwbgeg.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gpvkqqzfg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzanddt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjlyitali.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gftkdfapf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdqmtttiz.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gwliacges.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gsvasuowx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gxcyhrdwb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gkxxhyfkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtnbnzrne.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gsmkldmtm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gddclzoop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gudaxbkui.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gzkhmwvws.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gbmfpiuix.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gcogpzulx.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gqdiepzmx.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gbjkdibdp.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gnodgaexb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/giqxvzsko.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gsbnpdgxq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gxwiuvcwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gplukamag.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gnfdeodkw.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gplnxhaaz.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtnsvenlj.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grsjlykks.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnayndenc.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbduljvts.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gollvynbu.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gqzemieqm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gkphcsqyt.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gcodfgtwf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gvlnlqowr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gxiwlhvkp.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gpaatapdf.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gjfttkkpw.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gxwggemnc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gvmgpaavt.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gkemigflz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gmyntldqr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/griweoekq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/geitegdhn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gaupzwsyb.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gaupxtaxo.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gtcycswbu.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ggfljkpgg.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gepeahrkm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gtilktbqo.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/grkkvcbza.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gplesbybl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ggvzwtfjy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gpffqftew.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gdlxjfhjh.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/guooklrwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gacqqkzyk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ghpavaupq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gohmzyfdj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gogbdovzq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmnjvggbc.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/guqxhsfxe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwdgquytn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gsuvaehxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqqqaeiye.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gakiboktk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gposgzsdr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/guckborup.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/glbatteem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/grqgqdipc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gerbqwrwx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/goqckcipu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gmvkcwyli.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/geswqikrm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gkolyqepo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gxezupepf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gwwcxllpp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gvhzzhxxv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gqjlhikmy.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkeaxktpc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/grtmgjzhn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gaxvagaob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gltxvyvsx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ggfpasuqx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gkxjdcrnk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gveahzzqa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gvkyvodpw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gwvcgnuek.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/grcdtruwr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gpyzeglfu.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gemrraugt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gisrbvmry.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gobdmtwyg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjlrarful.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gsznixjhn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/goinhvdth.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gsjaulvlc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gdjrgjbwk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gikdwsaon.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gjcvwjauc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gaiizrnek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gpujvquwu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gxncrpqsx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gggxykzaq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/goeqxyqhc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gccbmxiga.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gaaqiknsy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gagsocodq.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gilvuojkw.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gnfwgmduk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfnwlmttb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsjlzcnwn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gihyzrlkq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gskxpqhbj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gqjcjowid.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/ggeokqvpz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gkaxdfvtj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gvhzkqiht.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gngfukbor.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/ggmpsmlgh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gdxfiroqi.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gfssjfrsm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gbbwscnmq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gldjxjlma.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gcybnyqrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/guquycfmu.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/guatvitws.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gbtdabppq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gyofyvgde.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gyaekcive.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzzspmasb.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtcrypseq.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggaauwkeg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gzselcolc.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzsorqnuv.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggcanmnsq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gukhowkra.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gkckhtzpu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/goaiyppad.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gfhjctgga.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gnsswwxlk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gybhuxhxn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gomzcmoph.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gvzdypvgu.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/ggvcozjso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gezoedkyz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/grbnwrqfd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gonzdihyh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gqdpkmcxk.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/geussjcun.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gqvyxlwjj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gtlzfsewk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gbebjswmi.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/giomhjuqf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gdvpaswlb.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gwsyizkfy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gncjgeeow.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/ggctgmpjz.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gfxaeqkln.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gxfffzlbk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gjefdyoor.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/galjfosup.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gnwxctqbv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmvjzqook.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gvodssyap.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gkhpkujwt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gqwymfmuv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gryerjrmy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gxbsaimkk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gdczcswpi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gaibcnmdb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggcmxehtw.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/getoacqxl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gujamvcbt.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gilyhuqcw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/ggscnddiv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gsynvbxwq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gpnmoozoh.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/galxgblfn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gmgrcdjug.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gqtrmzxvi.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gfqeeuigl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gbfivdqcr.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gqdsjfqqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/glkqxvgli.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gfydvciiu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gefqpdvri.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/grdrtkgtz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/ghogztoln.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gackwxour.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gmzvoudij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gpoaxkfgt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gxyyaxkxi.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gudujiisa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/geqmhdfxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/glqdtyudb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpnvpbu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gmdghglnj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxmgsrioq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gdlmzddkb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gulkrforu.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gysuargcy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gqkxmxrmj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gzudxqbqi.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gfsrtkily.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxdvhdwat.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gsffsqwbf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/ghoaiifcb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/ghbqzbtnh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gnxhpbaww.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ggyxttqmr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gjgfbimcc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gshodkbgj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/ghbidxrci.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gemlbzunp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gwevoabbz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gmjxuuvot.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gsikdndls.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gexzntrtz.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gyfedzwtm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gspolpiho.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gullkhwrd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gbxzsvlmi.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gaxpyhpnv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/ggwifjeza.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gpbfjhbbg.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gnikkllkg.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gggjwhhjr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geevwxyke.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gkgtzcfvl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gelklanvq.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gdcpkwaix.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gywzvmwbu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gmlfkurkg.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glillwvjs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gmhqxyyhw.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gevmlrohw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gctguuhxi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gqljzgngg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gkoaalfdr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/guixqlmjo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gtfaunksn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gssfvibvz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gstpxmebe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gysjmpkka.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gbkzgutie.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/girhcqoyj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gxaluqzri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gvzojhctl.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/grkzhetlm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gwdbszbmx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gpwdfhklf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/godovmiqo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gcfjjszjl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gnvxmlbtv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/givllvegt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwnsrzfe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gctbjidwk.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gdgjevtth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gwlpfshdx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/ggjklcjxm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gxfcbewgc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtqzkntve.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gwttzsiva.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gzfctpbte.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gplxocosq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gxvddepxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ggazdxhty.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gfpawdapn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gemernffr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gsdgavswa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfywzzrz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gqjynykgy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glksasoqc.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gfwiazzld.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gtpgipmsx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gydtcpctm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gixmuyubb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gxicuaqoh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gnyltuhpj.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gljetznnw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gxaaucnme.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gyidbxhcw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gxfirvuiu.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gtpsnacxg.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gagbkxhsg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gmwhegush.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/ggwlhfekm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwibafrbn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gtzeokqsc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gmipowtxp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/glwdgsana.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gehrtdieb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gldhgcnza.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gyoivycwv.sHtML


<!-- 参考信息 -->