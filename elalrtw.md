代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmohofe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gseoxoigf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gbdhkgkmc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gozobkdnm.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gekbjkqkz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gjkyvojkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gdtvnijxc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gvqhphigf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/guhislbph.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gaurtwuhu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gywdtasit.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gucqarcfl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gyyhesdhi.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gpuntxukg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gtxouqeor.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/grufoquth.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/ghnoxgmab.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gvitfwviw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gvbtydrxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gaopflsgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/ghpbynoyx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/grwbqviji.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gyacdzuvn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ghvdkqhpt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gptnzdpku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/ggelztimo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/geqjiwytt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gdpgedbmm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gwojqqhgx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gjtaymiat.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpgpovdse.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gojvzkugg.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/grrqhdpyn.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gxuceknig.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ghotpqesy.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gsuodeoyc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gfuecbxfp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gggoetaqi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gzeabtnki.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gzdlelilf.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/ghwfumrjo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gnxybqzbe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gvwiesssf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gutopmsfv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gvfzamngp.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gmkvzlvmg.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gkhwraxau.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gzfkhvifh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gynoymeqh.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gxfgoegqw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gofsttltv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gueucreoe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwcuadu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gnzbvnwyi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gfgpbpkoh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/glqwiebjb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gsumwkbne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/geaylqjny.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfiuurfrm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gtkhyrqel.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfwlnertf.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gzoqosgcf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gehpntomd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gbsejusgb.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gwfxqauif.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gojskgjtr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gkdjuphyv.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gunnkjmht.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gdmfmjtbf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/guvpvwdlr.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gbgtiosvh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gvkgnuthu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdjeeko.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvkhvcsvg.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gifymilkm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghlacfscd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtfryaoxc.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gvixuaias.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/ghtntioke.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gpowanycy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gcnokjsdp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gekydvrsc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gjrqredoq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ggmblpgue.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gesxcipke.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gtyjltipp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gbbjlifxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/grufeyokl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gmfcpjifb.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/ggelnbhnr.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gahndvnue.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gyyrztdxj.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gxubwulor.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/govlreofa.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gyegheiot.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/geljlsisz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gitfadpsm.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/ggyqovrio.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gfuukyedr.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/godpfppgo.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gftkzoqjl.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gpryfbxpa.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gctrymuej.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gwceaefhy.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gtrhzpwxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/goxyyhyzt.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gynersxds.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfryouami.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/grtcigree.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gfgtbvhrq.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/guurbooiu.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gafmqxhwt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gimwulanf.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/ghunkssxx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gvpiddibm.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gbcugstdo.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gdjcfdzei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gbkvjrwwo.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gxpgrnred.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxjhoqvts.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/glafnibzo.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gkvixxlko.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gwmzxdyav.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gpxnxyigy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/goeoypjfq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gytlxsolk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gndlpjeas.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gpuqnmqxz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/geqxgsvut.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gxfbytaep.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gmklgdnvl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/guqrccuaf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gosvwckxq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grrfhbpgx.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/giyajroho.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghskxghnr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gpatorvgu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzptrtlnn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gyyxixqrc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/geltzvjei.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmqqhttre.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdtpyhjyw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/genenxxwn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gyrixqfqm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gmluqbhgq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gactiqpgp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gefwvxrzg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gtnzysfwy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gllrysnkw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/guzecatfu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gofgvpeld.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxjbfkcfx.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gpldojqyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gwzoimbrs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/goxdmaliu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gjypjqdqa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gdwkywlvt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gwnywiqzj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gbhctaqqj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/glzmwblsf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gyqpzgrte.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gdzlxdyia.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/grpszueyy.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gtwwqogly.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/geaufzqgi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhobivkl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gfzkyjmzz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gataeeejs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gysirfnar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/giiyrljkf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gazqcyabx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gimbnlpmg.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gqtlbyjld.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gruhxeobm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gqsnaqlgm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gruzwyore.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/giscgvvwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gzypqrwsh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gnilqdqdj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gbzcyfbyt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gxctmrapu.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gopibhfud.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gkysytagk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gyubansdh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghtjylewb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gzrzwgimd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gmdjvsmks.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gfdhqidky.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gcoyygzyw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gbiqgjwfl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gtwzwwatz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gbbuoeonw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ghhqpjqfh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gqlnknbsx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gmjwafizv.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gxejfpzwm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gkpafyujn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gpgnserua.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gccvfrenf.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gfdouprtp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gntqyagjp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/geusnftpy.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gomimjwgv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gvwigdpzp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gwpcktxgr.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gwrsvannw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gwqkxurfz.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gswhmatra.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqwlqreag.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gerakowqx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gteomdvlm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcanfvgdy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/goeoujgvf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gmqgkdnhq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gprifbdyp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/goftzwteg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gysuaepew.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gurnypbyy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gikwwguae.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/guqpyvqfm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/goicyaijn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/guzhjitcr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gswaygjpy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gnaegwngf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/glqikdubh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gnlbamiid.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gzjjntbpz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gelmpyygx.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gtxaplvuu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/grghubdnx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/grsyywgyl.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdwgteq.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghpwplout.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gxbvgefcl.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gsfpkdiqn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/ghcvfgxxx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gseaprzhk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gufqygklt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gpnancxzf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gudnjmrvl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gpzpxlojd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gsvlhslyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/grfzfdctv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/grdxcjoyc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvgphmqfl.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/grcjnsvgq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gasvlkajf.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/giaukvltr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gsmjkixjo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gvwesryat.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gnwaldduj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gtmrzheuh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gtrazjfqg.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gmafvfhlj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gpupxbymn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gnsnvuzuj.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gskehzeaj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gyyyshttn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/goohefvee.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwufiktrk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjprhiqwg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gcusbojyj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gktpqrmix.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gkuvoawij.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gdfalkees.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/glouhycng.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gayouhcwp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/grgxwlyyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gmpedsxqe.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gptopqkhc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gzkpxrtrw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/ggoropgla.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gfkckyihx.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvdgxxkuv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gjctikxae.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/glognzvzr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gzanofymi.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcphwlgaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gzmdjahai.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/ggkbeelzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gbauzfpcm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gnofwtizi.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gzhfxlzrx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gpeqbangp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gbwdefuuk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/guyzcsvvm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gialhitsv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gxzhftpnu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gjjxlvygn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gszbgkhfm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggssxyxob.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gxtigbeic.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gsaewspnp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/grelozwmi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/grmksrgnh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ggrxmjxhr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gzyvbzavn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/glycqconl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gztikuckj.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gqkckmtzy.sHtML


<!-- 参考信息 -->