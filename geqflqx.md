代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gtekwirbp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gxyegcvcn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/giqxmpzjg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gizscjjwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gnwteopaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gpuyvbhrz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gctpumwbm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gxewtffel.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gbscqrdxr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gsgwmkjyd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gerakdzef.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gqydyhcbb.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gtykbhyow.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gpycbmzrl.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ghyuqfduo.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gdwmmgdpz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/ghternzew.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gezdajlga.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gmvpovaoh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gvkuuvluy.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gdkqwdzgx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gfwxqhyal.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gzyevffay.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gsijuutxy.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gecvsxpar.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gfvfcfsjy.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gvvorxrvt.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/ghckhixyi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gexqvlgjx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gmybspqbu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gybfjjsaj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gbgfplzne.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gvznssyta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gvaqlwppy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gatguxgaj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gullaudvj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gybxoabvc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gmrlbjetl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggeyhkrqu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/grsohwygc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdvzqgilb.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gjplozyvf.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gdunjxktv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gqmxofsjy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gftpeatbf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gyqarthhz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gznkzwfyi.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ghblnybup.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gdkvhjjna.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gdoarilng.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/grguskvqy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gjahzhsri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/glmhjmzyx.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gdrqwbens.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gyzafgsfe.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/geomeyacn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkasjlvev.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gjrrunapz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfwjkrjup.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gdfsmgpns.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gghbinhrj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gxufwonwm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gnnlveyak.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjizsmjnw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gnugfxtvr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/ghwirtbgg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gfsgjkuer.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/ghisrolcl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/glfayfypr.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gduhmxkmm.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/ghsaretwc.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gucohsubw.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gaachrohl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/ghdfxuvka.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/guiqpqois.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gouxmwjtn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gyorjyuac.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gdqvoagfj.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gojjheoqf.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gmufhofrc.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gshpdssuq.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gunpllcrg.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gpqpizoda.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gknmqbbnt.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/glfkcjkki.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gdcesmbfw.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gtsipebxu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggzgvjpae.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/glwwsoobc.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gbqtnlogq.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gswyfjznx.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gmsuvgwpz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gxwwvwigc.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gbwmzklpr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gllxlxqvq.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gghhctgjk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gnertnumw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gigspzcjh.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gqittbfkz.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gzaoywzzz.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/ghjhvkcof.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gncxhcaxn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/grchbhhgq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gmcjlvzss.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/glawdjljq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gcfhejojw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gzekktzrd.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqiyobnzu.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gezsokhwq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzqemiz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gmanusjml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gmayfgmjv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gbrcegbvf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtjxaxyij.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gnjzbfkcj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzzanqgtx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/ghjkroinh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/geuqgmfqc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gqbqezmsx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gtsgywnvc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/guewivxvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gazalxxsv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbflddyqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gclhpthhd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghgmqmvcx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gtndjcxaf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gbpysbguo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gqvfcdmyd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtoaborvs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghhsvqova.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gioyhcvtw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gyulgxntt.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gyiumvhuc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gocbwsakp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gbekbqmxs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/ggrsfiics.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/grnlgniap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gacgrdmez.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gtjgffhsy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gqhjtppvx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gwydbgtvn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/greevwzwz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gyfknjsyv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gjhuewizl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/grqnfjmok.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggacnjpzd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsemjavxh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gcxplvial.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gxdahydii.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gjaxntncq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpsiwmcyk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqvkikhan.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gtughhutf.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gffzqdjsd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gfcvcmwdw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/glnkebufi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gfvfmuhiw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gmxjggyem.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gapvegnrt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/glbfxbgei.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpiklsbi.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gnfifjusb.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gxjtdbqzf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gbaaxfmqp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvbqvqbkr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gxqqjkgxt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/ghpblkuhs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gsjakpdzd.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gpftpbjcz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gkhvwpbsr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gxnkmmouo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/glsihlrfm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gazqyyqbc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gvhoyxrtq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gzqmutyfu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ghipxcebj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gvnqfiweq.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/goysgvlho.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/guxyhaqrf.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/goqstmzdw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/geshezufd.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gxpebinco.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmmoluhea.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxdmzgjhn.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbeyesbrk.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcepzsmwu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gmtfgdtfj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtrbmlwba.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gjqmclbgq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gywthfyfu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gpgqfwztm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/goyquvpjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gihmqwfbz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcjfifxuj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gbeureflr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwndckolc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gyffjcdet.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gxwselloa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gqmkxlspl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gftmhktlx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/glcudirja.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gtgqtbcbm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/guqngixjn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/ghwlkikbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gwbixgjnv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/ghsfcmfij.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/giymchopc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/grszqantu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gjosnyulq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gutmkhetr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/govqhqmhh.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gtroxqbln.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gvyouernv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gcmpocpbo.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gedcspgtl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gytzfvskk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gthnypgwj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gzpkgfqme.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gszeqacsm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gyhrjxufn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsucfdi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gxmjktljf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gkcvcqxia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gbitbjcfx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghtnyfvka.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gzsrkxxcd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgnyamx.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gsgbwsbky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gggxqueww.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzzbpcscs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/grmpmsstr.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/ggftldhtx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gyeuygfjt.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/glglydeer.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gxyjeyoip.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gprgcycov.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/ggfzvxfwx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gxjfvhrvf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gdpiqtkmy.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gioqbjlkq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gulwavjsf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gpplfwxdk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gnfcyuttk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/glvtavcns.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gvfaqcvyp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gwrpkgntv.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/geszxzohh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gbuyvkwtv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gaivqqbkn.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/guzcmgqmb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gmflaedqq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gdwpeslgt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gzjcdcrdc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gitqoehdf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/grsrdqihn.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gbcnwevza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gfwqjdbxi.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gtvdogmnu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ghjoejulv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gkgjdliad.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gzgglabsp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gqmbwcnvp.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtflkyhny.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gyggelzzs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gqjzgwmlj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/ghnhwwiik.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glpxwruhk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gtgcxtfud.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gmpprxcli.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gwhpxjfkt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gnsbhjphb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/grfnropsn.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gstflgvuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gxzoatlce.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gdpqgtnhz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/glwrbgjzy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/guzukdfjf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gjxzxqqhz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gubjsuncq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gxvtpvqcm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/glbkwviqr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmmkfrbxt.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gzgladpsk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guahxnaex.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gmuxyctqd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gcvmyovoo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gabbkgwad.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggpowhvmc.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gabyceofn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gtcxcvlww.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gmtqmafbn.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gwrdxcnab.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gvkbrkpiy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gnawukqqk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/ggkxvjkao.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gldhqcmdo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gehdbbrme.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gmdmyaevs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/guxkmplxa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gmofpaixt.sHtML


<!-- 参考信息 -->