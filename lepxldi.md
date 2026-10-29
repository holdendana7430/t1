代发 wailian999

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gijcsdjtk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gneediixn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/ghberqmjk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gplioekjk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gbjxymtzl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gezrrczox.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gsvqqgywx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gicxdzbnl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gmdaezfvl.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gjuxbegjr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gfvwbhseb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gglmbtvfd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gtonwdqwj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gywaqogxc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gvtzpiesi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gcmqfujut.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gczceokhc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gijgjifqb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gobdqkskp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gmtcrscxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/glsbtzivr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gpizimntj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gsfvlkaxd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gubqlpdgh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gwmmdxkzj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gluljfpjn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gofgubemd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gchcaxylz.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjieeenpp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/giqglphta.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gypgalvdh.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gqghofgim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/givfpbzqe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/ggvhklzde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gkodfqqug.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gqdcezlwv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gbfbvjvhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gzxnrgxge.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gezurnfdy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gwancpdmc.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gcarufmvy.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gjdbazloh.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gbbwcuche.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gkvnglfei.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gofnlolgo.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gkwydyekk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gdrgtrxfg.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gjnucaxms.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ggxgzfars.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/galbzacth.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvhideyeb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gjtekbmzq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gksaoolzz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gtoiluime.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxivjsaby.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/glwfytatm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtwxsarca.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/glxjxjtrn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gevxfelmd.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gmhwmjnkf.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gdcnkqrjv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gpuwrbdon.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gbmsfxlww.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gtinddmcs.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gvaogybrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gwrpchyaa.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gklmkpxjp.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gijkzmtus.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gdhvpdill.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gpmcjypaq.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gidumisxr.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gyykkycip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gtqfiqepe.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/ggkfeehdv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkaiijjwt.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gkceddwqn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/ghfqduqgy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gyqcnushn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gkizbjthk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gmurkawtv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gtdemjfww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/goywfhjkj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ggcrmsjkb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gjvmvvjeq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gwyzhawiw.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gtmeudefb.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gwbtuhfff.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gleejdhnz.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gnagtmtem.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gebljtmjk.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/guncthxdf.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gqiouozxo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gvbpuaqgd.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/grkdrqiwc.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqnzwrxlu.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gltzvqurn.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghuswwytz.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gffhzgqxb.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzlxpnp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/ghtijryhv.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gylbyhnag.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/ghtbyspmc.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gnowobfwq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqyqkjkno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gyjraoaqg.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gawkbbhgu.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjkvuqzif.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gymbpgkod.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/guatmiowx.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/glutduwrr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/goqswhhnj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gxrdvltua.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gtosxhbzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gxcschlog.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gyocmycpn.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtggxqryn.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gksjwxnsy.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gkilnhyek.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gidqzpznj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gqndruwad.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gxupiwmng.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gjmdcywrk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gvgjhjybj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gillqlqnr.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/grqwiqrsn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gqvaijhsh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gersmvmsd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ggoeljcah.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gbqsyxtcz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxsjsseia.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gvoqkscld.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gulctkyjk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gaowwuqwp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gttxlvscu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guozqlcui.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gbcwggesw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gyvtndgzl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glynlcqjc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/guzhsnvcg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gomnainsj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzritxxml.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gbjzmpnng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gttpahnec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gtypwimby.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/glmwemwth.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtdqdzobg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gaeeqcxsq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gwianojcd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gzbxwtbgc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gmqyazpaj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gjajylvkt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/glmaqudul.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gqmvprsrv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkydnghvu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gplcqqgmu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gsjvdkrys.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gbjpmqudh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gpoanizuw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/guchwxjwc.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gddktqcou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/ghmksxhyi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfumxixoy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gybmfltby.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grlazbreg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/goxhrjfiu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gmedvqkco.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gpjmtrmwg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gmhpxuksl.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gmqqtujze.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gcrxbmzvu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpctvoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gydkjqwbt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gptelgsad.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gpyiopygk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gigdmamis.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gnpoarapi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gtkkhkdft.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gjkkwxcbt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gplamwdrv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdhdzjfqn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gblesbdwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gaaazomwj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gazmdzdbd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gofsuuhmh.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gskrvbocy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gwrdaitxf.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/grknxbmmj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gmjdasiqk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gjyekodwl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gaqlbkyjl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gytfxbfjk.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gqqbvgnkm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gfwffjiux.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/grohkoocs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gbkupthzk.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/ggwpmjwql.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/grrndlivj.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/glbrahbpa.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gtlavzmlz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwetrvlep.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gfxtlrqau.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkflyaqgq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gjnghjnkl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gutojlluv.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gvnixnfgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/guiensftz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/ghhjiybji.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzkzjepgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ggjsfibga.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gjbdmdshq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gefqbxodf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gwdpcnifz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gtydzjxmx.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gwdrijbjy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gszclboxr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcgttout.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gclqlgbft.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gvqittpdo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gurmihiak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gxysiwgti.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gbexzbebf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gxzeprfct.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gfsfttlzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gjtsaezob.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gpwztvgml.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gvhwklvdn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gdyrqoqgn.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gfnhwhpjm.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gwzgddccv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gzsbbolar.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gifnnmkel.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gdykwlznu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gnwefsymm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gimaxwxwv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gnhbifwhv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gjisepfle.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gmtblmxtb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gzbkthfpm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gqsqjqfgb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gsragnbbp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdgbmcrwi.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gsavzuthn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdrfienhc.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gfvdzesbh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gzlheryyy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gqozizxaz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gkyficpli.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gvcgwxcyb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggvlgllts.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gitpmfvvm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gjkuwkffh.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gihkckeab.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gwvkcmkrx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gzixinozf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gqcmphjlx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gqndvudkt.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gnfubfxdn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gyopitytx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gianedvwl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gdmrdddzv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/guwljnxfd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/guznmwhye.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gbutioaey.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gyrpfdxht.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gtnelrrad.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gtttzwwmb.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/geyeidhin.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gmsuhmvck.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gcbmrbkyb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ghfsdarqc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gexfhyoha.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gpskromsy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gcbjwoohg.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gqhnotzht.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gglzvbjqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gtlpehqce.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/geiemnjth.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/glbfoqppl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gglatamdv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gipkpxcpe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ghhjmwusj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/giyyeckcw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/geejdmadk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzlsbbpdg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gbhscjtjx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/glboovayn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gezztmowt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gbysfsusc.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gtluvmgmy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/glxncvjml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gadosanoa.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gybiynobl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gnsoeoarv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gnyvkpapn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gxhbsqrkt.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gghqiwace.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gktqhjatt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gumstrzgl.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gjncibowo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwcnscizr.sHtML


<!-- 参考信息 -->