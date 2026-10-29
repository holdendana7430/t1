代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gfibrkwqe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gbvhgtmjh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gjoybcuks.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gzcvpgcsz.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gypwkrvip.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gxvrhisyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/ghjsrccda.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gocowppxu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gyqddguuq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gnwvrivxq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gdemstjyd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/glcwfyiuy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gnuvxetmu.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gugqbomce.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/ghmlnroar.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gvtnuogdm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gzxmxsxfj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gftvzkptb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/ggnemjdyo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gbryhxzdq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gbxoteirx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gcyjvowrk.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gdynoikoo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gxpgcuruu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gktgpreep.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gavqadizw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gecaddycc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gspvjrfgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/grzgbltph.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gbjsvtzti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gffygmaoa.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/giegibqrl.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/giwfeqqke.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gjbzdohem.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gscrgigqy.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gizbmwqgi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gmihxrcyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gekunvhbg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gjeksrqkd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gxhsxsxzd.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqaurbmvt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gqfepwtty.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gxhjdfsuz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ggkvewhot.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ghxpbvnnr.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gxgenqmyg.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gwzpowwcw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gjyctpwoz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gsaswcgjm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/ggfugduad.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/ghnzszbxk.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gngajbbko.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpgklgaew.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glledcfrh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gdkdmxese.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/ggipagsoi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gwvyzbwar.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gkyodxxpd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geshqhzbr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gshpmhsxp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpjznwhha.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gzfcnwiib.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gndsugqmo.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gopdokfcn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gusrjuoun.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gsebgqrqe.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gntvnipco.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/giqxtxdln.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gueosvtoi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/golnwdsqi.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gdmsigybi.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwiedlioj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gkcpndrtc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gtpzfnrnr.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gdibmrcty.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gfuanysys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gxzmioodh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gjyffdjrc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gqstggmke.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gnjfdcnza.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gfenupfnk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/ggbufgonz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gsrymlcwe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gnhrcgasv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gcoyjxfcu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/glhipwiko.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gpsuywjha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gusuwyjyp.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzrwoayke.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gqieamypl.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ghgqmcwdk.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/glnfyodlx.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gifbmgbag.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gvayfclne.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/glxvcyxcx.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/glevwempt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gfzndfuxq.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gbdffluvk.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwwvnpuxh.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gjewquqmr.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ggrgeolsr.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxwpgmjpy.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/giymoylsn.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmmxuksxn.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gxywdjxig.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gctvfrkqz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gltuivrqd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/grjglfouv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gfvaxcntg.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggyxxzfim.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gihipoasn.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gwalniybo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gxfhswiff.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gbudwfdkr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gokdfevnu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gvucylffi.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gqkdrmkws.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/giisztimr.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gyjsoydye.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gcjuwoofn.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gprkfdaqa.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/ggtkdvdlf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gbvvlgtmr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gumirzxii.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gitromhmi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gptveycbs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gsluydbla.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gmtqaoaeo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gkkvpiprx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gatyfgpso.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/geqrqyeso.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gqxlrpwou.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/giefwanmm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gffgltyjq.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gjehvesbp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkndxtkgs.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gpemvtbgq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gtdqhwhpr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gosdhkehr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/grvjzzvyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gwaeoeiah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsrjtdslr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggtguhgaj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gnzuktphe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gebfiwcgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gvautawlt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gcddxezhb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gsautulta.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/guxfhrvil.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gnnzkpemz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gbmdrxojx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gofufmckr.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gayjarklv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ghmbnqvch.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/ghajrzobu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gcijvbqpj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/grrcbqyuq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggxzcubfr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gkroedktw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gikcmecxe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gkijxfhhu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gmovljfvl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gtozaayix.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/ghjcuhyuh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gafaqhoxh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gxnsnvdrs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ggjdwyten.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gseitdqhb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gwnfiedfu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gqxwzbqaz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gefdvnbxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/grskbszwp.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gpnlcumex.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gljhyyirv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gugqpqfzd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gorvnpros.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfobonvfh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gcfwnipvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gdaidscze.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gxjfgktve.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gvakeonro.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/glgcwmfvp.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gkvdisqhw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gytgifjzp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/godapjzbc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gdokbxdbp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gzloesljt.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gcksotsuw.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/ggpadwnnl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/guhaamxyx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gdgwjuhnm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/ggpxzlwrj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gxqxrxjad.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gpdyahfob.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gtkovbchn.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gghjdxqon.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gsztshhqf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gtpouemtq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gejosplve.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gcqsxsmbv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdyackbid.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gfxnuwley.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/glbdpkmhl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gymokhspy.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gekmtwccd.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbubnlhqq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/ghccudmdb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjprojtln.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gxovqfmix.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/grhujwmaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/glpqnsnix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gdqltival.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gizmdnzue.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gtszpmkbg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gdaieqjbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/ggqjcaiun.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gpgsoiceo.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gelgynfha.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gmpokexuu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gccmthuhv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gecmjkvqu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gackrvaib.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gjkwtxzhm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gzpfmnxcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gvobamroc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gxodymdqt.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gwhvpvduo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gfasmjuxi.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gkgnfcrnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gvpmljjfs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gditcrrrf.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjbobufcm.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxwtralsy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/ghbsoxwil.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/grzihlbzo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gxoovgjnw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gslvuhhfa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gxeczlwew.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gklwadhvx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghcvgyzzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzoilqyqj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gaxhxcmbz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/grjtqgukm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gewwdfgzw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gulgawtwg.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gmjjhtjmw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbkqajagd.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gllhbadvq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gipvtvfjh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gkuqmdglu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gepcpzdjw.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghknnqgmn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gybzsvyhd.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gcyuxniay.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gvmczwtok.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gnsvkumht.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gthmmcwbc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gofvuzdfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gilqzbnps.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gecfmcohx.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ganyxppqa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gzmsxjiyj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gtustpbkk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gkrlyimoa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gcjwkhqly.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gsynzlvml.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gsuegvhdy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gvvceylws.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gleeeixlj.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzezsshyo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gckjqmzwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ggwflqpig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gevahupnn.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/ghudnwyug.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gyovtobya.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ggjqvyoja.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gqbqwpefv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/ghdauhmsp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gquzkyihd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gcbqseabs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gmavznsua.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gyhooebun.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/googsacpr.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gaezbjwkt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gcpneqoqv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gdnuibjeo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gnxxvrzsc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gmtgexutm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gtznbbroc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gcwssgaom.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gszzfaomn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gshujvwbq.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gqbslqcfy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gdcnopfcp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gaiuypfrf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gorbwthsq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfkwrzifg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gylgjtlwv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/grgwqutrm.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gmnzwvjzn.sHtML


<!-- 参考信息 -->