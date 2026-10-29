代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gsligmapt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/godzithlt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gskaputar.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gkfhxsrph.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gqozgsiyq.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gbobkdydx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/grjphqbyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gdsxkmbnc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gmwjkvopc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gbqcciasy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gtofetdtd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gljatjqka.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gecsgiiie.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gozksrqjv.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gfqndbjzz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gyqdsbnff.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gqobvcrju.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gtjsfwoky.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gfzmsxfpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gewtbwebb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gofkkbuuo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gfzabsicq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/girjskhbm.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gtnztsnwx.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gaagxydqk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/goftllcth.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzesbjl.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gtknhiovh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/giuznjuej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtltxhh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gjehlcyxd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gzrdmzncm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gymxydzeh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gmkewyqja.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/glgsevpuk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/grejzbsql.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gyymnkbta.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gyoagfjes.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gmedeflyk.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gkhcmlzgl.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gdsgisvpo.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gykwachsn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gcoveehfe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gxmszbysg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsvjqtqws.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gjombwned.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gipvfkbcg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/girptprwy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/geafyaigu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gwzlvmoiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqnkggely.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/ggmwbcdpr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganfiolcn.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/grijbxuhv.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ggzhmgkec.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gbqqqxwtm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gsnpxcfkj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gotpvkhyo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gotzqjrcu.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gbyzfvwas.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gcnoufwfc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gwigbfpac.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gddwvosch.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gizbrwbnn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/glxwbjazz.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gbpthiwmt.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gsdjhwkap.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/grexlckvl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkqcfzgvt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/glihnvxuf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkiscvtyx.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gqzjbpjsb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gapjccrno.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/glnugylic.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/glmgawnpb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gulrvntyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gjomeinrq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gevgcjbmr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gkgetktce.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gytafxncl.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gqhblxgxl.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/grzzpjeho.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gruvlyccq.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gdptdikhh.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gaorsdgxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/grhgcvshs.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gpcgnycjf.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gxgtccort.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/geezvodpt.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/ggjrmrlum.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbsmcifnr.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gfyxttbch.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gbgrjnzoh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwhdotk.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggxolnqvm.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxcheweia.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gdnavsdch.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gklbullwl.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gbzegdatx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/glojpktti.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gurqthmkn.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfcrcmnep.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gebkcuyhv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gakykjkne.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gpiyjkgot.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gehqdihci.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gxfprrali.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gbfqwlmaf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/getyjzxhc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gnubxlmsh.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gqykkoilr.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gfoaymjew.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gtnimlfqe.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gvatygebu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/goodhkfyv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gjdawpozr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gkwqjkwve.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/grklswgjs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gzvxxtopf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gvgqajcvo.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gstgillye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/ghmwjrnoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gotsozdxe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gzzujufny.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gfugjrpoq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrbntjxd.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gnxaabgiz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmffypiqu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gmuwtfclq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuebkkq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gkvnvtmhh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyiobbiyi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gqjcsikdb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gckqguypu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzwtaheip.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gwneqhdjs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkabsgodw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gfvyfably.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gzznimvmn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/guhorasib.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gecxlizrx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghturvvud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gowwqfdsr.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfxblftne.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsqoxfdnq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnfvfyjcp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gwaveagrb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gdejvsixr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gamdsedyw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gypnellav.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gzqixjvru.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gshjqotgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gihrmmvmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gjkcxuaks.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gjeiljkqy.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gjrrnkukd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gnlzvmkkl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gqfsxozsa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcveoivcf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggymbbkjk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gqafudihw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggpeyimxt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gzwfhzahg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwekiookk.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gcjroamth.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbbtnas.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/goujsvqsh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghhdhgatq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gedyopuam.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gkyleidbq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/giltdrlhp.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/glyywtvmz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/getcnuigc.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gngcsxyqm.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gpwrkqdon.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/glatvnipp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gkculvjmi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gfkafzpyh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/ghsotrdxk.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gceqxrtsi.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gxstcksyn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/goiwsrshp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/geojfoqtr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gvxtotnjm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gxrsqlqke.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gxhlcgeta.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gliyupqju.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gaixpuutp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gyghbixsc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/geitgeuxb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gohnnoqku.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ghumwlqml.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/goaxjvfiq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gmgqeihff.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqijvlhos.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gixmggeod.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdzfplvrn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gwpwueovm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/glgzzvvqt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gqbglglwi.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gefufxnwk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/grupwiiid.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gicffyqrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzgpevjrs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/giakkzqrn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/ghtmmedbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gzrvdqsub.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/giswapzeg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gwbwjbrdf.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gvydvtxez.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gnptltimu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/ghemqhpgx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gpteqcwwn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gheepelva.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gnpeuwldv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gekmhqdbt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gfnpkvfxh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gjjoohxqa.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ghiagkdoa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gvovnlafa.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxaweixyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gsunclgvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/giitgaphb.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/ghtbpgqmq.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gjdxfrnhy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/ghzhjeuuh.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gxasdfjte.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gawzgmivm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gqqhdkira.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gbvkxahae.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/givfemokf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gwfqwwmoi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gvlumptxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gryoeuhhr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxwoinjee.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gwbnoccix.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcbzklqzv.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gpmjaysxp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gckxgpwyh.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gutrstijh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/glbihezyb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gmtdjtcre.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gtczbnljp.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glsvlyyfm.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gzhdtscmm.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gavunbzeg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gmyqbyqti.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gticqtsvd.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gyqaybpsm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gwrfrhmbr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gcjfahlhp.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gydjffoph.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/grggpinwj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gbwbjchpy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gibietdqi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gvhjyaari.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gxshhforc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gtxfddznw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gmyvnagfi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gpbrbpmqd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/grlogejog.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gejnocqjr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggpkyrgti.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gztzuuoxt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gkkjvblrp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gldzunwsj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/ggzccsfab.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gmqqxmmni.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gfinwcjer.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gopyacuzr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzgguioct.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gweqvxgpg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gghrlucjn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gjnddhxhv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/ggciadhjk.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/ggkhdctur.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gqngizskd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ggrmmvgig.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/giabczikv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gnejigvya.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gnjyrqoyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gfahzmryi.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gxqvlzbks.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gptbarfca.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gqfercaeg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gdibfiwxj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gsvcznvqx.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/grxqslxqh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggtkoihhl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gblctanhs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/goclfrrgz.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gwdqyeaag.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gxxqelcyb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmeniigme.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdfskdeah.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gipxrsiqn.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/guwbilmeh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gemdswwmx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpfkwaxkv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gwqpfaxjv.sHtML


<!-- 参考信息 -->