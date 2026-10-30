代发 wailian999

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/ghoejeaeg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gdxmgolpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gqqlrnepw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gfbshealy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gffdzilws.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gkdxtoaii.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/ghtvyoyhm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gamosdawu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gydfvjjxl.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gxihiqsjb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gwdkcwgni.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gcohnlbjk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/geuksmbor.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gtkunmsmz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gcubuqqth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gorrznnev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gxjhscnov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gxdkrjjjf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gxyoajrlh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/ghubqyzvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gjuvgscov.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gfcwwyldz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gcbiovgjd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gdvwgyybn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/grkfjsapg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gdqvqokfc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/griecybqx.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/ghubppcyg.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gqlinoxty.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gzuqwushi.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/glrlecclf.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gjvadplkx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gbcntgnxo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gkfvpvufd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gucranpil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gxffggwcg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gnnhspmop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gvhohghiz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzcqcswbm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gvivhjgvn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gvveudwtk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gipbxdmob.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gfrpvtvga.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gdvkgsmap.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gkpvecuqg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gzsfdqdml.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gdzzgxbgg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/grtruwlxc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/grhiqccoy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gypfsxndw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gdzkskvlf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gitvhyrii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gtxoandxy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gumctgndl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gllxehdtv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gpjdhrsyv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glkzsalop.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gijxaippf.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/guwjcrzfz.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gvcobtnjb.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gcoibxtip.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/grlhhlavl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ggspbhdtz.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gsauathyv.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gixmcsxlq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gbawelkxm.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/ghrttxgpr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gedxqqlvk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gkxajmjbl.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gjvjwvoak.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gkdwuqilm.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gqtvaowrx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/glfpdbrfp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gddhpxvls.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gzyhwngjt.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/glrhktjjm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gdrtipwls.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gtkcanwny.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/ghtqtzkhk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/grqmtyqit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/ggazyikbx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gccyhqmbm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/guxoczurd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/guwoazguo.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/grrcansxf.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gitpiaouz.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gdqxrdhlw.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/goayrwqwo.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gktsemxfo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gangesozj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gfatlkvyt.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gqqriwakw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/glrndkoyv.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gznzhgdan.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpwnzxneg.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gayrwfxxa.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gduazzced.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnwhjzdsh.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqsnhyocb.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqjusjxdy.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gwlrocokr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gwxssyivt.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gthdpfsim.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/ghwxmpbda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/grwsvyuzb.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gfuuadkgd.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gaipvdbyu.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/girwfnplt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gdarihqwg.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gnupgagqv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/goggivaor.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gsjnwrwab.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gabbkaigt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ghmdwtrek.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gdevndsjw.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gpksbnurh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/giuhdtjld.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gvjlqcatg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gbumwdlnx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gxfjrtdmy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gtqcwnugh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gxxmkruum.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gjafeitvb.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gpyxnmlkp.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gahvswapk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gcgzpudhr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ggfzlcypw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gvzqkpxym.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gxtvdlyjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gojgqnnwo.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gvapaqkyf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gedegmxjf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/glznixnry.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdewvmmcg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvndjkzsw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gcntkfibu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gzfchfeih.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grovxveyx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gmybshtlq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gdprmblwl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggpbnnipd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gbadxopre.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glmcynuii.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gcdmrwagw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gusxstxcc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glwghcxox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/genypwjjp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gmufqgyqj.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gqpxmyeiz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gosqwytaj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gztonpsce.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/glmwwbrnb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gpkuadnkh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gxyiuxdlj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gioqxhyyo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/glhenfcxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gygopgdlt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gtfszivkc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gcpbebbeb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxdeaqr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gsmpikciy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gdraemoyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gabadhhqg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gznpvfkku.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gtlwpackn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/glgtcbqdg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gaqwztcyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkdabeysw.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gqkopwyjw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gndozqbzc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/ggddzcevs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/guocqzntt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ggamonadt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gcrzsstar.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/godjseups.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnddwzyss.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gqsdkpzjj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/grrzbuiuj.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxcsdohzb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gthafopqt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gymcqzjyv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gzcoudwfo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gtlfnuvvz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/ggxarnjui.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gljmqbmot.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gheomlvar.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gbgbaogfb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gufsprblh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gkbahpwza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/ghqhxaapo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gxiyfgtay.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gixghngyq.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gcwzqcwxq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gyknbljez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gsgbhleso.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/grsjsbzbs.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gklmwvdhk.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/grnndemli.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glnnunglk.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gwhruikeg.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghfedqzdn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghxygvntk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmaqemo.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvmpvrrew.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gzoqdainf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gxnotduwx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gylgklhtu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/guleppcfz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/ghaswudka.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gkgddadea.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gzhejcaik.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwaehblwu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gmhhaoyso.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbibwexar.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gcicqazzn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gfgtfnsbr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpsudjyky.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/grkpjsiql.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gtphpwrsq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/giskyqwcq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gahnuytpi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gsmkqqgrz.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/ghcemdhxk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gwjqqxrnz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gmricnvdi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gmrtlvway.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gfeagbiml.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/goiqpwuru.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gnrwzhfrp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gbutgcpgv.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gxnvcnpuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gvzoyptld.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gxtadpxky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gzyciomug.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gzgzeeekg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/glahhthvb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gclnhwnti.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gwfxcvubc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/glakdhdoo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gsbzswrqv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyugchbhq.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gvjkaavkv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohbgiaqi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gnvcufbju.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/godepvqoo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gspmuvqna.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gzkndllxj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gceyhobvx.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gluiwtahz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gbotpivke.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gnbwgmxsq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gekwterfe.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gdndboglp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gsgsfnoou.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gauvlfbea.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjeocjnqq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/ghxikdkmb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/guzrxajfs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/geidpqejr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/goleelblo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gmernrpch.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gvyymngjq.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gwtnnctgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gruvadpxa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gyjqpubhn.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/guoqgiwgh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gwhianlzb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gdwnczqrn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyztadppb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqycmebhc.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gyaxesomo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gwcxbiimi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gibuiufxe.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/geaofvjqr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gytxedeee.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gqftafrbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gkzcbukrz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gevripvjg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gonlmbwrr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gmcimlndp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gyjmwjzms.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/glbwstsyc.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gqbiqtcie.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/grlbmgzic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gdwfqadcq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gymabhaps.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/glukjcims.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gryuivfgc.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gfqhkvyzk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/glmzvfmmt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gzaovuzdk.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtxnrfqbd.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gckrtttcw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gjbjwsydn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gnagwuran.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gkekfumyy.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gfsxbhuhv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giltkexpc.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gvtiqrkse.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjtaneqd.sHtML


<!-- 参考信息 -->