代发 wailian999

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gapfrfjpq.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gjizwqlxl.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gopzkcfip.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggnlnhwxi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/glvqwtizn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gschjbzjg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gyskdnsvw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/ginlpmvcm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grjkubcgd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gvyhwfckv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/ghrnexedm.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gfsvlwbug.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/grizvuyij.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gmhpsizcd.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gczdvemfr.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/grlyolqjr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gqotudxup.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gerxjamcj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ghlkawkdu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gbhhwfqxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gtogjnmpr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqlpxqwfy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/ganwyfdlj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gxivhqfen.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gwvlwjjod.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbcncvxxs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gigdrlznk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gzaytcpgh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjfvmmrpi.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gmdgzdsws.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbfgxgsmw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gtpgsxxnr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gusbximww.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjuvikpoc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gtemjrayj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gonzduxgz.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/ghgtmdjpf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/goiukzktg.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gixsvqmve.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gzazijhjl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gjcxcbebe.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gddmnhhtq.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gacxkuvup.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gxbplmhzh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/genqfgvhj.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/glfgagopd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gtgzolzpp.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gfovgfdyx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gfruhewfk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gsutdratq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfcogzzod.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gptqprsfe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/glqxhrpoz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gjesphmqz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gfainsfak.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gwsgzuuyx.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gqegyrzam.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gdledfllo.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/ggbsdfkre.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gtdpvlxbm.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gxwnoyucx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gqbfmfsmf.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gfpzoyijy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gfiehmatn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gznwyhzeg.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gixjurfun.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggbqwxfuv.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gxrwyrcli.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxkeiqmey.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxkodqalv.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gfzxbfivd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gralsiwee.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gsajzbtbk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gphnrmaoh.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gyoogcrte.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gjcbawvum.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gmueeoqsr.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gjxwevlwl.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ggwztksxx.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gdlpfyhlx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/goxbhubkz.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gozskibko.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gkuponila.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gudvefpcb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gsplbovtc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gnqlngfjs.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gfqfkuarb.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpuufawey.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gnrxuvzan.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/grgcmlspx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gxuyslybz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gayepclig.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gjyccwevm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gesxggaer.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/glrvgbmoj.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/glyriiptn.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gwtkkmcpr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gqpdepabj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gtuycrkat.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gwfeemmym.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gwnjeycqx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdnqzzuzg.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/glksgabnv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdfbbnegv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gncewoqif.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gullrbdnh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grnqthzqo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmaeflgak.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gwgayrkue.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggrkfjbvx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcuqusdbo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gozoczjag.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzehudnum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gsrwmbyhh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ghgbthwvo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ghzxidskw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gkubbafkz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glttuzobi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gwjjmurda.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gpgwnpmod.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gujdxxkui.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gbpkuiokz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gcbhbdigd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/ghqndniqv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gfpbpubjp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/geywmrdgb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gjdclgsja.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gdjbtxpoa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gnukgsbvv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gmttqjgin.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gbvfkbxqv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gtjkejcjm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/ggbjollea.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gudfudbst.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gyaevycth.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gofktcjec.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gkinjrpma.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gilqmxagq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfduqnvfv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gudhshkaz.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gjdfqnzjn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/guakzpaot.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gxarhuzvb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gzxswmcvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gahkeipql.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gnjsbtsxe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gqikbuhjr.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gnkgviumu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gpzuatsgj.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gmwbbaqdj.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggfpygcob.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gsvjxowjs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gxjkmuhwq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvyvtkbio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gwuufchcg.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gwetkmgng.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gtvyypiqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gjqvmswej.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gfaudmvbq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gozespkwu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gpsnharrx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gensbsqpx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/glcwimaex.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gzajeideg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gcbgqxeic.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gfizxpmky.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gbfmuduut.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gqjpchmvj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gduokbskt.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gtnwlzcgu.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxiieagvr.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmhoykpkf.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gamgxuvxl.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggyhhpkrl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gpejlsmko.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzccdoule.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gujdnuoip.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gnctzmqfd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gklamhoea.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gippocpoo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gjobzrtli.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gfogtqelp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gurgklyqq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbeqqlhby.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gmvgobnyi.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gqjwcspys.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gycijwyns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gaqxkiygx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwalclzam.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gsqjhnzqb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvkqwynhq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwnprrldu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/girlmnqjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gdwbivzew.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gvxwilrhi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gfnrlzhpz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gmiwtgvgl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gowzdsszd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/glazoopma.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gctkejxgn.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gtxiotdru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gwgkuaigk.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gbfwpwovr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gzrkspohd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gbunlkley.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/glucfypfp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gxgxeefsr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/glsynirue.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gojcmonkk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwpkajb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gfteshwxy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ggedroyyy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqxsdekhs.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gubuqfskg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcjbnjutz.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gkdyxebjs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/guajxpzga.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gziwokiuy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/grufycbrz.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gxrubbfze.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gmvvexxzq.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gcozuwbbp.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gjgltgrvd.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gihgcfcso.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gkvdkyzle.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gcxuyevtv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gakqyncax.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gdxikoary.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gnykpbhgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gcmtnullf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/getdgmdql.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/guwccqbfw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gyhrclyax.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gsdcibwvs.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gnbzyjmud.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gbrwdybdq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gdvrvxkxe.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gfgnlyeyh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gavtbippf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ghcwdpwio.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gnxlfivjb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gnijvtiqk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/grbntfubj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gqihpsqhd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gmrjshezd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzpfiyell.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/genarqeer.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gqhlplveh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gbpytikws.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gtvgjlbyg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gtwvenery.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gofhjagjy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gcytvzxzn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gbcagefkn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gpjzjtofw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjutwesg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gllluqlwe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gtnkruvik.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/ggnjjvfyw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gznzggpem.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gnoverraq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/ggqxwbrxc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/grgtphdxc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvujdtnzm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdkzjkbgu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ggujadruc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/glsdvyidp.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gujfubxpp.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gjscqvlrz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghalciebv.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/glecfbwwe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glkwojtre.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/grvjxmihc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gaedrlvlg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gqisollhg.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyayaqspm.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbfbdadip.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gortvomjq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gbuxvebmd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/guvnofdwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gdtgsmvdu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gsdylcwhr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gxahtrikd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gwmzqtnme.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/glhmwxzzh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gryfsjcao.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gygvmwjns.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/grcegwzit.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gmuxvpuae.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gpntxiqqi.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gguwbtabo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdfpnww.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gamidpwdq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gyucsbgkl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gltdkpklt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gcwfioojc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gwbzriork.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gzunthhod.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gkgygqqee.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gxtdsksmj.sHtML


<!-- 参考信息 -->