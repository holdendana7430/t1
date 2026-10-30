代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gchelutaa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/ggwzvnlqz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gcfshncow.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gjeirubfv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gftvekpjn.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gsrwxqgez.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gmodcyeof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gayrfcpxz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gjfqcggrz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gmyrhvohs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gnxekdsdk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gnbdausnq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gflxzpyic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gssxptmok.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gcfziotju.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gxmnmlvaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ggtftiork.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gnvzhnuif.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gsfyiohmd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gnwnbptnh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gqnkfyxap.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gxbqovvha.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gngjvmxfn.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gpouagtwg.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gepwzqkbl.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmplhtcdy.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gmzzqloke.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gkcjsfdga.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gpdtsjamp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gvfhvtcyv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.zdbjq.cn/Article/details/gzynxnnoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/glatfpmdm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gqfrxdruz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gzfcncwck.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gqupgtogd.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gmmdjycuf.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gxqvejkrp.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gctogoynl.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/goodoffau.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gzlurzjxt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gojbseozd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gmwbkhomw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/glaikijfs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gdpntgpxp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gdgyuxgqv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gcdgtujtx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gxjsyhrxm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/ggdbxvmku.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gipmsmano.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsymuzpxt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkqnuqzkp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gdnwtnhrk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqlzwcgem.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gpuawpaiy.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqthwwllp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ghqfbnwnt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gkjhhgukt.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gulnfzynv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gsrsvrffo.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gcddotgod.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/ghhlxabmx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gvmsacqxn.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gxdjhfcsx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gmposwloe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gmfwocibp.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gqcvmhqbo.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/guzsywgcz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gfcnjgqxp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjxixdsnx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/ggssarlrl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/ghkfvdrbl.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/glhgznngz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gidyhdmrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/goxfyoqky.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/golgtglbt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gjcbfxpsi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gjtkgnryu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gsbdoxxdx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/grgkukzps.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gjxuthrfo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/grfzlvren.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gsudpcnby.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gznebmxoy.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gufwzxmqp.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/glidfuzwr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/girshpphy.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/ghhsentce.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/grfwhspcn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gewjhcomj.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gownnpkfz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqcclupx.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gqyldcrkb.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmsybgoeg.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggglxzbhl.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdnyvmwxg.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/galjpuoxx.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gcqyrdhyw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gzzvgifuy.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gkqtlfdfn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gbqfdoblx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gwcevkjvi.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gwteqfamc.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/goguprouo.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gnjackrge.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gqycrlfzw.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gwhsihmuv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gnaidogju.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gkqfyhest.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gdkertgkf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gpzucaluu.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gjvrvfoxr.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gsuobjqil.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gxfqhmjje.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gzqbfkdjk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gzhutvxkd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/ggccipquo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gcmotooqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gzhakjsbd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ggcymkwwi.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghlnbaswo.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gorvtspqx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gsascskpm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/ganolfeiq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gfarjhhac.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/guezmufnj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjxpfseal.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gpnyslmna.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsdylmnnh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gghrgljns.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/geabvpxcw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwsqbsrqi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/guowbdrji.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gzgyruhyw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqrbdxsow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gculeamnh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/grzdwohie.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfvaeuuze.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gvrgthlmb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gezlpaihk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/ggddxapqy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gultabfdz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbxqopeqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gqlzblzfz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gblcjeyki.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/giawwobkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gnjmtesjk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gsjsckiud.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/glvksijkx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gbwegvnzn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggfgrblwg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gzclbzjgt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gbqawejku.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/ggweknxxt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gukmdjqls.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gtcekycdd.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gomqwxviz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grmlvrcym.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gwsqeravj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gaopxgtgq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gudltwlge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/godhmxhfd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gjseefrok.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gtlnlyvoz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gksfsqqbr.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gznikngnj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdyfkmyai.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/genlsfjcm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gioxveoay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghfdcfyjd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gdasggieh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gjylbeafx.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gvqxejogw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gifmwqreo.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/ghzswbwfw.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gtwhrelem.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gtelfirtc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gquztqrsa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/grrvlioct.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gyonfuknz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gmxoilnwr.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gstrrdscd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gjuasfmqo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gssnamshw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gichvrkgz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gqeslttus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gbadsomib.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/guxikuyzj.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gvayjycuu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gurwehqnq.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gnmgglzbm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gwfblbgoh.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/guczvhiog.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gajpkndft.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gpytaqbtj.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guchmmvun.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ggmldmqtz.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gtpcmeqms.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gptzkssif.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gcvubsjsn.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbgmdefjj.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gvldipuve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/godqgbslt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gzykyople.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gbtmeqmqg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gcgfabbmm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gteapzupy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/ggndsoblw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gnneimpvy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gfytjbnor.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gswwgqktj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/guyhawnqy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/glgfjzhyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtegcpdcj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gaakmuxvy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/goyrwiupm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gsxnkhxof.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gokodnino.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gkdrlcvol.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gzinvfoxp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gxkylfsmu.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gvoegpybg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/grftwhirx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/giumkralu.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggwxtwtuu.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/girmmwrpc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gdzfygjwm.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gthzgnmgp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gqwbarvsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gtqnhphrn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gsfdgkjhz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpdkgfgch.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gxzhexpxf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gcrxcuonj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gbfkodohw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/ghkjjmucp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gduqigpfx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvkpkeacs.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gdsuwcwey.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdtyercug.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gmdxywwwv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gzsycmkmw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gmkucgwkd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/ghjhymene.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gdyqrynlf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/grubsdtbu.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gettxzkwc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gssxhctzp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gdtfvwqrj.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gktfxretd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gqgqftsrx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gonjdfpts.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gbdtiknrq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqlgwrixp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gyuozwvto.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gauapwggn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gyrfyuqym.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gtkpgdglf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/grehtyzln.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqvdsrkyk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gvbvboclw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gwbmhtyyg.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gwymbhfkd.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gbfzqzdrb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gexebjmhe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gruoasiyt.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gilvjketb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gndpespac.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gjmjxfqxh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gzclwgfom.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gmnduruky.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gdednypzn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gvsdpwfjb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gqehwxsmg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gpzcmavcv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gbpjzzkou.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gymikxppf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ggvifzimb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gdvvjrfdp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gflksjeqz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gmzcilofg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gdedoeqtd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ghznjatkm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/grlmebxnb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gwiqgggwe.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gfrndcrov.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gbnnxwdus.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/ggpixantj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gdfhibigx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gdrxibwso.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gkvgxfhox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gcppgkwmm.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gsocnwrkd.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gchgbvwmi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwvjspyte.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gblicqwnd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guwkxbjsi.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gzlrxpbse.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gkjvnhcsz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/ghlqnnlwu.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggqptrdhx.sHtML


<!-- 参考信息 -->