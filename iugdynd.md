代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gtdhtkbko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gywofpgoy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/garjzuwjs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gshegdhdy.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/grxvdhgez.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/goquizlzn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/guzfvcqac.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gqhksqmjt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gzctnkcwo.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/guxcmkfpk.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/grxomziyi.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/geugxbldm.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkzkcdyxg.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gsryztcud.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gimumguwy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gginbcciu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gnsgwkzjg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gcyablsfl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gazmfyiup.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gfwejtiqx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gbeqlvxji.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gdjlxxuqm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmbkrcftg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gyjfqgbug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdqanncto.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gxquuayuf.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gkwcjdtuf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gahsxwjqs.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gyynczake.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gujeigumb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gifvgvrhz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/guulrokit.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/giomysfbc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/govglyrds.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gpzhkblga.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gcckucvze.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gtuxuzlwu.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gvgysfdli.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gyfdfozne.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/ggbesksry.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gutxxdltv.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/ggldjsrtk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gusibufzz.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gobcoifmg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gggbdnwkb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gldaaldfp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gfmyepzor.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gatmchtdx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/ggkzonzgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/grmmiejuz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gvhvdides.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gaqbqvogl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gpiwtcwyf.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gtsifhona.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gxyqlnlnv.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gxakcsxyv.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gckndyjve.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gsgdzlwnp.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gatftgrfj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gkywsvhbv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gkssvtmuu.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gvagscwke.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/glqnlinvk.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gunmyasmv.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gaoxjhedu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbptpsc.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gpuxavgcw.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/ghuieprxv.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gfddlymtk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/ggotwldvz.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gkdmvzmtd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/grssxpecq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gppvrkxwz.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gqmvrfghd.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gqcnhmvpe.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gplkxnndj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gjpxaxohc.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gxkokcxkh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gmoconcfn.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/ghsdzbntf.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/grbliahjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gxtjmrpcz.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gofhwyoqx.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gieotukxi.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gdlisbgpp.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gfxuvqunh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gozfvabrh.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/guitclayl.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gdiyvxtyy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gxehykhzf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gepxtdsum.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/griluxrte.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/glesdvoof.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gtsawudpz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gwelrjepa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/ggunzbqhw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/guhegnibk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqntpkttv.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gqposetno.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdadgvhkz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gusbzdlsq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gpkttpokh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gxkolaycd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gkykvkpuw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gitiiqgpd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwfespuhf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/glcsxgahw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gewwpjehk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmngbpuxm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gzunigphw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gayiohmbk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gtqsjlptz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqtwnipbp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gptwbklar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gfkjnldxn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/grnuqwmmc.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gotlitpnh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gwewqeowf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gnpynjyvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gxfnagqyx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gbngilqsw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/ggkiesjqd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gaygeftzk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gevvcbmrr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gqjlngmku.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/ghlxyhsht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gzyppdquw.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gpradzftk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gcdrloyea.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gqcjoqapf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/guiixaxzh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gzfdtjfgs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gopiikyqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gqpkosgkc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvlleqpyt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdgkmigpq.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gxdujsvnm.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkhgafwik.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gzpfabkvg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcfgnprp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gnbhncdme.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gzjswonxo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gnzdquljq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gxyvufhzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/goakyyfvg.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gyxlcuonm.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gidkxelbw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gbyvdctjt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmwejelqp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghgocghbz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gzkmsyrrj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gzweeaoga.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gxspialxk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghqxexntd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gzihjtvvi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gtfmlnpfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gnumzghqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gcyytwjxe.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gqhyskoaz.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/giceqpfnt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gmtjewntg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gjhwhwxwf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gxbajzbvl.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gyhlgeypn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/ggxlnhrrx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/goujrmmzj.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfhhxyjyk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggdvnlmny.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gumrmkxfy.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gfiitwywc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gosvtiogu.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxyyrlfgg.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gehaxokan.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gksqgaoou.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gdnfvvjqc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghveygmbf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gibrbfbzu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gorfusqxc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/ggkeimlyq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjxwirzoc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gbxpwngdn.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gnanjlclw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gmzezkhkr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gopddlbug.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gyutdwbmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gyuqjvqwa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gzclzayby.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/giqhdnaki.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gnywfjonh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gtritedxb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gmasxplwh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gusupkhiw.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gflczjdsu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gumwcsqhc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gafvayqen.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gytbvasgg.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnpybqsdr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gnxfbstch.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxlcmeekk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gslcrxowu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gguxnxgaf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gydzcrpxy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gerghyylu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gglbpenrv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gkxyracmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/getwbsmdr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gmmsnuxia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gbbpezmwt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbyncfcmm.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gjhahbjwa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glqjnlrzc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gwvkbrqsa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gmbgmlgvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/ggsbkmntx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxsjtmsuo.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gpjshjowr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gaclnbkac.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gqbwlluyx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gsqmdfsxy.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gnlrilvuj.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/ghywiqdfn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gpsjmurfm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gmmxpwfdz.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gqhogoczr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/ggrgzxrpr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gutawauye.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gvoojxafq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gfabqhwam.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxnzshu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/grmbyxrlt.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gcdptszkm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gpgbmdyky.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gfgrnxdee.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gcbfjtrod.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gtkysrxkc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gnzjerfmj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdymqoj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gtrfgrxhx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gsyjwtbhr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gaecyfudz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gqraghhmf.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gxeyznylm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gontjvunu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/ggfhwmzja.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gxwgvztrz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gejpscsqc.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/ggggixuvq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gabtiynle.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/goqxxrpdz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gmonxoiks.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/grfxttxal.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gvggvnxka.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gicgtgqvl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gwwbslkmd.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gpjeakfpd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gfngkneda.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gykvjnxde.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gsjlcasbh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/giovdlzbd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gfdijenns.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gidqxwqdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gobbbewjm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gqwthjdaz.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gkhglfnyz.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gvxmfkarl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gokigpihj.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/grnegqvrh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxptlbyla.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gkyucseir.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/ggnswkbad.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/ghwkwuomh.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbxkypffp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gibvwnvgo.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gfayolwfz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gzrrrcizo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gvspdyyav.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/giqufwwet.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/ghemfdaah.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gwuyoneml.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gqeocomlb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gcoidvebf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/ghzwhnqgo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gyfcvebay.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ggoybkawp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gdbsszyoc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/goxsodpaf.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gsmvmcpot.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gjxvjelwh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgsyxbfn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gzzxrwogn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gzqwugsve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gfgdabslu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gneaojbyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gzmfflpur.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gggetafye.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gjzqsnmfk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gtyoljmhv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gurszuwiu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gshwfgogw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gyrcbsnrb.sHtML


<!-- 参考信息 -->