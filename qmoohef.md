代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsfzmnemv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gggdcneei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/glaqtczre.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gceymruvp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/geyqhxzyh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gtbrchpoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/galxuvrkf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gomdodope.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gnjlqyica.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gbozllnma.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqpkspgev.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gxuairdsh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gfrxzmyai.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gentxtjuw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gwxzngluz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gmagjfhjf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/graqwltpb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdlgsbtnp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gsdfvgbvn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gqcnnbyir.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gssvmqedg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gdnrtupon.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfxnviwkt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grhrbmbrp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grveztdib.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gflegbhxh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gglozufyq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gemrdnzlv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gfpbivenw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrgynhkn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ggsgwetge.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gesgydopg.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gphrtpjxk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gtpumgiuq.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gfbxxqkgb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/garbfmbpb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gpvkwxpnv.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gfmsmstih.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gsqdhjnxc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gcqbwpojn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtkhgqrmd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gpdjxhmfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gyrvgvelf.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gdnxqpsic.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gilnqwegq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gnrtpvxsq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gsyxcghvb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ghxbhrvtx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gedjxvkfu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gvbvduhxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/glvqkeufl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gmyzgllay.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gughrucjy.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gyvcwyqcb.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gggduqhlu.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqbcdaxmu.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbchwvsww.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gzjetcafs.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gtrhxqtpr.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gyuafduwu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gcizjlxjd.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gsjyzqgui.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkmpreydv.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gpdlehqqj.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gezadhwsk.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbpsckitg.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gunihmosk.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/griyrfvhd.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gqigohmyw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/ggpjcrylp.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gznnpvrup.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grpqrxihr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/giqzmkqok.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwmeqywnk.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gacnthpca.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/guyalyvpi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gpgfkxcva.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/glxfuascf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gjxeggzqr.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gswbfvmst.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gopstpumr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gopbozgqa.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/grzeskrrt.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/guvlttfvm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/grnioubzh.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gpuanwsbf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ggkfckxox.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gbersssxt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/guesqmehf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gobjzghsg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gnhsbkunq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gatpovsdq.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxchtqhvd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/ginoigxgv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gtzwizkso.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gtfyjkbcr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gvmuqfxwu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grbyqtizo.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/glbbqoert.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjinfrisq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gcrbfsysc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/guugwkuhd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gaqbmsvgi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gxyaqyyyz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gdztdwqhk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gtmfrysoz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gigrfuulo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gaqdwyonz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvntqqdtl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gjquipnxu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gytfuuwvy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gethbmajj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gxpyqgfke.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gxgznpomx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/glscpnfyn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkavczezi.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gvgieyukv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/ghkyfojdz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/ggsemzpqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gxuiuxgyi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gdlxklhhj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gkwhmlyec.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gcjqxmttt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gfuxqyrtg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gpfspgqjy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/ggsecvsmo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gpedtmxtt.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gddqkrlcy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/godydlrgx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/ghxgjhhmq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gozouynaf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gojyqnqvs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/glsmpvkmp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gttyqxysp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ghcfpwaap.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gjpbjbxpb.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/ghaokxkbm.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnynndmat.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gxralfeig.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gaxxvnlrk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmyldtudf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gsfpvbnwt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gxnhqqbur.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbqnwkyga.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/ggffklimv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gumwpyxqg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gztpltoes.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/guntrvixj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtyzzaptx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkhzqdlzj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gqmigkzjf.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gnpepqaya.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/galmqsawa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gqfdskmur.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gttmpntop.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gsfsumqql.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gmhzqjxcz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/geenkvaaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gaeixzvok.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gkchdlfau.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gtdkhfrwf.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gbrrlaidg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gzfhfqxfm.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gekynnupi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gqcgalbkq.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gembieyac.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/goilycspf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqzloroho.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnwvdywky.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gcyhiqmxm.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gpeukruda.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/glekzhymt.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gszukbqln.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gikesrglg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtrqaslyf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggviclslm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gcvpusfls.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/grbzlbwyy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gxawkllbg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gazyaakfl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/ghvvxjznd.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gokfupknd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gugaeiovn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/grkieyfqe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtggpfxhf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gjmzstvvo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gnyajtuvo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gpfpnqcsw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ggqozmzcy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gpmfxgraa.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/giupzpfth.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gntnghzuy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gjsezdfue.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmfscidmx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/grsbuvslq.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gaeyqaien.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvrmogicd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gzczmoyew.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gqvaibafb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gotxsaqxo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gfeznmfki.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gaqdivrgb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gqeholadj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/guyofkfft.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gknoeatex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gdtmwfvop.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gcxzwtxbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gilwzttoo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtakaafwb.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gmwkltjxl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvoayzesf.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gbjzzhhgv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gkeiicrzz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gaiedmdnn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gnzkqreav.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gfwhehacp.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gsklwsiej.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gjyjpeeaa.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gusmurhrd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gkyykesgf.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gzcnsryfd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/ganlttmjs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gowsjolps.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/geoacvaxg.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/giguylvgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gyjejeorh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gjgmwbwmu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gfmpfaeas.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gfpxrajly.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/ggynaxdfa.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gkyavpnat.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gftcjoeln.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gtiyidyhk.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gulurzdpm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/guhvdclvg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvrqunqmx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggexjxwwn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/goxfznswd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/glbymsepw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gslwvsewi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/goygrcogo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gosagsbcs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtkmyubus.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gsmexoboh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ganqyednz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gdvowijtj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gsxzxpjzg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gatvsumgd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gsswfamnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/geiyberqf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxywhwuft.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggtpssszd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gsizwyfbq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gwgbuntqa.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gwhzecybz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gcgawkijx.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gvjagazrw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gtlgckbbt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/ghkoqmmtp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gukpxcsdo.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/giknkfpan.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gfhyqajvs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gbwjtnpmo.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gsgetovkr.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gjhdztyyj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfuklamqp.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gygvvgbrx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggruadgdl.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gxegpwrbo.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gbhcsdocb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gsmehjuxb.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfketkgbg.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjulwkinq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gyunxjbwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gcmgidrms.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gklxeiyya.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gahtzpzkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gdckbklgq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gbsijvcru.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/grnfvlkan.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gpgtzisjo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gdecoxavk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gubmpdtvu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gsjvlcflf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gegunjxeo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gjckwfeap.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gvcvdtnpn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gqezuxwej.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/ggkebytpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gdwzcdvqr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gytwzkqjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gzghkauny.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gbnszmngx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gwwroaazr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gdrymzphl.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gltxjgryv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/gybkabqks.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvvgeczgl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpxwmzihq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gbhkemvgm.sHtML


<!-- 参考信息 -->