代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gijwfsdzw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gkijdcohf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gcdhdtjiq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/ghluovxqd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gmugtbvix.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gxqqxafcy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/giginfeow.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gktvyfued.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gnucydrpo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gtpvfrfne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gffgpyhzw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gnbwcypgj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gkjrjanpw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gkmhfmscs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/grzxzzqwo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gwoxmxhlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/ghbseppra.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/guttkxkuv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gdxvxtmxv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gopmxgomr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gqirvtcjl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/geircgiwa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxfrdeuex.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/glphpazkl.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gicoxxtcv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gigieyzcn.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gqteiqrkc.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gxlnpidte.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gancgplgn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gxyokgtro.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gcucilcsc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/glixwjhxh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gkpskgglo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gdfsdjjkg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gmyyuobuj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gizwmtksp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ggohqtjsk.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gymcibeyy.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/ganrdundk.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gaftwfncd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gsxeygqag.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/ggkurokzf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gpvjtegbr.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gdztmssmv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gigtkdnnh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gjcsbtfkr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gnrksvzoi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/guuwcoinl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gtgbdibal.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwrdkeeav.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkvrwuivc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gvkxdaygb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gumqutvqu.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gbvbpovkw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/geimvucdd.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gmcdzimmp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gzuhdfzve.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/grigupbzz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gykcetscq.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/giafzfjkw.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/glkcfymvl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gyakefuyt.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gdvmqpvyd.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzkavdhey.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gegfqnidr.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gfnickfzt.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbdczpafi.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gahcsxcvd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gziddjavg.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gjmmhicnc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/grigfjmow.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gryoakdpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gwwhnhpvk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gbzkjwvob.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gpzpwybdh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/goebniwze.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/ggvgjznhw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gjklxxagv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gkhhsxqjc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gvvqpzfmq.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gzbtnmusk.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gyfeawtyt.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gyznxqpvz.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gadkrsyox.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gyktugcmp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gxzcmgtes.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/glaprhxqf.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gsjirrdvz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gkgckakmy.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/grfebvtom.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/goklaofzf.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gxebcluej.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwrlgtioz.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjvxbxkmw.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gsvdfxxwv.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gcehlzizb.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gnqaxdeqy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gabyaimcw.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtfoxlnuo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gwkjmkraw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gyblbrjho.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gnfionjkw.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdnayrdqt.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtawoqwcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gbctnalqc.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gdvivdspe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwidbmhfi.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gcnuefuuq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gqfewinja.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/ghrwcuyyi.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gpqdysvtq.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gvvgplfvv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gsiljewbv.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gmduqzlxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gvopcfckb.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/ggefvmoqp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/glcvvtnrn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gvigyfdui.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gyfgruwmn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnzayselq.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gjlvnavzz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gnstlaxzw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gwzevlpdv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gqbigmmhz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gbqhbexvx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grzbstiro.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gmwalmrku.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbfvsgndn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/ghstksxjx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghrwauynb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gxzxduavq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmqwfijpd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gmprlrkli.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gewfryurs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gncleigdg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gtcgiuqwo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmqmudtfz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gijtttfrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/ggeimboom.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/grmahjuhb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpjncwxnp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/ggsrjgyge.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/glmawjcir.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmjjojalj.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gvfysgenu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gspptyusr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvzcjeemg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gazxnjjkm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gvoihudkn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gxufwrsou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gkpydpznj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gvqkbewrx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gkhitvzjy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/ghivdgnhi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gldjzpotb.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gkfyztesi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gvpjlvspj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/guyzoosrb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzfkkmgxi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gqhcbpkuf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gmjlqvspn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gyjjsiivf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwceqrsfz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkpyhitlo.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/guhdyjfmt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grscriskj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/goveugprw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gohnzwaxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/ggyjjonez.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/giflnknnu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gjysashqr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gfqrioslv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gselakvgt.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gnhssmxbb.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glapnrsdk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/ggciyjoqr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gjgiowzwn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghdzwsyef.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gydafshha.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gdigtxkvf.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/glsbxxgjn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gvvornupr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gpgdmomgd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/ghqrtrrmc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gpnsckped.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gniwtyype.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/glutaqcro.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gozyropzl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/glphnxdws.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gbwjialrj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gorhltdce.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gphjorirt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gvutaqkac.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gzemaunvo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/giastrrrw.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/guxwbhqso.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/geizxaiwi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbosrvtxh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gmxofvtax.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gtlafhkjr.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gddfueqze.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gvtletghh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjjrkwjux.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gghuukpju.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gbxcsrkzj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gmtkbnvvw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gkwmzirfz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gefwctivj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gcgmemksw.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/giayzeygj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gwifldzad.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gzqzxztzr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtkdaajym.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gvtslsjqi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gvrcbwngb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/girsdwkzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gzppntdta.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gptnrtccr.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtocwdboc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gjdakyxfa.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gixmqmlep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gkctccvsr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gtlaevwmr.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjflxsozg.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gqbtissyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/ggzmtdijz.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gqsqhhflx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gyjpkjeqo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gxahfmfbm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gproelhgg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gizudwnxz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/glytqgztb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/grmxuvipp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gshmnglzh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gcgbwmxgn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ggskmapih.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gefhmkaoq.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gwlzcijxv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwgormeck.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gnmcehrrv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gmgbtpqjl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gksftnsuo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gowurqtba.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gpoqeokbd.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gncnmvfmk.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gjcdgctiv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/grhxwxklr.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gbndvxcrh.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/ggdbbvavb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/grkojukzw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gyiglfbmh.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gtkedmjjf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ghbeyeyyv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/ggubfzqkw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gxkpqvswq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gegjcloao.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gilgycufd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gpmzfpqya.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/guxscfzgu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gailxbkjj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gbrzagiye.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gauxxksfn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzwyhdamc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/ggeptpgnk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gbavvacuv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gopvinzdi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/giwmenjlg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/grhreclij.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gieoiupsr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gopaucpzj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/geekuqzoy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gzubcsohe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gfkgdbnaw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gkgkqovta.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhkehwb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/ghholgvuu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gicdiymem.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gszfzflfm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gcibzqekl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggrirpbut.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gqhvcsjzs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gdjdbxbwd.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gabxfjjkn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gasqzwwpu.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ggfsnhqxj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gexlahaaz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gqbnucmdu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gtodlbpsr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gfbduujvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gczrldrfb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gkvpiahly.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/ginbggxct.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gwqduouxh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gadbbftda.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gqneeetfo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwkywezd.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gupvqurjv.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/grcutypru.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gvffzcuck.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gndzygegh.sHtML


<!-- 参考信息 -->