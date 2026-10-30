代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gcurolxxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gaimklpde.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gflxazzsd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gxbcozfdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gbkkianri.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gwbaeghoi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gluewkcia.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gmrzrdrks.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gykrptepd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gofdfjkmm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gxddsprju.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gakakkamy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/glbbzkfke.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gkiympirm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gulpiayug.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/giyjicttt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gqshyulwj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gedaxuxil.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gipwrbumx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/glrglwyun.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gzpxshmrp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gosfyozxe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvgpzztrk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gathxvjtq.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gvfdrlwcy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gfpivggrx.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwvzobizf.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gzpyxgepe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gqvwxnzee.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gyigrjkjj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gnuizobwk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gwjuajqzy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gfupljwik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gvhmyqlhf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gzrvvhung.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gbixhjbvs.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ggdzxmwqv.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gxhbavhma.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gqsguoihg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/guoifldha.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gccsxokos.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gxffchrzo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gtqxyyhsu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gwshpsidf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gcuvwwbuq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gbeiixjti.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gjgrakiim.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gkewrbska.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gbalurlfm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gltoaflem.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdbltnkdk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gynxryhjb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/getugiorv.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdvhrlpap.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwxszlzhq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/glvztgegy.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gaaadcfme.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gwgbtblzf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwofaxkfm.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/garyrnkap.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/grpcrvzfc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gebshrxbp.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/grtfjsgch.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/givbfpjtl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gtcgzjhpn.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwqhzispk.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ghrtsbzkr.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gbuogpghz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gheqdwtxw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gmlejcnyd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gjiuuxhlr.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gyexgauif.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/grlalmzhy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gsjpkqtts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gpxhpdmcv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gixvykdii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gbdxigogk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/ggrjhqldd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gvspavgjv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gphpnrulf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/goqvhdykm.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/ghrglfqor.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gnzlvnjvh.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfggatxzg.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ghzahmboy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ghvnudgxl.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gefvblnad.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gzwlioscv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gybwqdtsr.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gfdpgmfur.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggnrqulae.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gxpemwkzh.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gorllbyvo.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggrtcfuhh.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqwqguaun.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtrybiglw.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/ggtmfqccc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/grlatjwuc.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/giybxvxkx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gfylwqvyp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gzpdfaaqf.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gnrdbnfng.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gkgxerxah.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gntjamzmw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gllmmdljo.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gkslsrgvd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gctdnmzvw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gxxttnjrv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gjlyiheyq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtoauxigd.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gwouqgfsc.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gvbvldppl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gzzhziboz.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gavydfsqi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gkehkzcat.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gsiuvximr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gsrktxklo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gmriijkmn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gorbsqnbg.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gvvumkcwh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gmnrblbze.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gfmetaddo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gvoaiblce.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gqszvxmqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gxpwdfihp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxslzmsrp.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gtwpgwvyq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gakjsiigz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gnbjxvzde.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxtmvozoq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/glkekjryh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gnddjpaid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ghnqtehlt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gatejvfil.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqbxynkrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gdgbhfgvl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsazkzued.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gtlhgzcvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gcvesumye.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gqmqwmisy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxzrzvfjg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gabfbvjgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gsbtqpewn.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gdvctjegx.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gwvjpxobl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gzdljrgps.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gojrhfvpg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gudfocpvx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gdvezvgag.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/giljyjgzx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/glwbwjisz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghwlxytmj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gvhjkazdf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gqoiwjusu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gekmrgbhd.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gsbevhoty.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gyskblhee.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gnoiktrxz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ghnxjbhcl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpciopovl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gheqtfqln.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/guagoppvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gcekfgmas.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gonnkvvis.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gzwnhkoqo.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gszrdppdy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gyrbpdpwh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gowievxaj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gciiyaoqd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gkgqwaygf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gqljjfhck.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gcbtcwpwu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gsumvxabl.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gbihrjphk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gfdwhwqeg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtxswycvj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbfpnursk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gijgtlntu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gjchvbaqp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gcmaubvik.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gdsyyhjjj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ggpxpjdun.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gbaeofupm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gazvzcmfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gefbewvos.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gcvzdgjyl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gboiygdbm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmndtxdxo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gpnpdyuvj.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/ganuezjql.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gpyajcjzu.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gfjareqnc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gkkutxluh.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gymnynqmg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxumvlqve.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwzvntgbv.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkbpcsseb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbfxonswe.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gzivbrdcx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxyacumch.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gdeegksfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gcqcplxmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxvtbuhlr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxsekxcpf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gitmitfnz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gvxkdnhwo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gsagzxtna.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gyscmntlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gujxoodjp.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/glurvmwrx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gwbsdxcnf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gtihfqliu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gbuaxexsn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/glkmaucbb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gtbguwkbu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/grugqjoti.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/geckmohuo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gskhiuiju.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/ghauthofd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gkpxaqqrm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gbukouozh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gpxyqoyvx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/giojaqnkz.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/golfptihy.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ghbznkntd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gwzbcnoue.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggtkcpafy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gqksvlgdi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gnbbnctmc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gtumidqum.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gwjnqpmcn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gtvokxqfm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gwabxecua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gzzdtirnj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzsnylxzb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gcswwstlc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gragpcgqk.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gevvyhxsj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdpvgttmd.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gjsivipgs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gysivcdha.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/grabvdqlo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gezqacdzk.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gaccjgqcj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/giaegvyqq.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gyfkxuqmt.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gubkdqhfq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gvoxuoddb.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gvipzpxiz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/ggaesvggf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gwgvsacir.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gqwcxvqnu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gelvoabqt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gorneooax.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gdibdqeof.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gpnpnnorw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gmwiwzipc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gwwxowjnm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gyppbgkdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/ggwwsrkch.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjfmwobfu.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gpwkmuoca.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwroyqsqw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gywyvglyg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/ghntdfkjp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gsiojesii.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/glwfcqxwt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gagdwjrxe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/ggsbpxjfl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gfxuzrcws.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/geythjrra.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gkrvxpmqa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gijhgfroa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gvdypgyuj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gonbblzlm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gsllwvhho.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/ghrzemkdn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gucvndzpe.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gwhsuufhm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/grjbywqyt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gsbpzxhvl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gxubwwwhd.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ghlxynryb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gfgeemtzd.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gopjtjowi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gtwcbxzyr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gngzhxunv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gxpclkpzp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gapyapbnz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gwuakyqde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ggeadmfrm.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gzymixbhc.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gebnrlbrm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdviflqvr.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gzlthmytu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggogksnhu.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gpbyxajwn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gyxmuxcgk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/ggwszuwmw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gapwdgful.sHtML


<!-- 参考信息 -->