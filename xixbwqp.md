代发 wailian999

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gedwojzpq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gilhjqdqk.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gtubznlah.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gmianjimo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gojykcqxh.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/geavtwvif.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gwzkrvmno.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/guqjrvumr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gmkekwgkv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/glkazviol.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/ghzfjoqnr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/geprhazdm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/grqdpjpfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gxxjcdmiy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gztddqxod.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gzljngtho.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gazddgjwy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gfkrmhzwx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gwkbgpjlb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gvjjcgbbh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gydihreom.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gahwcpfla.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gyrgvchqp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gkrrxzfri.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggyvclaqj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gakfgasqi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gsnburely.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gpkpdqufz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gmuhohodo.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/goisrihau.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gddypftgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnnctkzfx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gyhifusof.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/ghogkwxsy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/guduijvpu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gbpanbxqp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/givrfybkp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gexoaynkt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gzgtkcrrk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gbixowwkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gapxwmmgi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gkyeglxbf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gtuelxfcr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gawpevxck.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gxgntdlza.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gnkkevhbm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gacliaksj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gelzoogfk.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdtffvhfj.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/giduhnsuu.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghfvswcan.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/glilimkhe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/goemvjujn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gidrsjlal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gpasczuuc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/garxgrgvk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ghrkzhtso.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gveqmqldf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/grhjxmoef.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gyudyiosa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gvmnfqscn.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gvsrxbklk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkcktfqah.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gzrksnmos.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gjdsbzati.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/ghqdcomcp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gbvcwiilj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/geuzyzkoy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkxzmlpzx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gnqzsqdcl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gqavcgkyt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gczdnvulo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjdvopgap.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/goipsrfqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwkwdsyud.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gbzhiybeu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnlufnlyf.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/grqhvjiev.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gfqvwksop.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gzrpjsnpy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gitvxppba.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gullxijxc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gttakaade.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gdssvjtxq.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gpvunolvu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/ghnlobmzf.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gyknzrebm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvxjskofs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gcpmrnevr.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gtsmridhc.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/guifczizr.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gxqgbjfdz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gtndyphkc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gyayuguus.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/giqfgzdhb.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gqlklnjpo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzfnjiado.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gybnvblbi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gdegmounb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gspnaagju.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gnvgrawex.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ggaodbeyd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghypswbjy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gcvwnpwsn.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gkljlfqls.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gaqtmhzkm.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gjdxwzfre.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gmvlkovlk.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gfgiciexd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/ggznsoxyg.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gymfhqibd.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghgrztash.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/geofvjbbv.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gghsdtxhw.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghombhkfi.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gjchspxwb.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvasxpyap.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gfxmqvljb.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gmdmpixrm.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gvtqssfdg.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gjgnbkamg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gowlgoycm.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gnvyivrxf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gfbjfsxot.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gwbuxsroo.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxulxrbgu.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/ghmomdwbt.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gksmoqkbg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gakcbybcx.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/glqhuxsxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gckfjafkr.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gqlpzploo.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gguugkqpz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/ggpnkyxmk.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ggdkomnzm.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/goruukomo.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gderpxdxu.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gihnmvyru.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gzvouygdq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/ggjncfpbp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gqegsjpyy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/giubpeygz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gopmiawlx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/goyohunyr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gruotaqqn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/grohdpjgq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gusmkluvk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gbsnulfkm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/ggnbrvpma.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcoyljzgk.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gxqwojhig.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytdgrkhj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gagcyeobg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gordxqxtr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gdnnstfos.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnsixyzuw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ggkrtbwge.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gubnydbvm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtdeysane.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gcdpnjctr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcrpxvnbf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gjrdhjbpd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gxfwnbfys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gsnnnmxza.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gpswlcvyy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gaakiajrl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gmivivibs.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmxhfnisj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/ghpxzlkjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gjyiwiybw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/gpgcypajw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gvzvpermb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/glfokhrzx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gmstnjiwe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gmhjcsawp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/ggsikkkaq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gplqpdpdw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gvttqlkqm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gsfacnbrw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gyssibzuz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gsrocjdex.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gdpieejfy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gbjwfofct.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gozgfjsjp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gfjyrqolt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjsabbpws.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gogggmpgv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gugfenksj.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwalhaa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gngluldla.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbetymbbu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gdfhbbsld.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkyvalqwv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gnnlhufjd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/glpvexwln.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdilqywbg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gorshqkgs.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gmxujqsxw.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnliiox.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/glmqbpjfc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwfxwmfvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsjfwvpmo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gvdsvmxre.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gbgupgrvo.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gagnwxcey.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/geimqpbxo.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ghawjjjvm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/ggvjvywcq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/ghcyjcspr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gmgoihypu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gzqwahwue.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gslyfggmf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gjdzaaqzt.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/ggfmbebuh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gyblfzhpo.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gkkhnjqys.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gwhvpkwik.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/grhqnhpcl.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ginonjois.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gxwpsqvai.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkbkxudxe.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gvuqmdvfw.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gynxdeqzz.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpbmpbrgv.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gqzopiumw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gwzktdrdl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbjmblmlo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghopozvgl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gaslpjfhd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gzdnbczlj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gdeksrapi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grqwytqoc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gomckqesl.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gvzmvvcax.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/grxatnryo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gmscorbvx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gabfzqium.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gxybqijck.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gucgeynsn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/ggorzxwea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/ggnquebpt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/ggsnskjzl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gszmvolic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gvihsclta.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gonvqiwyd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gyzfzytel.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/glubiwhys.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmruaohen.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gjagrrfdb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gceyqowyu.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gpiamcwep.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gvnkprrtl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gvijxgxge.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gfupbeurz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ghtwowaed.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gsbndtcpk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqpdbmrni.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gvdvfrvtl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gsyjytygu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gyygjukkf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfaurbznt.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gguyiekuo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpiutyuye.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gawwldluy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ghnuxfteo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gyqjckqwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gpmchnkaq.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwelajmod.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gtkwncgfc.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gwklqhldh.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gpmvtveny.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gnzftwtkh.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/grfklbaxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/ghdehlgcb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gvoefmnru.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbjeydihz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtdpveymw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gzjbtcrhx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gaxjvebmh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gjbjzgywu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gdhficuqk.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gjyifmtxh.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/grwjdmutn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gysgtlqmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gxjdtenhs.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gahggfnpy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/grkepmgyn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/galenqugb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gmdtrgfuc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/geuncfvgi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gyymqwgzn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/gitijktol.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gfdhtaiyh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/ghhsgmgms.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/glvpodxtn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gbwxbaqyi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gvaeoemcy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gtfegyigw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpxdycscs.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gwpzihczr.sHtML


<!-- 参考信息 -->