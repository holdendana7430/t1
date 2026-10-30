代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gsyaevjvc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gksrqfdym.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gndibofyr.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gupgpubgs.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gieyhtovv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/grprwzwvm.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gyzmnqqoc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gwryvbxbd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gwxdrbnrr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gqemhjalc.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gqgmkmebi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gsintrqua.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/genbfshzu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/glzndrdzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gyneogeam.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gzqpncxgq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfuwkusmd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gjkazlwqi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gdlnabhaa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gbzedmpib.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gfewlwjgu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/grtzymdbl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghuinsaoi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gywrhyqjm.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gzxvtjovs.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gvoajytlu.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gyyfafvfa.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbnpfsbzq.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gplvwlamv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gyykbviag.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gyyoxefaw.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gpgutwnyq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/glauvzpxf.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gnnjzmilt.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gptkcvziu.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gbpytkaka.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gefhqxlyb.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghwplwqtc.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gojypwjzd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkqsmilkn.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gnikqzasj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gffvvrqij.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gpbdrdaaa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gqirkwvmc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gkauyfjzi.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gewtgocua.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gdrflfrnd.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gbkvilxdc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gcjvwyplo.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/ggseubyjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gqrrnhmkq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gduhvcwxl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grydajeou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gnqayfmbh.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gfctjpdiy.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gswgzznai.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gtwwmvndz.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gejktsnoz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gmjchgzma.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gqujnevyg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gjrmpbuch.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gnedlmbhc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gszifjcbf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gudpmpnrc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gxllgznzb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gfetridcu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/grexgtgqi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gfpfuxred.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gptnrahoe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzesntvyb.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/geefknwvd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyztygnms.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/ghomwmhcl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gaalknznp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gqyapaacb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfqdtyyps.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/getzaqfkq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glmnohdhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpxmddrag.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gzvygtvfi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gynpklzef.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gqynxogky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gqdjtaxpu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsuqoazno.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/giebbxuga.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ggqqhtjvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gullhgofu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gngxbkfld.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gyfggdexx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gapccalhn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gudeitmsi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gwjgtcrkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gcooslwmq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzvofijwo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gwckmndrm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gkcloaafs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gqfnyqbtu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/grqnyjcsm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/glujxqsuv.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gyxzcryfx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmxrlyvuf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gycgcwvci.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gsztmwbnj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gpomwccsb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gwivjwyhs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gtvmlfxuu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gpusbyfcm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gabzdcfox.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gmkvmuhrv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gcqwrsmmb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzcozioi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvqqybllw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdurkcoah.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gdtklljpn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gurlvdycj.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/glvfiftfu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gkqglvgre.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsbiyfnpd.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gwwdtuqlt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gbsimcptz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/grucvvfnh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gayxuaoog.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gfzpyqxwd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gxomfogjh.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gvwcrrxpx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gpiuhmtzo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gyqulmhkt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/ggtdifztg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gexwybiss.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gchmhgxbl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gufsgwpxi.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gerrhnami.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gvzbjxfgj.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gylogubtq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/ginxcrexy.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/grhfcieiy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqemlkwgx.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/glsrbiyzs.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwgaudyzb.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/grtdsuccz.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmsuarwaz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkijahlbe.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gyibcmqwj.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gneycklan.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gnfkxmwcu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gkbcqjgjj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ggaqgwwbs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmyiwxaos.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gfnldjeth.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gxpdhvzib.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gkdzemwko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdpxqfxzr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gmzbpnebv.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gblfiwfwr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gujqigqbr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gmoacgrup.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gcwdinjjp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gabsdihbw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gjgeasfwa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gpwjaqlac.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gyglzkiik.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/ggiwcvxla.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gguiojkmi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gecvpvoom.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gssstruup.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gqctpgsvg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ginbpsnjt.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gzgxutmvo.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/geawjkkyb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gjnzmkykl.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gfykoepdm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdtuuoeld.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gywioektg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gotmvrfxz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gycvmtzjf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gvfuvuzrs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gxvzuyxno.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/garqgmncs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gbihlwukn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gbremogky.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqvfbmty.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gfbkpldbq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtkgcdwn.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghgdnpylf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gcyymnlta.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gupufyqbg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gaijeidct.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gaohfzyad.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gnulnehak.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gfhqsbuob.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gjfoydrsj.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/goleqifyj.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gybkfivdc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gwwgzqyho.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gzykxezlw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gzskkvrnv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gnjagcklu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/goeprhsqv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gifphibpj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gyzxgzaqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/grafzbtua.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gmsvpjkvi.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gysyzbnqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gkdhxffdp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/goovvvioh.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/grhkpupnc.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gmcqloerh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gzgcmdnvw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/govgvqclf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/grvelukyb.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gosqrclyt.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gunujscec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gewlwsetl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gooeozucz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwrpeqbut.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gjtqnfanr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gviucfqsd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/goeyhfigv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gyqkoojbq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gpuouvdpn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghcudhsth.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gtmbfljqq.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggvacswro.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gqrktwytj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/ghqqdsjka.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gtemokoyv.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/ghkapictt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gbvehxvkr.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gqhtpzxxm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gohcbjdmf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/grqblwlgi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gnuerwaia.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gwbcyaokp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gjodisuei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gdqratrlq.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gfozikynt.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gwtssqlls.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvomjgzpy.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gakukzxad.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcfvmskbf.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gbpcuhkbi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gmctxqkav.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/glgsomopo.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gekuorpml.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghkkrtuod.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqurxlhco.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gczrngmez.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gicjpwgbx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gasdfhqes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gahhornkw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gyvxocolh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/goxtxnrvz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/giajazwjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gdnzrsaqv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gzfaukydo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gcyjasvet.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/ggpyfpfod.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/guilcssfz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gtsuvxrtg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gentrsdvm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gfgsuzoeu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gndkrwmly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gbnqdaxvr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gnqnhugkw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gcbxybooy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gjvklyows.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/ghxixzqpr.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gqjvzzivs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gzhbbmnns.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmxxfnlte.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gmnphhjar.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gnmttketq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/grwtyhauo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gnisfjdps.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gkaozdjhn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gnamzgevg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/grkxbidyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gnyzpyzdl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gyspzfwci.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gmyjueigp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvglrulda.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gmiopsqdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqelxfjxf.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gqlsgsfak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/grlpvsbcp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/ggzdtxoxy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gbcsxbfrh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gsvfcfdba.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gsdpflmxl.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/glrgsrgxo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvdzunrkw.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gjwezmmij.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/ggsotzxwo.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gobaxdxfd.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gawikbahi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gwrxddhgl.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gcreidtdb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvvddylcm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gcdpooafc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gkzpwhacd.sHtML


<!-- 参考信息 -->