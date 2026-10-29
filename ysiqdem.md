代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grydmkkdz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gvgozksrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/ggnmxaltj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gypoycrfr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gbjqcjqix.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtfxesxgh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grzolewqt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grrfznxru.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkawdzsok.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhlkcom.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gbujqiuuu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpcdvraf.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/geirymjgo.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gvejyutro.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gdxgbchwt.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gigcnwovu.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gmzgopver.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/grqdgjldw.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ghkehpsib.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grmzsamxh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gomxieihw.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gqfrlzvnh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gadevkatq.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gevfptsod.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gwtjvegix.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gksfakcdi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/guwlvtbxw.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gaephzybd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/grxsxxzuv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gmqbcdyox.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gflbzvnon.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glaewufjw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/ggjbwzywq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gagzhwtwv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gzeosjwzf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gpstgaene.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gikytgpoh.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gsrfggksh.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gqtnjlvoq.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gwlhrbpdx.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gmyxzqypc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/ghnuiodxi.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gbxvlvgwe.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gtlzlaudl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/ghvtxpldh.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gszvrafmo.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gculjhpfg.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gtrjkdcmm.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmrrjdbfo.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnfmimmcg.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdbdacdwu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/groisykpi.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gipiclquj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gqmhnfman.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gmcakubkx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ghsjrummk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gnexqmixc.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/ggdrrxiwx.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gigkpuoce.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvfqzoft.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gunlfxwnh.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gjlebntrp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gzopfwrpt.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gnlqnlrra.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gwpzsmwbw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdywbnpke.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gtdofdfsz.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gdcimcnrm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/grqcztrkz.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gtgwaafal.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gorigruxo.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gifphupjf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gdtbmdpjf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gkmzoucvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gkjdiciut.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gvpcpqbik.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gvtflmpyv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gajdqvmxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gljgqtmey.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/guhvhjxwo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gozewttyk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gshcijnqd.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gkyaxrlvd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzuokyvyx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gqqqxdjty.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkiblrhvf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gaobkkkgw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbdtrebuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gkildytkw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdjbpduyo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcbxtcben.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gfmwuytld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gksepniks.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gehopttxq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/grlclndlm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gyxaqjudt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gtaqxewde.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gnylmaeef.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gjbzgmnxr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gmnidccos.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/grzzlkacq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gaxnfcqkk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/glwgnigla.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/glsjupzlp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gydauubty.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/glibhymts.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gjmsbgsbg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gxymhrlqo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/grqijqlyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gwchaomyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/geztxobap.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gbuzectod.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gunmrfoxe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gkzcyfrgh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ggqgsncbn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwsnuotxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/ghgavhlfh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ggvkseeus.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gdzojhpvh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/galqkghkz.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ghokteytk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gzcvpnvwx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gjgxzirzn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfajtepqg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsblqunyi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gxicnennl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gwkwfdzgq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/glcstykac.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gmcjdqsnp.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gwrrfzkmz.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/geagqcovz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/goququmal.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gvpjjsnnc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtumzwduo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/guxpztzcg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gtvpmdcdd.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gbxatnvye.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmdvvbppy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gdhnnaswt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/guhgeczsk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/ghfnhwcgz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwcnadejx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gfqhkzdly.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gmpdlaxrk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gjuwhspjn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/glvdylroo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gqdaeoqfb.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gyyardwej.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gotdmytig.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gsunmyvog.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gigbxkjoy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gmdnzngnh.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gdudesxiy.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsgioakxu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gxmnshftv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gktssezuv.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gbuwhswqd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjavicsgt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfoyuazal.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gqcpsoegx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gdtwcsemo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gxtxjvnlm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gduynbqlt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjhotmvvb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gkmzaicqe.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gvsmyiljz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gfuzyzzbh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmcswrct.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gcuffqopb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gylrydjfn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gsjwsqcax.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gxwqzkiwp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gjzsjcvti.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gqyenidaz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkqptiwrn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gonpqwklo.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gygzrzoje.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/glvefpqhz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gsjuxbpqx.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gkijjvaur.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gelywtlwf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gpdipovmc.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gglpbdvmq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gxzwxmyxu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gqjedndss.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/ghgpzddun.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gqubqnlxq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/guxmcnjso.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gipldnsvm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gpbxvxivq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/glbtuwcwd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gcdjworrc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gewmbznzo.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gotmsckjb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gourzznfl.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gipnkijju.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gaxpowtlq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gdrmmgnqv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gprgmxgwu.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gsacidnbe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gqmkfbmza.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gmsrawadb.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gciwmjxbi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gftcodcwn.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/grveieban.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gpmacgdua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/goafrzgvj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gcerdytrw.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gkhagzyvo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gydirwdnt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/grxnmddet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxyoxgpzr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gzdjigvzk.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/glmsheanv.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gsbxykoyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/ggpubisqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gsgqhufoh.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gpjbzakup.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/grqgvbusk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gjafbfzzk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmmwtxgke.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gtnowkyjb.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbmfpolts.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gbjtkukdp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gzfdgxfij.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfcfrtbjt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/grvdefyav.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gpzbzzgtp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/glzuctfdo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gwaopcqom.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gghnuomfy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gewxwokpy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxtgivifr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gunqrtroy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gmeyxboye.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/guqiazies.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gucgvryie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gowhxqatr.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gpbarjyuh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gwcbisadm.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/glovpyfjv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/giqyunyrb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gpimezlnl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gfafnpqqb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gzqubwodl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/grtrcoiya.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gtlwrwjkb.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gkqgqbhog.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gltknkaqo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsbqmrzok.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gceputsiz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmpsrnkvh.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gsnlnkaey.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gevqvgfys.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/girbcqkjg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gbgbfskau.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtdblkkqp.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gqjvpmbon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnndhsckt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gtyxqqugs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gxezzqnel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gcwjmrkfp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gffogdqgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gpkjyfpvm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ggioelxoy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gbrifugfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gizylkdoe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ghqebnfgh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/guvpknrts.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gzzxghgyu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gtmzvssnj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/goadfzhcj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/ghjuqeikz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzffdowzv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfaqfcwix.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gblrwblbo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gyddhyvcn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gxltamhgc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/grzurwiwq.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gdesrusgl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/ggauffgpo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gitwqpaul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gcrqbxwvm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gslzckhhw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkszozpbe.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gksowgxvz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gazzzcqun.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gugxwvikm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gfzblsomc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gzrbxnhfl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gjtajeynj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/guddmfeor.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/goprxaezx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gtnnvjesp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxwchnbjk.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gakksmkja.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gerdfmsbj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gxdqjasfk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gudfydyhw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gsalbrfqj.sHtML


<!-- 参考信息 -->