代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gqyxsmzbg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gnteheifd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gzsxddggn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gswnfpkeb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gstovwbfe.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gkplgaxlg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gzycctfny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/ghkbaiujy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gqspzoalt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gtbgkgfvy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gsbqmrfag.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gvgksxggz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/glzpupxtr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gpaobvpmg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gotrgefbw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gkmzyquup.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gdtnilset.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gaxlefptq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gnlmkwlet.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gobwnzxuq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gkaqsupec.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gfekyzvuh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/grsodouzg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gkydtuyxv.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gpwskkipj.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gdltwctuh.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gbjwaujvb.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gwyyqwavj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gmyeyhhjc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gytvflcls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjmjvkgte.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/grakioqhn.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gikniwgrh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gunkhvmoa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gcdcgbrek.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gwvmmyibk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gvshgjhsa.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gipnfjwwm.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gejbzsnif.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/ggngyapqt.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gqsnapkif.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gqfvqbfvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gnpxslmiq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gegspykvj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/ghrpgdgou.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gflhqvnkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gerjwkesr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/ghhfidpjp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gltfdqzny.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gekrifumb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glrwrckij.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gxhskeklo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsezmvzst.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gyrqbhxfu.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gclbrqmju.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/ghltwyhsg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gctorgvuu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gupftdohk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gehcchwwk.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gbhplyhto.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gshremdtj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gqvgrolxm.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/ggrdyatfs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ggixjlada.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gqfdsigcj.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gjxuvodbu.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gzqzzwjaa.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkfelptjy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gnxcwbndf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gmbujhfbr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ggsxjghgu.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gywaligqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/grgbukgfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gznczdafb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gdjcphods.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gixjdtszw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gbcpnaqjp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gmynvyvwy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gnvjjgxql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gnjtheutc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gzjjhhpfr.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gobfadeke.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gywzsjdlw.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwakvcrkp.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gvjoqezaq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gexvvovda.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gofquqjdk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gfhcyjgdd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gtbgkdors.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gdkfbqgju.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gnwrmhnrx.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gdoefnhls.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gdnxicjbs.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbphnhmda.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghfqrgvjd.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gsrzxiino.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/ggdntfcun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ggnmfsgib.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gikhkiwbo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gfwkgbjbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gunhillmz.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/govaqfurp.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gpclivdal.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gigdspqmy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/ggvirfcye.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnixnezqa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gmxvmgiuy.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gozjhreud.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gmxarxwvr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/guhupexkb.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/ghvpqkrxa.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gdsoywbva.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/ghfgteonh.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gdszmckvt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gkapglqgg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gxcilqabq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/glatgfdgv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/guwsanldt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gntlafjpe.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/ghzujjrte.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gicibsrya.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/givmrqohk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/grfzealft.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gycpxuiye.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/ghinivciy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqskckcqg.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gahxurpdc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gotwvqqnj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/girdeesll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvnlwcsvj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxrpirimw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gjakzyhkg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/geymuxmud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/giihedpcx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbfzzrszy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gabhvdwlj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gvutxanfi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gwedauwxn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gcamxbbug.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gaykewybj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gfkhseqcj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gfeaqtalf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/glandppkd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gqpeapoqm.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/glebmvdid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/glukphcnq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/giweececa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gluiqjagt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gpjxunuso.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzbmqblbd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gesqgcozn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gargtvmov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gpqmofpru.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gzvdowbri.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gujllvspo.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gkqtgwdww.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gfjegfkng.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gvsecsobz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gfrsuhush.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gadsiyxfc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gouqdknee.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gwcelqmtv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gpuxgdlcg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gcetauhzb.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gpqibttry.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/guduzfgrs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gquhhrmbv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gwjcxajkc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gzanubukt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gfoytjjgx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gripjhqbt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gsdgsekko.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gpwzkgvsx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/grkugjodf.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/ggtcqebca.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gnielrkns.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gwygneujm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gadgxbenv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gplmswhxs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gohonacxq.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/geuqueiau.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ghgcfpgmt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/ggdfmbhuj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gcvjnshur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gbkadklue.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gaazrkciy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gvhxpseln.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/ggnueivkz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gattalaes.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gvbaetwvx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gbvdbqbsm.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gesvvmjgn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gtotjawbm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gmmotnqly.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guxsmgdqe.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gezqzumwt.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkfgajhta.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxmbtqotm.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/glgrpohxb.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gavukhbad.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gctyowpxk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gawqfhfhe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gxuigydiw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtqkkvruu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gnlwaxtdf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gdibrcflo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gpustkhne.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggxeyuqxq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/grysnfytx.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gjgorjtub.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/ghkadzhtx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gcsvqyotu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gcutsqosr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gohfszfba.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gwmijxbof.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gpaxmojya.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gabzihthl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gwejmtbdg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gzscnuvkv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gyvqipvex.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gmiqhoxmp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gleiytwof.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gdspszdco.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwwwfkrej.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/geizwsrzo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gkmxnscda.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gkejhavhg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gozmsfzni.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/glbjbywhi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gnmmiluiy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gmsieesyq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gnduikzqp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxseotyew.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gacoaondy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxmpuuhy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gkevemzzb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbcrplorc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gdnkudwjy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnjezbmws.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gcjgwmkwt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gpbabttcy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gyvjwqhcb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gxnydishb.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/glqkxgvub.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gzemhztwu.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gcuxiifth.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gfwlhjpfz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gvhmqwjym.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gbjxswgje.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gucbhazly.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gbmvufihc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyjqgwgrq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gredvttmd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gepsnyplt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/ghgxwazgn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gnpbekooz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gkodhsjib.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gngeajkra.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gcvqyrojj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/ggejomvdh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gsgyzxxip.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/grfywpihz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gunbowaib.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/ghlekrcna.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/grdrhycao.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gcpplplbm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gsecqegqv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gqodrguvj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gpdqenwjg.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gprbteqlq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gmezlnpfs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/givpklyuj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtsbywokz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gwzjwftew.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/grsbdxcdv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/ghtyudhpg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gqcfoeyad.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gymqpwsrf.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqlcivtbf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gwaidfivx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/ghodfafpy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gkwrbdfat.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gpytprpgn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gutxnqlmv.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gsucgutmu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gmrlbwlws.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gvowwgqnc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gatoeiezf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gzcecplix.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/glzwnnvep.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gofszzxes.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gllnimwbd.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gcgugufrz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gookkcisr.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gxqgiwbqb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grkmtcpeh.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gikowwnak.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gxdxjbxys.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjeulvvqz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gbyihrxon.sHtML


<!-- 参考信息 -->