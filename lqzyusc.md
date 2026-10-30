代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gkuzbiqdx.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/giyvbosrx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gltxmjpuu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gwgsrumkd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gmqgkpdap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gqctjfimm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gjwewfcbh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gtwkwkvts.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gtyjltefs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gmcabyxju.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyxvptmvf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gtcbfqjsh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjhplbfgf.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/grawzcqnr.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gmhlqjejl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gwnapafpv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/goudfwhzy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gpywwfrvr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gzfryempe.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gjsnnzuif.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gssierlmc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gkieleoay.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/ggrrmbpyp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glczykddf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gylxscmbs.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdczjbjmf.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/giyifmcha.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzngrladt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gqogjfibp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gcnkwjuiv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gwzakotsu.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gufkqyjkg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gqpbpnvrv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gujfhmudx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/glwhfozov.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gwmvtqvpf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gmnqjkwvq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gvcgcvhwh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gvwheykbk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gqzisfizk.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gcgzprivx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gxmrgfcgw.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gmsjtbmib.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gdejfrxty.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/guijplmwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gavqsssaz.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gtbjomqlb.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/glkvqrbfv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/geaqowsax.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gxksgvwrc.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gvnmxtdki.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gbtinsyht.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxbrxjlaj.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcbuuslrz.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grmghnltg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gbpshsgou.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gumrxyufi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/glvkfjxxt.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gcmjwxuky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goukkuukp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gikvpqhuq.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gpeymvkup.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbsjvhlsy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfakpmu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gtfyjbhtk.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gobohamia.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gztmrcnal.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gvfsdgvoh.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/goblndotu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gahtspejd.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gjstxrrxr.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gecvlirmv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gyrtwnxhg.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gfagrmimm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gouxxqppc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gjzrvpecu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gmvtqfzew.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gitudyezy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gmvzjlckh.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gslxmpfeh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqavezuqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ggaamkscl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/glxwqvzaf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gtqekkcrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjzmnsubw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnjyvwxxl.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gcwdhychj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcxrrovxj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gaddotasb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsjfjuxdc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/getjrsetz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gsgpxzhma.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gafalqaxw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcjcrteub.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghkdqnbzx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfylwygx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmvncrpae.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gzbwjusbi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gefogvllo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gdwwkryyh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/ggtdjoiad.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gxfzvirwn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gmqnovqor.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjhbmhctl.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glexdrdkk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gtcmfrgen.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gzyvoxsen.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gdfokhezo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gcevtcjuh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gkgccirkb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/ggxxbhbuf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/givjiudbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gebchvoyq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gwhmsmplq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gkerajcxf.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gueagsauy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gsqmomvpo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzudcldix.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gptopquab.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbplfbasz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ghcehegpz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gjrezoioi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gjbymqmlo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpgavtkrs.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gvyvgvamu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gmdboyrqx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gvgkleukc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gzdajnyxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gppohesmj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gtyynbaja.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gebzksfgi.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gnvbbujac.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gfazylved.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gylnfvqnw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gugrdqnoe.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvycqevjb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzwhewnbo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gjteazvjm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gdxxscxur.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gyuktqwla.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/guivpfhyh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gugpbjrpw.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gpsuunhjz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gsdexalfh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/glkmiwzyo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gugbxfazh.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gsazubhem.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gmvkladzs.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/goyrzpnds.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gpjznnyuy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/grajlnzvc.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gdedtfinb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfxrjduty.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gaduichzq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzdrufvej.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gmvtzradc.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gqmnqwjad.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gekjkobdr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gonjpvfum.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gboscdmco.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gjsprfuem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gxqaatghf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gzyeizmdz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gltapwgge.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gjndntjip.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gvwqyfqyk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gnsankqas.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggbmrogqe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdcqexrmk.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gstsozibq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gefeaenot.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gzkezhdvz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/glkeqgabi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/grkmlpcju.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gqrstfuud.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmzgwafhk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gpcbkgcxc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gslmznzar.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gmtsagafd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gmxzsgjhk.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gkuwkayob.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtqxdqobq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gxwipsuzz.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/grexyiyny.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnvlopoba.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/guncrnebd.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gmiiupzpg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtijbkkps.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gnohfpbex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/ghtyxvpgo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gosiqzxkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gakhovumu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gojlescto.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gvahjhxnh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gtolrzpvo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gzfncvadc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxwuxqyit.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/grxylxhjg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghhvkcssj.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gubncmfgx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gqqigggyv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gyprcewkq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gcnakzcth.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/glkcrxvvd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gkhuvllpu.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gpwmjlish.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gorxapzss.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gffzirgme.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gndtaevat.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gcpqwnths.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gpcajgaer.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gibvmioqm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqqtxoqha.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/glcecujrj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/ghuyxzvpr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/glpuqsjma.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/ghcsalkyf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/glmfdplbg.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gijkrvmcj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/geozqgnqu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gznyuehsx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gfuaxmfku.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gippwnopr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ggocumjbp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gwxhseysa.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/giriifihg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/ganzdqgig.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gzhkbisqw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gkxktquru.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwvfvwzmk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gkplhsrvh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gcenknopf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gjjuzvjzp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gbdapbpfx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gesatgrss.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gxepjvxun.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gszpezuxc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gtjswocns.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gyrcsoqqq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gzakdmmdg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gnommimye.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/glbrjfwxn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gtyyfzifb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gngisftii.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gzuhdahlc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gwmdtoqop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gdupmcpzu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gmstgemuw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gthroluez.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gkumswekd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gheooishn.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gkhcesmsl.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/goobyewew.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcqttsbzk.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gnggytviz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtlxgtenp.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gkpfepvek.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/geqxjsnuf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxvwxawfp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/girnordql.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gstvevxkw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gongefmnn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gxigbkaec.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gybkwnxqd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gizvcpkno.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gftyszbop.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gyhfelkqx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ghamcaako.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/grvydvpfb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gfndconxd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghcbfpzpp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gruuwddnz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gnlxwveum.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/grytwmmok.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/glhrxomko.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gprjrimpa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/ghtcxsghk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/girwbfqlk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ggzaudgni.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gzfgrjpih.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gfwevlrqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gprggdmjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gdlozogsw.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gcejsziaj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gnjqbnanj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmqknmstf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gxvbwmkby.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gxekurgxz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gfvqoqboz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/ghhyxddsy.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gvdwzqbjs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gmzwzrcaw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gmekuczqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gvgmwxnxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gpfdgmfqx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gwhecsxul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gdwaeclkq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/givyojyxq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/grdhwnxxp.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gnrgabfvb.sHtML


<!-- 参考信息 -->