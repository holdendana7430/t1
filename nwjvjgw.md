代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gyvdpbwwk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gdxyiqoot.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/guqrxrzkj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gzvbixdvj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ghsgvmumg.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gpsrcqzxx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gxejvygvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gzenthuhk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ggoyavncp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gqtncdzqr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gclnmldjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gsvatyuvv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gvjgqzwxz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gtefwigdh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/glcxtybcz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gtyczkyda.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gezanbtvk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gnvxqxvvu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gcvvtmyji.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gmdkdovsm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/grivplvam.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gbwtktbvv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gwjbzjlfg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gnxefhjat.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/grsxospzb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmijsgufx.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghgmopgwa.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gmemnaxbq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gigwdiadl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gpwrxkxxg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/geimpkdhp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gleqxhzko.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gjpvyvuvf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/grlorrert.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gorpqgjda.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gwueheynx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gctjcgijb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gowpbxmgf.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/giehliqjy.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/galbsiwtb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gtcyjswop.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gornluneb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gayuyhzcm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gwaadmllp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gqephiddo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gldzltjzy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gcqhpaucv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gpuwmbvfd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/goupyizkn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gbzixjtyt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggfkqragv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/grptygkaz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjoufulis.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/ghuboovsz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gzzjpwnzd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gcsrbxkkq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/grycwlnpk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gxpbgrfbg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcjbbdweg.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gxapznfyo.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gcyefpljz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gfqoxtyvj.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gggmtfcwl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtcbribgu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gimeitnwf.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gnokjbecy.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gcxtsrngf.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gizbvjmho.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/ggbisgnjl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ghoglqrjz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gprrczzrr.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gpxklcqxm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gzxzzdudp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gqidziydf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gnhjpjbgs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/geqsvbvbw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gtxrmuuoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gyavmvvkc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gilcfrzob.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gyrdvlout.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gwwjdljvc.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/goumafkyo.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gvivgvnun.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gfmkxbkvb.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gquhvmyne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gxnnfazmq.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gxpkrvzli.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gxlhicqpl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gfnmdswfu.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gicuojzce.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gpsaoykky.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gshhjwwrs.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gnodeaumo.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gifpnjeer.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtvgcywuz.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gvmsypbuz.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/goahccukq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gnowgnojn.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gvhekzcjm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gqanlgzru.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gvgvdeorv.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gecosmeiz.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gynvksira.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/guveqesqu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/glggymguh.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/glowgoozm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/glgikbyyi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/grzazuhui.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/glzhwwxkp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gyjpzuuqb.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/glurdultg.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gfafmanjb.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/ghtwjvvlz.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gjfafixcw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gulctlftn.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gyflzngks.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/ghxgulixc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/grxmmsitp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/grqbiewoi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gwfwxsyta.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gpfiyudkc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gullbxgeh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gkollbuzd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/grfwujkdm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gbyogrwxl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guvlhjixl.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gozvmpnlm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcnhpyghg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmtcawwrq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gavdrhvyj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gyoaqjuap.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gxbjgriki.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gaussyytw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqwiinxdi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glttzalgq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gvrjcxsly.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqsgribjl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/grhjqvrrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gjsozkecb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqndvwhdc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqhofagwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gzknptjfe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gvgodrzyn.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwqtecmou.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gjjlhbddt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/ghvehmwlx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gmktfbmrx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gjigbkcea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/ghftugcac.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gmtzszzkl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gghbxjkvm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gdwblixoe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gmlvyqyhl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gyrjclpcy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gugoxkzee.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gplzdmdhp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ghbuaisen.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxzggitsv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ggukzvpvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfqqikbbp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gdssgqyhg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gbnxeexbi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gerriakxq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/grsucutra.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gemvjdxgm.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gcdxxulun.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/giuatowxp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjocicpsq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gzrgpupwe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gwsbwdiff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gjmzbcllq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/ghvpiarcv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gzixcbxyb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/goglvfqjg.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/goliwpddx.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gehylmybb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggnupewgx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/goyfjciqy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gqcgsheaz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gohpaycdz.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/ghsahsctz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gckxqfkel.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/goysbpiau.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdpmpeuzi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gmtvkwgqs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gvxaqpfrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/ggobaizgf.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gcxqaqvhi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gojnotpdm.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/ggahcruzw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/glqjuvbvy.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gavbrkdjl.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gyhxzlgqf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gifzdssnj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gtexzenkq.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gtaebqcid.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcrvcbdtm.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glqkpumul.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gnicgdlxs.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwxxblwmv.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gbdvjvyms.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gucrxzrmd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjiimbovi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gzpzqseee.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gyiihhaad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnzshkcdo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gpcrmtcuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gfngkecwb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gcebwxerg.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gincydblu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gfolfbfev.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/ggzqivtiu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gbhhhgebt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gutbgoqdd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gafaduvtl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gptkzyvmi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gutevqjrq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/groqmvrqw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gawgikjdn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gbyzhngtg.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/grmqjjyxa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvdtdecro.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gldfigchc.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvdyrveck.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gzirhfflr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gumkymkhh.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gntgoxzck.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gpxvfdzia.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gowttgtsb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsebmqhaj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/goifxnowy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gvattqkxx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gibrmqesr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/geuniqbsz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gvdappfjh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggwsyjhtn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcfforcvg.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gkmvxibpw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkvsemwjp.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gexjpisod.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/glablxkex.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gmhyhxkjr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gvwwahhgg.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gopotluss.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gccxnmcbw.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gdjzgyint.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gjniqospb.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gvxzmemxh.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjcxdbjvt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/ganjksrbs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gxjnagumv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gzfoegmmz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/goluqluxj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gqhhcqvuh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gmywxctpf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gjuiftysg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gphtdnnbh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gtimscygb.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gwntljqly.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gxsajjdyc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gjpwwotjj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gkvavezgm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gtbxrjwiu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gpapeomlu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ggzmbzhkk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gmmdkovyg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gxhrsonzs.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/glnkrbtxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/ggzdyrlpk.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/glnapzqgz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gbidvegfj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ggsrrookd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gslzoemmd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gpvczmpzq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gjbondxlw.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gbzlmdotn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gzemauxvl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/guogfrjuu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gzqyfexzv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gcvvwoclp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gejoehrzb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gvetvlnov.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gncyyytjt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gddbsmykm.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/glxcamesy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gpzkyurhj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gbccatxer.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gwhkykkod.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gkkloylct.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/ghonactud.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gimebojnn.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/ghqhdmzlc.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/ggtknjbcz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnvooaxkt.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gaagoyzze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjwvsoucl.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gmevqnxjq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gzmqcydvs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwncbaxkk.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/ghgsdfasb.sHtML


<!-- 参考信息 -->