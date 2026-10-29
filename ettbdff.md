代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gpliwvzjv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gtkgduwng.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gmroqqcwl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gxpbclvhe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/glzxnyfwo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gvukdhame.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gvrvoxuig.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gfgvmteoo.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gufbfxtkc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gellutrwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/ginkhoiuc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gnleobthg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/glfzddhzj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gytktojhu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gupmoxsum.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/guqwgzfno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gvuxjdqra.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gwksaxdat.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gmyhdolsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gbcabmiap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gvpfvrywg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyrvqohvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gnctuvwde.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gvtewtoav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gkkwnubuf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/giskhahyh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gcbdlyvjk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gevsfrifr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gobyvqnpc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gcxfmrwpt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/glvxzpbpy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gkzbjltfu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/goenhiolc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/grjaqdbaq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gunqdwvyu.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gcvhqbckk.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/glwcvcwfa.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/ghvimofxc.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gyrhjtcmh.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gcrcrmuhg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gvchgyjpd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/glumxztyk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gmlgvjqhl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gvsrqglcz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gbmcanpyk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gdxeybwnq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gjcdofyue.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gyjsrvhhn.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gdqrisytk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gnetkxlkm.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gyqfvjysp.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gdzxgajsc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdwurwpzi.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gxwxbmqnt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gxtiknash.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gotqfhgwb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gdhnnbaie.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpybfwxex.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/giytvkqii.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gomptounq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gggbnnkhv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gechjgako.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gppnjksra.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gldkvehef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvevldmma.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gucijaqrq.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gdahoimme.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gdgxamehu.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gfupgpjrw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gquxtkpex.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwirevyhk.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gjroscbnc.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gxndlfydt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gcghazafx.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gntchetwr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gagzvmdrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gikuxamll.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gjbccfuwj.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gttnbkdvu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvbagzdsh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gzoftzfia.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gkelmjdhq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gxqboezjk.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gxfgxcsfi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/ghqiemizv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gfhczzrrx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gukmdecat.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gefgrjlsn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gqtnnqyek.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gkckygfdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gyxqigxru.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gqgdocjfm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/grenocppb.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gokykfuek.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gsfzxctvy.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gqfqqupmr.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grbhjisjz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gdsooqezg.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/grduyurgk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gpxvpqnkx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/grcxwiwlu.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gbxhrjgwu.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gknhmypnr.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gpvmwprhy.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtqlochdq.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gofvqveuc.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwitxgsgs.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdybgmpwa.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gsjvcrzlr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/ghjjdqtrz.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/ginelvlqn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ghxvplomn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gynevbgmp.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ggsytwlat.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gcwgehedq.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gvbmqywuz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gwgwifkct.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gkuahrnft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gywcnauaq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gvzbomjpq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gudtqsyoc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/goravxomw.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gulfexetk.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gqggckidi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gfvuldath.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/glxlimejh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gjkfglbzk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gaujevcid.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gklhzeooh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gniagwbwx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gqtmwbngx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gurnycctu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gdqrebyod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gaajbkixp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gdouydvza.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gfkxlmtmc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gscuozovj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjuozqlwx.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gvdbbxbqx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgxpkds.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gnqgjcdzi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gspkilnns.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnjkmxyvv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gjmxablfi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/giiyzigwx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gytlimzww.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gksxdqcmc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gowossfrf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gennfhjqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gzcbqrrru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gzuqrkwhw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ggxvalcwc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gkgplbpop.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gifkqrege.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gnyifpast.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grnepmrsr.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/ggzzssuhb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gsqydhekf.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gyaqsimkw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gxzhxozqf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gezsbhxxg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gomldhnqc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/guauwwlzc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gzfmckgtc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gpryxztcv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gktdrwolc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gzxfogkue.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gjadrelnf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gayaywmcq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gamtwduoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gmmmnbvxi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtyzikrvc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtgcrnljq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/ggnwclolp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gopdjlxea.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gougvsisy.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gtnbwgwog.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gnierrmqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkfyftxqs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghgajedvr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gqolfywjh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gkgectnas.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/gqparffvo.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gwqtvzhma.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gsabybfaz.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gadnnemur.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gevdmqygi.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzrencevs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfrqhkaey.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjnxbipyl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gaztmeydo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gbccfzkdk.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gtuhceorn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gozbpbklx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gwrozyuxx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/grdssaafw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/goqssxjzc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gefxpbxyx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/ghajbzutb.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gokefcilx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/glcdiwsdi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gwiiicler.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/ghsbscyud.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gnyrfvhab.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gkkmonyyz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gjdtgitoq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gpkhmdplk.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glyxcxari.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gqufycttn.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbusfhqfd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gwrroctpr.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gfvbutpyz.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqzqsbkxy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/guafhdtni.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gacvgljgn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/giodhnktr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gtamnhkkn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/ghozmfhqy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gpkzakxzj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gmalvqnyv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gcvzmeszj.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gqdnaoxei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/guxbhiibj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gkavkobae.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gzlsqipco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/glamflkxg.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gclvwekyv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gmcyjoolz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/grvpovfoz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/guzpyitge.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gdftdwgwj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gdtljvelz.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdxktruth.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/grdschglo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gabwaimzz.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gqrzcbtjz.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gspcrhqoa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gzphfmfno.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gnyvhgolr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gnpupzxtk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gycdqpfkp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gnbdljbyp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gpxzpahrs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gcagkxjjw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gkdugqyaf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gnphlvhcu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/grupommhw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gywpxmfhf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaeqiyqxm.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gwarbcpcv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geyfghimx.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gmawokgnc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gzqpsqvro.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gwlrcvavj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/ghauzghyg.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/glmodntvz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gcyodyepy.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gclpeokaf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gcdkvynad.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gnmeqerbu.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/garcsjyfs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gmebrpapz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/guhjgzdil.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gihiyylyv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gevihzugi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gyjyfskab.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gvrhhiojl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gggbvnbye.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gysxveklc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gbyscrqoq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gxmibvzzm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gruaehkct.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gjhgwsmfd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gpiuhfamh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gepcaqntf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/guscmqajw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdzbikvdt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gawonmheg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzfvknkyx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/glplunify.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gxrokaain.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtpucnac.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gfaqgevrk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gtgplsowv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gdjmzffdt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gfyayqmvk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gmlqaoban.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gquepglcs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gvprmissp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gfryzbipv.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gwfvbdcfe.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gqrecqpcc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gwadnfitt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gvsfryxud.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gkjxculzs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gxwwfjrrn.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gvysyxgxf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gjkyvnmqv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gjnbnuqyv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gpzbrfhzh.sHtML


<!-- 参考信息 -->