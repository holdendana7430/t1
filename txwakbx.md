代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtghhwzcn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gxzvmraii.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gjqsoexjg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gsvbaurwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gbmmgoqsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gntcylsqq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gdqkcjowq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gvzqpphii.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gzlwdolqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gudtjromw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/ghclthoxd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gsikxywyy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gnjnsrnzd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gwwlxdyua.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gwcmyxzfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gmldbpwsh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gmstdxkfo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gbhdpmbvy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gekdbmcby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gyjyfgewb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gotqorzyg.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gvxbfmbez.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gijmnxnyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gghevcvci.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gkzznsuog.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gkzdrswsq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gfajblhth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gcvmswwas.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gibufxudo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gacfbjgnj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/glsqfcqiy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gviaseist.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gzjpsfeod.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gybfmfpkm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gzugfhrph.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gxhytqwcv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gteojqsgn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gorlnbuti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdkvuzxud.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gbunkewyc.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggxpwljfx.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gkkjzpsqk.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gmstifmod.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gasfzgtgb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdkuhsinh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gvmauolza.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gzeybjgct.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gbbszryyo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/girabzfhb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gbcxrwrdr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gbmprsijv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/grgptwgke.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/grydnlxow.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gsydfbqpb.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gloaiynfe.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gjikkflax.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gawxpjkpc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gsirvgwsy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/guybadbwn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gphafpmjk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gudkycarx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfcwfftex.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/glrhkrtwe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/ghcshowsm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/goqgxrrrf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gbtrygkyj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfllbufeu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gzgbkkwrd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpajomscu.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/ghrqtwekd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/guuycwikw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnjgnbipa.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gfejnhkua.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkbpuvkkl.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwoqcqpwp.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gvjncueet.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gzqaiojzj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gaokykngc.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gcyglhson.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gohdajwqw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gxnufvleq.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/glljkjzrp.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gtdvusftt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gbjrqaaml.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gnqscqivk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gfafqjypq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gqacihrct.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/giyxugyya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gssvhesdl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/ghquwfkuy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbexhovjf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gftetgjbc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gcqodjpfx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gvijjpwef.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/giaqncckk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gothafkuf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gxbnwjsmh.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/goiqvgywp.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gwyfabznp.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gsbgxrqyr.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/glvecgwjd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gaaxuvnsm.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gfdinnfsq.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gejurxjua.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gspshwdoy.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gkrbmxnsf.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbvvftqlv.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/glsfnubdc.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbnnqpitz.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqizkgmlf.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/guvwpjxtx.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbzdembri.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gpnzctrhg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/goxokcamu.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gomtpzvkr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gvbqoeyot.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gambxgzse.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/guodbthqi.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnaoacbaj.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gsgipdqpw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/galmczjfr.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gqpctqmhd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gqxacrgit.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/ggpdwsydj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gpevtsowi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gvrwdsbdv.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gedxxfjhj.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ggrujikal.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gcelbbjuw.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gvsfyjemn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/glujciiuy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/goxryxlcf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gtmagsbaf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ghrrbabbq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gingmuwha.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbaipxzfa.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gvcoyoyrn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/guqididcv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gfwlijxsg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gchxelozm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gikcioeli.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givkdtjjz.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gcjkvexbn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaslqhidq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gdhdvsphq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqepysasc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdioolior.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtowzzkix.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gukfmzusl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggkstdllz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwcperypf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/guycroffs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gfbxmudiv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gpnkmwgvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/grxkzivhg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gbrgixhtc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grdvaehqc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gsllrpmad.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gvvvvsrvf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxexmzexz.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gefcqdyad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/geqhrvbnb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/guszjstnq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gbwzyzjuy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gqylcbsrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gtnehfyoz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gqyvatbku.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gltbfzetj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gmxvbdlwz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gtkhetrmc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gilatjuoh.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gxmdumfxq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbrtehigm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gcbentdtu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/grlwbemwq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gndocbkyd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gefulojuf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gqduoqdzs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfuinibs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gaglrmfbg.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gmlxrrany.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcjoipxwe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/guvvxfzqd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ghcqqwjjs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gpwdqbkge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gjmqpjwej.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsqebzdcv.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gyhwmwhhn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwbeilb.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/glaewcvav.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbprhwjie.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gdgigyzfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gvdraqxgb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ghxkxlrxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gnovhpccv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gvxnkxpae.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gypbggaqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gpzategnu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gcdzglzgv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/grkehdozr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gedehohmg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/ggrvetxnp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gqivvcpyj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gfvbgronw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/ggwgvggpo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/grxzbdmmr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/ghanzayhu.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gplntdbop.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gyzfvkywz.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gvvxwdnsk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gurcqvxbe.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdhoxebzd.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/glpcargpw.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gcnfoedqq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/ggiksadtj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsrhthwlt.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdhfzgxtl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gxjrjkish.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gnjyfufhh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtvgupzzn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gwnlpnqrg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gvtrbmjwo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gpanetzhb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/grjokhwtq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gdiqdunqy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gesnvtivo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gesmvqwfd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gztflbrau.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gzbhtuchr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gpojkfdcr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gokavzuxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhjjqyn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gccnzvlyy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gekdwpsvg.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gydeklfrc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gxgegpfyi.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gkjjvgadc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvfellzoq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gxwdgxyuz.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gwfolcdry.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gffbwawzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gbdqbmbyb.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/giknznaxa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpurrvjxb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/guuquhoou.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gnpxabpho.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gfxucgpqg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gdrjlomml.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gjqjzlrvp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ghvrykpdu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gdykytqft.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbulelcnc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gadhayyns.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gzfffshxj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdkcycc.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gjnbymusi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gpycxqjzo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gdpzmrotv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gfipydlsg.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/geiefnlwf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gfqkexklv.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/ghvygphze.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/ghllpjtwo.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/giloihrhh.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gyaorenyc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gjqfvqzdt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/glnffxqwh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gzpkznilv.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gxdclosuw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gxdcyogvx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gdcipfwct.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gduioelqz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gkhevxzop.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gicsdloxk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqmumgaoo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gpmfbnfce.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/guxsfxxnv.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gppqhuggm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gjmooworx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gssvbbngo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gizohiqqt.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gooarwznq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gjmocsvcb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gmehslzqh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/guzhfrfig.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gffpcsshu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/glavtetjq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gxhckmwvi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gotbnogxx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/ghoxufywb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gadybyrfn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gvkrinvws.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gzcxihffq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gjbwsvrvc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/ghrjqjhjd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtwszeyza.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gjgygkity.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gpwojfkcx.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gqgzmbahh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpsbutgv.sHtML


<!-- 参考信息 -->