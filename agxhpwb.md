代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gcjpzwypw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gzbqrarie.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glbceixyy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gmumybuyx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gupvawiyk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gwjhixqfe.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gbefzwakh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gpnhsopcj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/guaqejmjj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gtjnkzfof.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gniyvyxmz.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpydsrjgd.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gvsvupcbh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdrltqebo.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gwisqunfz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gqxnblysn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/goeysnosc.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gpycmnabj.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gyafjscyv.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gnuxcirvx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gzrklsjys.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/glgnqupta.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtvkbvjgi.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gskjhmdoo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gktsasuuk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/getawfasb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gvbvfsdjt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/glzmvzwjo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gmulvyqwa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gnkpxpmxo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gawykmnis.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gfnaeyojo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gmuyljtvp.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gqqfaeonn.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gxspofzic.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gkzetysov.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ggawlaffc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gxefvnqtt.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gqelgioji.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/goywotksd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gblcafrfe.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gijxmjtme.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gamkkypdu.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grmijpzgk.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtmvgfuks.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gfrfghwwn.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/govpnriju.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gguarbfbg.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gtcaiukmj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gikytgfoc.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gohkucruv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gsuqhxjpa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmfdbtgxd.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxvvmrveh.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gvwfnvhzd.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbtyppymd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gmrousbcn.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gsrelrsiq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/grhghcxxb.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/guianujml.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gmddzxjlv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gkwutbecf.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvffzcadc.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gjbtlhyrl.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gweuatqbu.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gkmunzwkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gnyawfypt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gdxudmcky.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/ghwlgiyot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gaitvlkkt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gkhjaeyps.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/geffrvxjp.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/ggrfguwpv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/glielvint.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gtxvmadym.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/grdcofjoa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gajzoslll.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghvpeyihr.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gpphphwnf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gctyfljyq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gbwnmyeqk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsffxpzrj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gvvcixpmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjeowvqwu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/glphzgcwp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcjppjjey.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gneeepmds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gqkcaegui.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gquqnfjxu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gquophgay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gakalxcea.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gfyphbzgv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gsjtsscro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/giutnxiaz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gipnvkmkf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gvrabzeib.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfvfnaczk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/ggvesipcj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gfztwgeax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gdubgjfij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gevifwttd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gnqmpihwf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gjxxtqbnu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gifdnpzza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gclotirqg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/geuaetmbv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gknelvyfy.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gdzfviffv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gqmcrxmsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gbcczuika.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glmimkqcl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsscuvjon.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gizesjkqg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/guvqxeakw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcuauxuel.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grszdvzxu.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gfpbjwlcn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gvfoceviv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gwqkcuypa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gelqckdum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gxncxdeyv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/geyxlcwti.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gorelfxlm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gaaicmukd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gkidehuck.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gjujkizpq.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/glidgfzss.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/guhjkpdsu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjixtlzhr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbefczxce.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/glceojhqq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gwrxwpyrf.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gupfujirm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gfylhdghq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gmrifnbfr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gojkzptnj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gpknkiebt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gcdueikkk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gwavquyod.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gwddsflvi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gjzqaczmv.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/ggpbzsuzs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/geoxgdpby.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/girjxxpfj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gvblpteeh.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gaiomtnua.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gqlkdswdf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwusvhpnp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmkgzuagu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghfdofkgb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gsvohyftj.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gumgiwiau.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gvgdvbxpu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/glurqjeuj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gjjmyvrjd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gducytvwn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gbiwwbtdp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gnaglnqfd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gehljfvbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gcinnvbpz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gcffhfsfj.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gltlemxvs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gjuficjip.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/glhpmbhsh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gobgsquhq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gspkogcwx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/glfqtxoaj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gsfktpxka.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gmfmuiksi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/guvnjcamh.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghqjgfpej.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gkjrzfnbm.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gajxhusxs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gqispbcij.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gitnhdqyx.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmolvywgw.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gahyoerdb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/glqhsnkfj.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gpwxwakns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gdyskpzjo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gfaxxmdmm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/ggnywctok.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gxuwlumgx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/giuavztxr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/glqtwceom.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gsjyupbsa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gmkkckmxj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gduqdhywt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grgplscwx.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gyucwbmiq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzlilmlms.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/geusfdgni.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gdixeeogl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gxzudofdh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gdaskcjsm.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gqhlkbrxp.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gehyjsjkb.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gghzipotm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gidyvoqjf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gkcoblluo.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gzxztvdsh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/garwwtgbg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gdcavqcsw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gxbkcbzdz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gyfnlfbax.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gwzdcxncn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkjhxagcx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gcxchfukd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/ghwcecasi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gtzowaool.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gkqwivocl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gqduwfmxm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/guwcyvnuq.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gcetilqik.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gogmsadpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gkngevbzu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gyhipdxbm.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gonxitggn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gzqkbneem.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gqmsgdncu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gzsfibhok.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gknbutyoj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gbgvqgrrc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gczsmicpp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gqezhfrzd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gcxpofytk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gvosmapha.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gzvqapaie.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcurrpm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gnvvzrsxn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glmxasbtb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/ggfbtguaj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gsptstjan.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gyedwsvdm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkgpjvzsp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gbwfnvtiv.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ggktmszps.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gntyrwcif.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/ghsiodzfb.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gridruffd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfqxrbfks.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/geuggqsoo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gjbbnzooj.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gmudtvlxj.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gzyhnvykb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvvphdwaj.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gkntlpdlp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymsvvgyh.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gsptoszbm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gmzzrjdfl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxfuemsdn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gqqrjmrzw.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gkcarfxlx.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/grwpbicsq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gynajbvzt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gkdjdpzrh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gyqjnygnp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gtavfdagw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gmjwwhyyj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gwiuhfpup.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gdgvyplse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gctylsjvw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gaxougbio.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gkqwtmyth.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gqvissypy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gtesrmtgy.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gvpfoadds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/grbaarfvd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gyznnjwyy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gpaayrakz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gjfjtqazl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gbkuotrms.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gbvglkqxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/guiyhcbmi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gafwrqltz.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gsayhrvqj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gljjzpxep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gntpiddgw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/goeseygzd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/goyopkxmv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gicvyxuiy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/grktfridk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gimwayald.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gtbgqdzmv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gdnfoybqg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gzbgtmwyt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gnnmeispy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gvidfuzxd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/glnpykwcj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gubxbtdzr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gjyoumwqm.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gvgazjlsv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gkizvzmvn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gaumehcal.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gncmdzygp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gohngqtdm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/goqzohuan.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gqmrntjjq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzixhpbnu.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gyiwwbxom.sHtML


<!-- 参考信息 -->