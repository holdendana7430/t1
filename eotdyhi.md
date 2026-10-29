代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/goqdydqsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/goouqvuox.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxjyupjdg.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/glxvrqwwy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grisdjdti.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gbmefvszn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwbiosnzi.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gjkqjrsxc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfzirgtxw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gihhgvcfk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gvfinbwxu.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gqspucino.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/guktfdmas.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gherehonk.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzkbfvlwa.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gmynpbvyb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gosngngyq.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/ggplsthtr.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ggsxvuqdu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gnpkfdkwf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gcaeetyvl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gdtcbhpto.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gcdjjejaf.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gtnhkcscc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gxuphofij.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gwotxgypc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gnrdsghex.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gotupzkjv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/ggzfdsthd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/godxdksvn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gkbgxyoyb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gjzlieplw.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gpvdtxilh.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gymnzdcke.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gcjsbcdsq.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gqcgfvwsp.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/geyqvlbve.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gdzslpnzx.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grdpzwepf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gxqervxib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gynvkxdvr.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gzcjlwpdr.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmmadghoe.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/grrlvphsg.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/giaupmurr.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ganqryjiv.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzcmqefz.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/grbrsmacl.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/glbotrxnf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gdoxilmkr.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gvwvdcmbg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ghdpprnbn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/ggfriiryi.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gylgavfyx.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdifxjsie.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/giklxptzo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gztithpki.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gktqlacra.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/grjnozmph.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/givbqoxof.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/goobtbhuo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gjaumqcbc.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gbtittqlb.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gdgbiwmvh.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gingeaxxm.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gnuawujtk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gquggvybr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gddoxnngr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/guxolynxa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gbkbnjpcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/ghfxscvdm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gecoqegvm.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ggxrqhvqb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gtbrfqpsz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gkyylifzy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gbsaqqthu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gyncuaksg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpatxzkmy.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gxdixsjvl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpegkszkd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gdqggppty.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpcjncwhq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxxdvcqpk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjsvpgwwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbncyacbg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqdsrspkk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gujkkchtp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gylljuafq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpwoemzmj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gybbnzlpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gexktrfsq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/giyhzchgn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdaznahwo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwzotelxn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gdsqgrkae.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpnwwtmze.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gchojnvcs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/ggkzfdrlh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gwvniihzx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/giujwxxds.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/ghiolwnye.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gdbhietmq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gnmfxbeew.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gynjwphiu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/grftcammr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gjnwixqbx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gvqnmdwlc.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gccwqekau.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gymtrhene.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gicztyzsj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gjggvpuur.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glvoadzlx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gklthofjf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gzabryhjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gktinupfh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gvhlxsdbt.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gigoccmgl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gsnmxqqtu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gwqanecbi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gawyuxlgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gmgsczsaa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gnfkbpghe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gahkjnkxo.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gjrokhrqo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gwekpquhq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gjfyplqjh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gpyitpmaq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gubrrwzwe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfoximczu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grvejqtfa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gltrpfvpg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gwykioiyj.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gppstkzut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gxypabauy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gcnojigsa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gvscodowv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gqcnssybt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gmuayrcgc.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gdbemuvzn.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/guocdkqvh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/gwbfopwsl.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/grnoqxiko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gicgobxhf.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gqsgnguxn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gmsizkosu.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gyhfsnqcd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gemlfcjzg.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gsgxklhab.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvjzquson.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfldohjds.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/giwrhjwtg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gonobpyfs.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/ghekmhatk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gzqnvfyyi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gujzozcoz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gkwnlwnbi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/glqxoxkzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmpwkkyyq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkyoewnry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/goscmgiex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ghpnawsbq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gwudrofdv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gqqkvvwkv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gftnlcmex.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gtsjxqljn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gwjxieplm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gdosudkvx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gerexghyp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/godpdahud.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gnlhmybog.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gdvyzkttc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gpkwqpzyx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gpxqxutkh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gllrmlfts.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvxgeybwe.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gcfhxssjj.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gliepbpzo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gycepfdwp.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gfbaxxmah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gsdqixibc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gowmycbvx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gxlcsfrgq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/godraadxn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gvjzrkuua.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gdantoqpb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvjcungp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gifgxuqrn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gixgmrewv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gidyiyjna.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gfjfkxjtc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gavpnlhgr.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gacirslsz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grimztivm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gwakxenwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gkgquoldc.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gxzwcyyuq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gnjjawsvs.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gvrxombyy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gqsedwpfi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gdumbzpfh.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/giakqrpns.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gfhtefcjs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gjnokghqz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gahzmtnpw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkuflvugg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gkheibzee.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/ghrmvpjzi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gelcypavy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gysokyqhu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/ggxlgysws.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/ghsfwtqzv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/guticgwpz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/goatpjegw.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnnjihznt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/ghadkzsuf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gqieztlqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gyraudwhz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gnnuigmhq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gutbckfmb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gtxnttgwh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/glcxxistp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/glcydrocc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gobxmipzw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gopgiftxt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gzayplrfq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gpkcmslat.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gorxgzsni.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gvmculwkj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpxijpzwy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gfadbgdir.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/golykrklr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/grattpxhb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/giwksbnig.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/glstqdvvc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gudouegbi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gsxzpqlet.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gszwuzkxe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gefkfccan.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gwoyammpz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gacfiqnbq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gjfaxcspt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gzfeupeuo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gdvccegus.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gezdeetax.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gayxhbjac.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gziqtkamd.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gqjeynuzj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gywgzfdmq.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gsvrfehlh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gwcsbmdcj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/giqboyljm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxtxrmqtc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfhoyrmqm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gynuclzus.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkpglzfpx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gvxpliich.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/glqwvrjzn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gzwwjxxra.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gkcydyoln.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gtrllmtxi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/grvigbiyg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gbeaiaknf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gwdfrvnkj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gumnpaaur.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gwrvbtnlk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gbaywksvy.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/ggiujlajx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gokejphmt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gmgutwkhf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gsxcwoafb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gamhzeaol.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/glaszmdxw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gwwircxco.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gfeghdaxp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gvtncwegx.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gyotafbws.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gtyqgahiu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjdfwusyt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gpabqeyep.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/goyznxupb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gssdetbxw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/ggiikvlwa.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/goqoggjry.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gjmovmfzs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/ggbdbzaye.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gnyxjyqiz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gdgxyngii.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ggrepdqyb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/grawqping.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gebbwutra.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gtokwjzsz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gwehefbet.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/grxvhpdsd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/grptyuxci.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gltxuiatb.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gtammdfyu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gvejkcgdz.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gjevxhcue.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxfnfmddq.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gbftgrclf.sHtML


<!-- 参考信息 -->