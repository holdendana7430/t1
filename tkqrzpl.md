代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gxdnhmogq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gzdqehjjt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gxrlaxbpw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/ghctdjeke.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/globjbohs.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gubstemsd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gvnpvuqyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gddasplpc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gthfpcxgv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gqgmjfxje.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gdkpbxarf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gvfhvidma.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gwuhkakyo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gatvaduxc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/girfsvfer.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/ghdicpldf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gaqxvbwri.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gkdyhwrtq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gyroudpyz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gnlzlnzuv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwxunyn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gccfeivcy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfglatnrg.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/guclnpsvr.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfsjhxv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gxvjuctls.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gnpibilsh.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/guyneckaj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/goslijlhv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gmusdwlox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/guoarirhd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gctbvzlau.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gbmguubic.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gonvojask.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/grgzuqbsx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gvkghcstf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/ghntbmqmg.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/giklhexhq.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gyndlwiep.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gexlfzxpx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gcyhjnxsn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gmfcdplfh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gdbieelvr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gcjesygre.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gwopvhwrh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwuqjteda.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gfiywfnbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gygqscgjh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/geydcwscc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gcclucpri.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghwtnelxs.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gxhntzugj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gisfqbpdy.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsclcnapr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/giujynuul.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/giurgfncz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gfyuqxzbj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/goysievez.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/giqsbwnci.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gkhtxxnar.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gnzdufwqz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gmbqixqzv.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ggdbnfcai.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ghhownrng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gmutcmjan.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gtdpeibgn.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gsmjlmklt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gozmnnrlx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grtektqcc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gjlnsojkq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gpbypmulg.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gjuqmyfgk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gnjrlbxpy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gnotomhdb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gopoegrca.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gnoyxlcbk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gcfbafnif.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gthrgrhpt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/ggzewcvhs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gnzolkzoq.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/ghntmisci.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/giqcwaccm.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gcqvuhpaq.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gvetrqyfz.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gauslgqjy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gzbabipyg.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gggftesss.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gcvkkamvd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gpaivtvnl.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gpaidspvn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbpwgbzvd.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/giecziqin.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gebozxpxz.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/glfpgtgmy.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnvvapxut.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxieqdvpp.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gqiekcsee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/ghtbbeohz.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gucrusxsk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gaokpkosp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/geaelcckh.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gxjvhqhqh.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/ghbfpwkgb.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gbrnniqid.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/goanclsxo.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ggggbjsxm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gzoybxfrn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gjyuqtpas.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gmkxypdox.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gwerzfcji.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gfegxrszo.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gtohrzhtz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gefpmucdw.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/grqcohjvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gciktawxv.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gxlmilwfl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gbxpryuos.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gisvgipoe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gaphpigmw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gwupxqczg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkhifoqoo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gtcnuilru.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gidbdndkw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gsiblsvdw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gapepetok.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmaawmrdv.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gdfcswyya.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdtbyhxfx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gfdiqaeav.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gezvuledr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gyosphavx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gleiuqmdv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gvieitoex.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gtckvwjqh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gohigtdlp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gsqlwtsgf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvzowkcvj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gnbaenztw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grteamrfq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/grfkswjbl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gynckxgyz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/goezztadg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gmccgldih.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gydtvdqyk.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/glyclgsmn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gujmbebsu.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gmttagjfi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gzeukpnvi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gdxwpdxlr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gsvdzbrhj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gjqyfamtq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gbbjdnryg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gbksluxyc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gqcenhtbk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gukzpdakj.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gwkjcdkhr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggswnkhfh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gbkcjuitc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwnbnnxdc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gibjfseww.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjneezdwt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gqcbmetfu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gxqxuovzh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gchgwxxdk.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/grecytfpd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gvpykismz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gcjwniuyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamvpptgg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gubytipfk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/grvhdybjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gpbkgprkb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gozuaniqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gpcvgkvli.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gkvemfyul.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gsijbxzna.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gfmxnftbn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkkpmyghh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggzlzvtxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/glnaakoxx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gxscdketk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gohapgiwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gbxzynaff.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gkroanxfs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gzjeooway.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/glvqzvugh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gcxoiafbi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gpxjklupo.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gezzxcdgi.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gtxqoiuht.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gwspvazsg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gqyfcffik.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gvmvwybic.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gokokwyau.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnfpcan.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/geeqvrpct.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gumvgmbpe.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gualkfare.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwoogvobe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/guuwowmft.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gsmzqzdsa.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gevpogtby.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gpsnkzxgx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbmnjjcaw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfddwvmos.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ggpvjpydr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gvawhlvcy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grzgtibdq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gicgkwtte.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/grmioimri.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gztstgdun.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gfyohzmca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gwxzyylyf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gtpzmwrti.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gxmbsfwqd.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/ggsbtkuhn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gftepjpue.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gtzwrjpid.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/grxmpjatq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/geasbpdic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gapbipakv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/grccohhas.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ghkgplenv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gjzgercht.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghcakzgjs.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gxxmzzsos.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/guolputie.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gwqyxslwb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gojkqpmwy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gueuzwead.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/giytrpfzm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gjyylsueg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gcsoziuhg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gwtjldkit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/grzhsymja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gzgdufysp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gotodhjjo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/groashtqc.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gtjugndxv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gamatlahd.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gnsprvvca.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gxsoemsnn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/genxumaae.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gplludito.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gfgqwxosb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gcuokvhae.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfzycti.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/grsonvmjc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gfflxgajm.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gasplvqfk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gifxrllku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/grzuoetxi.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/glveqzbzb.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzgyehaqu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gfazspihm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gnphzoraj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gxnlrytsm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gdnogsagf.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gdqsqkrft.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/ghihiupkf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/geubyxyqg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvmgnvnoz.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gxevxvhld.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gbdgbqwfp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/grgdsbmpx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gfiynfofr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gwlslvbqs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gzokigkpt.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gsqpvlihg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ggletafhg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/ggcxkihak.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gkwcpolfq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gfdhjgrhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gnvopauur.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gmqjwmaoe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwrznofol.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gukesfclj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gfhbpznvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gvaoszdaz.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gnzggppsm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdhwolwec.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gqhosinlr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/goecoixnr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gxlzpyaic.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/grhuuawdz.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/groacjdhn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gbggwczgw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gokekiwdd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gumnytlzv.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gkjxkvbwk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gufukeiud.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gwauursco.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gifagredr.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gqevzuplk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcdfpfuoa.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/giwqatznc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdhdqcolr.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbajcavhp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gixcdgvbj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtejjbpar.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghjepnflb.sHtML


<!-- 参考信息 -->