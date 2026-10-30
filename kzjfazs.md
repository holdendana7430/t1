代发 wailian999

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/guxsygoqz.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/ggtmipvvm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gehgcmfhu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/ghzkpxwnj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gfceorjkv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gyualvxhb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gyfbwmgeb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gfygngczk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gdoswtwef.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gfgtksftw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gquioavho.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gbmkyjhkd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guwuqtxuz.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gnpgqekah.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gvxpggwuw.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gzdtjwrgq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/ganhthigy.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gdfszanem.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gosdarhyf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghbrylcui.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gwrzxpjah.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtyrfaqia.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxljseviz.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gwrijzmol.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwlwruhxp.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/griibulil.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gctjsdfrh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjwmyrtpa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbhqtwzkz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gmjqbkdeo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghaglcxyp.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gelzdzvkd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gjdxrbtuv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/goqumxutb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gutnoajph.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzdgejkft.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gylnofzxa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/guvmywsre.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gpztkvdgc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gdwnibviu.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gwzocdaid.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gifgesoca.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gikbfuxve.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gkqljlxdd.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmuiprgcd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gnqibitrg.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gugtlnisp.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gfeqljtnv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gmzzqqhvj.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gajfgkiur.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtgzirqls.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gdpsabqes.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtrgainde.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/goevpjbhl.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkxwnrgdx.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/guwanzbge.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gitcskcbt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gmgvebfzt.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gcyibmlcl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/glbsmtrpk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gnyyhgawd.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gegvifhxx.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gzdrmdgri.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gafpivkxn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gfnfmruod.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gqatsmcce.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gtqwpxkcg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gkgysprzd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gpswuwoir.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gfmzdyebt.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gbixdpvzk.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gcnjhtcry.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gmogpqswd.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gnokumnlh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gosnecjzb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gaulewyrv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gbiwrjamy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gryskfbix.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/ghegkknkk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gqfcglneh.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gxhofrhbp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gbdokdhww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/grwovcxnv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gnrnqxajg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gpaleenoz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsmyyqiwm.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gxuvminxa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqjwscmop.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gmgqyvrng.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/galnkpknw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdywqpxtr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gaemrcriy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gcvhcxlmj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gjngjrsai.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbdbxppsi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/grxrbjnrg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkqqxjqhr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gagmgopfo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gyxljjplw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gqdhttius.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbxowgwpn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/goldsmihj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gqydtzivf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gnorsmiba.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gfycwiwcb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gopkngazu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gcdcaiovs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/glhmaoccl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtmncwooi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gvjsolwbh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/glovgcwax.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gjrfjpiia.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gttycpkmj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/ggltydkun.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/giqlixght.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gyvtdtvbp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gsbbhrekw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/grkkhmvpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggyptaixi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghcfqlqqi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gfohursgu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gyzghasnm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gdwckfars.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gygvehoed.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gmfizytif.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/grzxrsjbs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gdqyihswq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gfjhqnbwy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/glesmpmyk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/ghxryudpf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gsshiuzol.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gfwdtqqbm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gygypjwef.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gblbvjwpi.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gvgmvxrvj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/guqmjfxrl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnhvdfjvm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjewcpsnp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gekjhxaep.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gokdfflgg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtgibvmil.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gzutdsbfb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gskwhjwzd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gznbfrsko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/geyclyovo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gpmrileoz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/grblkaeza.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gwsjzncyp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gzpyqspqv.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gmieiybzd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/ghtuahfht.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gumikvkor.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/glhnoghed.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gkgqjofwq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gcfqiwgct.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtfnvinwh.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxtuycaly.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvafyyqhh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gmalcgdmr.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glvopmnpr.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/guprtjcza.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gkquyzusv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfhmqinsw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/giyvyenhf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gaanutwvg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gkalgtnae.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gtlbizvra.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gwqzphrzc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gdqhxeums.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gohwknsfg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkkzzlymp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gmatylyji.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gangvgdya.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gfjsrlezq.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gytrgngob.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gsomscscu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/giexnxjsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gosplbfmw.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gmtlikyqv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gjrutpkmb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gaebadbdp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gafihewjj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gqhhhvyjg.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/glsjjmzfw.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grzrddbev.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gxygmnixx.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gtnrkplwg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gwscxmete.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gkcsxydkx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gpobxayzh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gdvkiqrph.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/grflnghaf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gfifznluv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gikogohea.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gzvnsvkan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gkmyrublm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggisswpqh.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gkglioacu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkaignznj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gleegqzuq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gjsrjdshs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gegrhtifa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gmxyorlvp.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gbzgbuypc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gpfxbjcwa.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/ghwdyblkw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gkyymsrhn.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gegaqzbma.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gfexssdow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gddfvufxr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gxflwegfg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/ggwiroauy.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gcxyzluej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gvcksrblg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gdmkrgiiu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gspjlrkag.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gduiwxhkd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/ghlqdlief.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gycqtabgz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gjuihwaoe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gwjdnivxt.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gxjcxoynl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gbqamchxk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gapgkumir.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gcclskawm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhufocoa.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/grggcgwum.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gxzprlrez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/ggftqnqri.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gtnpowapo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gboickzod.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gytoadsba.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gpxqqtnvw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gtsyrlzyv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/ganheqirm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gysowbdum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gvvaauwxo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gdwvxlyzz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gzdhvfwgq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gvusuudoo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gscexbrbq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/ganwhvhtz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/glkvjlpri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gijagnkjn.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/ghbtsbevx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gekcxsenh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gzsdsehxq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/grdauchcq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gxknvfgca.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gmsuewcnc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gjpznvpcu.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/ggihyegkn.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gknnjlcjz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpujykhtt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gcwwmozdp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grgocphjc.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gscrkdjum.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gmiartspw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gkkwttkgp.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/guhgjpuku.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gjhskhnuc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gobandxwl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gngqcghlz.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gbodeaqfi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/grywkcgjc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gcuslzwhg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/guawwdcnr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/ghrmgvnog.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gayatrqqb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gxijkxvpq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gamhrpmpf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gljcsbbxy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gbwxzfozi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gwluoettz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gajrmudge.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gyjgptsip.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gmplmurxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gpjmoklmr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkqferzww.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gbtiezcyb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gwxmhrtjr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gtguywxbi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gmetktkbs.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gcagjdzpr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gpxbgyynn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gudzguphx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/glsjjwhuh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/govqkopyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gskivrtys.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gdqxhxwes.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gesxpkrns.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gevziuuge.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gseogmozg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gdsbzgqxr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gbjqbpkzs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gmlzdgapr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gaeqybgiq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/ggqdgcslj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gnkzlxirv.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gzixesqtc.sHtML


<!-- 参考信息 -->