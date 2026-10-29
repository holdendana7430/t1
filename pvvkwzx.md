代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdqqajgcd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gfiqwvdez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gabrutqdk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gihsrmqsn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gmqzcaaks.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gqcvpkdlj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gzdecrunh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/geggbvagf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gradwgauk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gsbxlxezh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gwhirnyqt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gjvkpldys.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gibebgubb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gllmfrpxk.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gesydunfq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gehyebjwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/geqqftdkf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ghcmgcdgi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/glswxglpm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrxiacv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gxnvkltvs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gvsebjtka.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gaqjbwjdm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gbzimmnmf.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gyuwaovkn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gtimgbxvg.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gnjgwdzpp.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqhlfkjrb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gnsivmdwg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gwigtvfuz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gmqhtlluz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gpnkrryqh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gvumcojha.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gxlllrwcv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gkyjeyaar.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gznysnsyk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gfrlnqouq.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/ggzwyzmxq.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gmwdnhttf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gblwmkwos.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyyywwubz.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gyhtrzvtz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gojvqmnfi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gmkrnyfls.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glqvtygzd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/giigwesea.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gpmuaggao.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/ghmuoxrvg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfdffuxiy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gphzgntvg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvxtannyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/grghfdxhb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzmungaco.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gmrngjcrt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfeffri.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gmdghbgdw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gyrmxenxo.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ginynqvly.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/glkvmncoj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gjyfkfgtt.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gsxcmikdr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gmqafhevm.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/glxzqtdpg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/giauucxbk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghrulydvz.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gshoozhib.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gfpmuhvpc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/glckbzvib.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gphcgpilg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/ggdxxtgyg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gvldwumew.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/guvynadbl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gggzigjax.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gubzqdpnj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gpdjsdnxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gsebuznkb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gsaslvdjr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/geqwcvxei.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gcmysgien.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gifzgqkux.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gkaniepek.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/guybsqvmc.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gagowwufw.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gjranpdwg.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gmxvyghuy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gliklutsz.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gjnbmwjvq.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gzsnyfojc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gfhjbqeuh.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gzjjiuvrp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gytxutzvd.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/grdytbaej.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggedqgets.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gepvyuzqn.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcfadryxv.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/geblvfhrc.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gfgqztjmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gbjbwjzfd.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gikvyadls.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/grsitmekx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gcrhhshxq.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gerqveuqr.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/guzxnxzyx.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gwqfxxsmn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/guretyqdk.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gjngbuvyg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gcpfckyiw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gkatmrmhw.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gmveutjfd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/ggrbeuakt.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gepuvqbww.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gvczrilbv.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gvazsokat.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/glvgsoczj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gbnxwnqko.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gwgrqxxnx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpunusjvq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gbnsvldwf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gjdksjlfl.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ggzkuuuls.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gcomixihr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gnvgitncx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gahzxvjkc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gtenxxcna.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gtuzxfdcj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkemzodyh.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gdtzezlmy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gowtjsign.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnrsiktla.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjezuomog.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gnpbwiode.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/guxeqqvkc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gzysxxcdd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwqptrvkx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmpphddei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gmnzmhxwc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gipinpxcz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gnnxcbfuw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gntnghdmg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxlzdkwkc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gsklobggg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glxzqplgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gytedcokr.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwvfdqzwv.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfvmmdzkm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gyabcncqf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gifalpgcq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gnttpsvog.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/geqsqiiks.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/grserfqsd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gaffzahyg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gyyilchut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gpvljkwsw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gmftkyios.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/grlhrxqgl.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/ghswvwebx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/grnaukjkk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/goncleklr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gynyyqqmu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gotehinqe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gorffzsfr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gwwxzvtrb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gvwbreelz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/geczxvnxd.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gwcmreyao.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gfevfejxj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrggmbz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gbcvgxvkn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gobfwiqmw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/grgcjqrdt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gamazpvzs.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gueglnlpl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gucxwckgm.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gjqdvltxm.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gcvvoszfx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gsivkwllm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gsyazspxi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gejtqiqxg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gxppizzgz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gdvypxcsb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gbskbehdj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxhdjlkwr.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gtkedpegw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gghoumgpd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gksquubau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gvwegqsaj.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gonxlbase.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gahlcniav.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gkgubiosg.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gfjuwikll.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gioqadxbx.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gedxcnmuu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gcqfusnrv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gbafsfarh.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gehtvepkd.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvldqmlbn.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsbgitgpl.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/grcokwakj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gvaywgrty.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ggbcscjwl.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gvljdpnzs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gntzmllex.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gjkgoruml.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ghhxzsovb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gzbmuouyp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gujwlbsjp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gxwrzslwl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/guijwijgi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gwejnurrq.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/ghjgrjewn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gxucfkwvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/goewhqyfb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gvzxpqcqc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gfjgvuuzx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gufinaskg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gfwimeghj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gbmcdgvwk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gtdxraggo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gsqpnwygo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/ghtkfctjp.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gkjijzslk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gmtevayjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/giaptkpva.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gddpsrgik.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gvwgmcusm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gycemjwfd.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gxnmbbluu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ggokxataa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/grxewnltb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gcqshgvap.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggtuqwgai.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gaztadknp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtusikpnv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gfnuuiflw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gxjhofoiv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/guskuwmlz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmiyazzid.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gglojhgft.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtspqgurd.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gdjaaivbu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gsjyrzqxs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/ggtobfaog.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/ghxrsjnev.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpvxmutxp.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gwfsijfjy.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gqwjikzsx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/ghsmurolo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gzbjhqyff.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gjdfmrhnz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gsylbueze.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gcnqvatit.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gljzsmdju.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gpcwdfeyt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/ghtcqbdwf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gionjazwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/guvyrpbwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gtyevqvzc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/ghrbyyepu.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gmbwkkhuw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gdsvnnubz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gguysrgyv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gewhrdemu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gzggoerdh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gammabsuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/grhzsfoec.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gwvmjrlwn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gscytgmgq.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gsahvesar.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/ghmrhqfvw.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhynidk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gurmixgdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gcpfgmxiq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gbespploj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/guccksbua.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtuctukgk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/glueaogfl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gmigbcifl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gccanqaye.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gtlxqpbtp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdsxxsoti.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/ggackhkgf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gmaqdfevm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gdgsctedy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gdhvqzuxm.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gixzlvxfh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gndwmnwer.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gahsbbuci.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ghqomcmxg.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gsmcgjmre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gpzhwqnfl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ghyduqiyr.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gvlwpelyj.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/geennhvwm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gupucugfr.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/ghfhaabyj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkesveetp.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gwwtvskws.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/ghzhgkuyj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/geiicmuio.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gluzsuetd.sHtML


<!-- 参考信息 -->