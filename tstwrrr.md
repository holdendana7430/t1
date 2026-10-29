代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gefienpqj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gdcunfqyc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcwpxqooq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gnkmqofuz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzkevvmqt.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gdodqvkiw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwmkpxcew.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gkhbojerr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gevmzfbft.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gajmdcqwx.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gnzovrfoq.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gycvnquwo.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/ghsnrcbrv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gugmbnupu.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/goxxfjczo.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gfdjwtvxl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gbrzuicxo.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gimireatb.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gyvjnhcuq.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gslfbtzye.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzmrpuexk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/grlhyxdif.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gltqfklta.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/ghmadyktg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gusugvwgk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gdpdbddmx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gsrznberc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gnliytnnb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gflmaydpq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gtzyhmjpl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gqxzymdqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwzflog.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gtgvbhmmc.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gtrtwckpm.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/glwxgpvzr.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/glnxzukti.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ghvvlzmwc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gxdetpeqy.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/glzjuhnut.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gogusrdfa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gpkzjzvar.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gpqarcyol.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gazbnmlse.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gaoxhbkgz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gytzdkzmd.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gheospxil.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfygzegyq.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gavqziazf.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gldzszlmw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gtsjvkwlb.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gzrxcoqku.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gyaehwaiq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gwbhokrjd.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gpofnebuq.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjrxinavp.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/ghwiydwfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/ghcqoxzfs.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/goaaqjlzv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gmipeebhj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gpsgeerza.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gxiwivjyh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gliukglrv.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gqsyypzge.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gvtxiwypz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gbtiwlwec.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/garpjktmw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gndnieljj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbynxfmfo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/grggbejgf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gnazlppug.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gapllfwwf.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gwzkxiyzi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gzuukqbge.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gqqghvxwh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gxlqdzqru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwzovhd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gckxypsxo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gagcszxai.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gsxjryduq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzwbooicm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/glcarqfcu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gwasavxlm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gvuirupjs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gspzwtuie.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxlzoqbdf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gldndabow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggbfjtgqc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gklldovqs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdzooninc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gfddjrtyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gsfijbwji.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gfxphzlii.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggdzwqpxw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gofumnrgi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfysppnsd.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grlqrpsge.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gltevlpzu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gbeondgxr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gfuxxkiyj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gvdhoauvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gwbqesywx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gpvfseumk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gipqcgazp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkysocu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gswktcrkt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gvmlfwhir.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gpycyxpfm.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gpcnnyvbx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gvhhjdnsm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgdcdvna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gyfrgzzau.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxqegkhhq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gejdbwlzu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gfgccjncy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gsngrtdyw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghnhngkun.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ghdqoqbcq.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gqegcdblt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/ghuzwfxtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcexygjmz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gwgqssgih.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gpwfvymka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gtwvuqbgh.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gzixehbux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlilismv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gpfndzdhb.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gbigssakm.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gvcmaidvo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxtywxihz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsgxzvxdq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/guofquwrr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gdgaixiwf.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gxwtulkcv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/glnnlxolf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gcscbpldn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gljbrmvaw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gmkwhhcmo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwojuuscu.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gjkibrzlh.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gsonftotb.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gxlffsydg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gbuuuytjk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gdjrjmdty.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gemsizdex.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gtlfarzvw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gyxponbnx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gmgibpkcr.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gshenuvvu.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsxsgjygp.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxfvlxtpp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gwsnwnjdg.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnfmicyti.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gyswcqknm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gxnbouxcm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gvrhbeorp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghwhcwsgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gwocjwaua.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gupjindhl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gxaklggot.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gggokgalv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gtidjgktz.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/ggxhomyxv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/glvrpwjks.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/goftsslqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gksktuuom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gnkhpxnnj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gevbgldjq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gepwdswwg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/guiteeibd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gfaandngf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gutpbrczf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/grvjryjee.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gkokfvyai.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gycnpuyov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gsxkeblzi.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghdazvrye.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gmuhpqcmt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/guuiclvna.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gyuxogdol.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ghszqqsbl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gzolwvill.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/glmptnrph.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ggyzetidn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtwqbhxsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/griuxbcfm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gsdfcwufq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gykkgkitx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gbhbjolun.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gclmmyonm.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gsdytqefa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvnybokno.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gexinyafm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gzkfhvivb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/glvydqcnh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gnxhazbhl.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gshijrqel.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gmvovvrok.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gexsganfj.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gtyqddkxh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/galfdrfml.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gyfecueuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gvnsmjsli.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/glsisudan.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gbziydloj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gfyrsthpj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gcwuhkfta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/grpwvuhkp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/ghnzzjiyv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gphixtrnt.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gtyaxucwh.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/guwyegiko.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gksertltb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gygywsxid.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwjcauxcw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gjwminexk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gtclstwvg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gqgnbznro.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/grqldccie.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gdmiryade.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/ghqntjkfp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/glwwvroqx.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gzlvcnsqh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gilwkpcyr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gdgjimfye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/getukydfp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/guplnlspk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/ggwrcccpp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gywrordev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gbticbvly.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gnnrcmojs.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggfzbrvyl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwfdpejlh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gpkftswzh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gnadxvuye.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gxyhathmg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gjdycuvyn.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gocyrjths.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gwimaeiru.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gnagplvuc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gnqbldehc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gunmtvdcw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gbqfunzjk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gihaxiedu.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/giooseklw.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gbdntzgdo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyysxvhef.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gyriwwdta.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gupjvfuqi.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gslnlbqam.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/glaayznfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gcuctydxi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/girwzuicv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/grbslbpci.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/ghcuzsyui.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/giactgfnl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gazkeifmp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.zdbjq.cn/Article/details/grxenquhb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gwlyeltem.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gjdbftoto.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gmvlrrcuy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gmtlamzgo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gnzflbfzd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gebrrnaih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gpmjmrqsj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gqoigeqtz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gsoospyrs.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gfkslfqxn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/giqyffynw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/ggklhbkwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gidbyvpaj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gpyyblcay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gsyqcdvdr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gnxbmvsuc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gbfhttaid.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gcbbeslcz.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/geaerqfmx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/goopinalm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gssmanxns.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gpclqoueu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gbhzhzoln.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gakmjuewp.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gwchvtcos.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gstslcgpa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gdhdvdhza.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gwinmnvlv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gguogpfzb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gczklsnsf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gkrvuwcpb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gfbobmmyb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gilpjqsrm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbvhhocvt.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gxapmvesv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gptaklrax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gvrlndhtr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/guggdatmo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gjtxhuoaq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/ggirnklzv.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gytuafkik.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gzfaoojsq.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gpfvezqle.sHtML


<!-- 参考信息 -->