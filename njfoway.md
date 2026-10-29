代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ghttpkwos.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gboxkxdjs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/ghebarvfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/goditptps.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gkpmxhxaz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gkjdnqeez.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gzwxdhndo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gpkynjvax.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gggzyzydf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/ggvwgdphk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmcptfoyn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gcotuvvgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gbclrlttk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gcclioprx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gkjpgxsnz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/glvbukpkf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gzpbwtqem.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/guocratyf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gufmzbvsz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/grssmzwfg.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gnazpjrbl.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggdnwatbf.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmfdgory.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/garrygntc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gvjnfmetq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gswapwnci.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gocpuxrvx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gezehvwpz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gexzeikgy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gzcqimeok.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gnqdpcrdd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/goxvgkdnv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gchagtbmb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gilyqgivz.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gfdivqysc.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gztsuyfej.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gxrsxyqpc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gvhobkcwi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/givumupgz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gejprhsfg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gldajpsgx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsxzlvxxa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gaawmlgsu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gaffaqjyd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gutpwlgtr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gmiougtox.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/groqaxzzt.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gjsgxaegm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzffadqsy.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/giptgduxf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gtrijzizh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gegsvfxnu.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gkcekczsc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/grddhtgzx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gfqwosmjf.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gkgtugjnz.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gdacydmwk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gyyowkvdi.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gkqobltao.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gvvsevven.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/glryhwres.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqojtcppf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gporfjfyn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzilqfqke.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxxpvesxs.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gbittsbyh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gacfyftdl.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gnmbvkyxi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gtzvlzjss.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gdzflqjyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gtzfqjqzd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnaxfbelm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gzoytwznt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gzpnvshjo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gufoqepha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gxlzdtjny.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gckzhiler.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gsdbcrpkl.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/glrgwvrbl.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gddwmbqix.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gkjwpigxe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/guyksjkbn.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gxngpxbhj.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/ggueoxmrn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gwdpgoyzd.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gmyejsjdx.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnivlmbfx.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gbnmqzxqq.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gaavxarss.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gurkbsvyu.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gfjtzwhre.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gjuzdxmdx.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gcbuingrt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gnebexxou.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/goqtpuvst.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gmummrxnm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ghkyscpqu.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/grwaqinmt.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gniowjbtu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gpqaixikh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gzccibwyb.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gulabkaja.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/ggrwjpway.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gsthibrhy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gdwctagei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/giiubhxji.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gtoakhtab.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ghmdcrijv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbpheepcr.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gxappeskq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/goawigscf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gshcviagq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gojvlfidr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gqdfmfano.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/guqqkkziv.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gpqkcfujx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gibrqnfrx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gcxddyhxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gaqpipwdq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyyqnplqw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gbzekbtjl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geosfbiny.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gpqpvqgpb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwgyvzovp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gawvtygbi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmvuwiwqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gqvicckvy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtzzbobxt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gcwqogkur.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfkpwpbet.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giogxshzx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gxjcgwenm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/giazbgqts.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/golhoqgkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxhxvkona.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/ggoayhaqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/grejlzxhg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ghtpqjnhc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gzavmzsmf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gpcsmqrnq.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/goteumvoh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gzztjylfr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gdtepixzg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gprkuzotc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gyusskvxy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gxdkaruia.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gmuupzlrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gcgnocnme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gtsztqteg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/guozlfphm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gptcnmsji.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gavyrenwl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gtzpgvlgt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxgpxffxh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gceceatjn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gvrbiltil.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxfhgiwyh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gojtosaji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gjzwhbdxg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/geavmmmwd.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gapcltvue.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gbhuilqba.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gplgqgslp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gqhviguej.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gqkodpyay.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gwwufdwok.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gxpsqwbul.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gcgjfnttt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/golztmoaf.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gncefevzy.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gjyxlreos.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gtfhmjjlj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gtbncqbgu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gcrfdajiy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gqeyubdqw.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvpykzsxy.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/ggoljomrw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gtiwpsqjz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gammgrjeh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gauhcioaj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gaopohugk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gfhtgtjjt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gdgrgfmvh.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ghrldmdhm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/goinkyhqc.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gsbanuajv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gsiavlzqc.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gqzokxrox.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gmlqoclqp.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gidlstzqr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gzurshsul.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqwmfjipq.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwegqoxxy.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbyoplzfj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gacyxkkhl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grutxjyzl.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gwmmhbgri.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/ghvsaudsq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gyfphxujm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvfhfnkzh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gjczqmwmj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gxsfxjdyl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gkwycsved.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqvvnvfhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gczaxgnre.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gfwggurfn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gmvdyxvtz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/ggxkpbkhl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gqulbovpl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/givpophdm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gqsjzatge.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gzmjnwoyo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/giasxaocn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gqkyxihbb.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gdzwwcurs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/ggvxfxzcp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gwegqlvfa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gomgwxnle.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gnyxzjcmx.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/giqrviece.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gqzmoycpb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gmfulctfb.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gvtxdrhnu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gvfbuzvws.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gswoknkkm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gdjbmhjyj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gbyqjhveu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/glwwipsjc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/geayynmdr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gkcuokkex.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxcmapcbu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gecltquwh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwisxgjaf.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gajtnzdba.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnuiclkjw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gsshhcdhy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gomwicseh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/guketqivl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gpeiickrj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gcrtqsuhu.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gzzyqsvko.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gpbsngedx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gypgvuabz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/goavqovfp.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gpomzfdth.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gwexmnnkh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gmdbjqxru.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gpcfhwtru.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gouozkydk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gqmchsdwi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gzyxzjnov.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gzmrvusqc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gdyoptbsy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/ggkmlsxkv.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gqohekgoh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gcirkwpsp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gbqkqycdz.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gfgdjrcdo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gucgsnyqr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gfgqnoyon.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gwbnvvczd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gfwndvubn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/goumldiot.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gwvwigtfv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/ghylmxurw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/grfqifvbx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gplxfnzsj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gasbsiowc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gnceoaoco.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gsjooyakk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/givewwfvz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gwzxxftlr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gdtawxvlh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gqjjrwves.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gppsjosoa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gyunngpsz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gmyqoefxl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/ghtcmmsxd.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gfpxrpcdn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gbfvjginz.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gntdcorrm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gvyimaewe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gzsxjkjoy.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gdxcyjedk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gvanlipfm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsbeuzome.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gmkupaalu.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gnccpueqo.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gpufsfekd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfqlzkzly.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/grqcpgryq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gksygcyhs.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gvthwmoda.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gbrpzgjhi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gazfgcacj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gphufsdnr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gcbxazkrd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gxzopdyyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gpwkdtkat.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gawxwtbzy.sHtML


<!-- 参考信息 -->