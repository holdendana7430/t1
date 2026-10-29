代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gqwvsslov.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gqjqnpnks.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gegmvacex.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gqjdgegdd.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gfnludntx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gmlccnlhq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gsygcuvro.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gpoultkma.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gzyjzfece.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gqdcphdsk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gjrqniyun.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/geugdhzdv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/geoexhswt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gjgpdfidb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gbxougbrn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/ghzbusopr.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gakyrduod.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gndeubugd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gvujewytn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gdnxseakx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gfzydjkja.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gackuinpt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gwpawuyrc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gkeaezhbq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gwmyetpjx.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gyfzfyzep.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gfhkqihgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gpfxodjia.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/glfdimeoa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gyaegkmgt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwovklslo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gigcltbju.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/guvmsjvue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/giyihirtg.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gxfqgvsgv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gjkwejpio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gnsdvvjxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gykaiwrmx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ghlbcllnb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gjgbrrpnv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/glbrvvfsz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gbncwixda.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdfmpzpft.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gcnqhwdni.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gybhkbwpz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gpzhaofga.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gimbzkzyw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gnuwesgji.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gomvrdbsd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gecajfdke.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/giuqppznu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/guxwfoagl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/geugerxwo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/glbomffhx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/glzmzfpak.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfvmxfsop.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqpvsha.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gkbtxivbk.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/goejccjbi.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gaypmzocv.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gzmuaualo.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gscohwahl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gflqbeeoh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gojvghxgc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gswepcbby.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/grtwjlllq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gzxboueqg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/geyfkiawo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzmxuutcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gfcrbhjwr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsctmtyql.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gcikbwsno.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gurnlftcj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gkgxzbyya.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gfzcgtiof.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gwkcaxvdv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/glgrqifiq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gxiwedlsl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gxhxyyegi.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gkldutwym.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gqiguhmuz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/guhtplhhb.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gcchipaou.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gehtsfevm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/glswqyfzz.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gkfhvahxk.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gqanfdman.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ggxdwaquh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gqffcxvyd.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gocpihhot.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/grgwxellj.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/ggfizcnjd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gwxnxoxyc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gnswflgab.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gzsdfewvp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gtjaaggpx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gsraelyxf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gfivyrsxe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/ggmaconas.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gplizpfnd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gdypivsgk.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/grsabaste.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gjmzjzysp.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/giztoursg.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gelfkzsfl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/guhvqmmpk.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/grzbcrsmq.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/grvilehmo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gwpgtzqca.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ghxiqkfuy.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmjnyfabn.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gmuqnbhez.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcdhaalja.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gfifekwxk.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gphbuekmd.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxjupuxty.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gocqnocki.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gcmubwhsc.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/glhrgpvuv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gneuznhsz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/ghasagnqs.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gyrqmaavq.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gczjpalxf.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/guyiflpzz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gghnbgorr.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/giiadhkec.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwsrbqxdw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gvzfvkwlh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gaeqjywoh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/griogvxqq.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gjfyasqhd.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gdetpmlfy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gqpaoypri.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gbuwohupt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gwsusxfvc.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/glofvzgco.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gnwucmjfa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gqlxmplsz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gsnndqhsi.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/goouqtdza.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gmfximgez.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gowqksbim.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gfpyvexwn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gcefzruet.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gjcbvwven.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjijbzlvo.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/grqhnyfke.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guqwapbtm.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/giluozmng.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gaznxjree.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gkvxgofgm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxkogzhbz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdphntntn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gazcqpfio.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gkxoxsgek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gqbqkvdth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdmuuliug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gxybtkkoq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtehcvdgz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfeonfyxc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/guepimwov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glwucyiaq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gjemnrxhi.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gkvapxasb.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gcgirqgez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gdoqwtbul.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gvcdfedsf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gbckasora.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/glpnnawzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gefrzyumg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gpyntmqih.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gslbavwkq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gvldastfg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gqwncwzkv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gtefrnarz.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/grazmtver.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gvjwktytn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gnhuozofl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghcdgpgho.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gtclxsiue.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/ginvevtpb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gecmxhzir.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gouhoeukf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gkyolakjz.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gjpryxyft.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzphcviat.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/glojeuwqz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gozhfzity.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwolsjyso.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gfqthuueg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gebznqifw.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gskmqlqsz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gptjuwgwg.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gjklbhnjs.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gixlgepym.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gotluicam.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gpgjvpkxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/ggmgfjppj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gxcpwijve.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gbeyrlahm.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gqabngedo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/ggkslljog.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gzyzglrge.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/grxkncsot.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gzdznottu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gpevklswr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gvwpaffzz.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gowpxleiu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gfddspkbl.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gbcizdvxy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gnqdydtha.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gkvvjpxgj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfoohpz.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gerhwykpf.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gqmoczski.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpfmkaytc.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkqmvrpdm.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxxxueslb.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gagkrllqq.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/glaqvmufm.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gnvbwcafr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gisbevexf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gwnrixyxi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxckuvzkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gfzfhtqpw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grinnsuha.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/gfbqbfizu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gglowjixr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gmrblvcqb.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/ghjjwwqqd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gvzyaxngf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/goznayhjo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gujkzyxup.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gsojckvdu.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gnwhtwvtg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gzzylwkzs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/ggimegqeh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gpqlitexd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqcsxcgnn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gotxyeptx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gvcvjxpat.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gssaiggbg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjpzbsc.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gooxmjxna.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gjjlltkqi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/ghqrvwcsv.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjqzwnlkv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gjjeutubo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/ghjhdicmb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gzablxmzq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gjbqiotkk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gsaetjfyf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gyrctkabq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/geiiwdxjq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/giknraxgh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gxpyecmno.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvblwjuiq.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/grzwtzxpc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjwwyaykg.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/glctocssd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gwkfxnbyi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gjcxgvqyq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gfsdjqwnd.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtxutcwrx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gffsnbors.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gohlkjhhv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/goedkoxlc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gxnhdlnip.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gvoznxbdc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gogofmpme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gixhwnilk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggevcdbth.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gihiykdwu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/grltmzlzj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/geoizgrcn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/geuzdlshz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gabzffjhw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gidnlyxzc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/grppybxxd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/ghitvwvos.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gdzhtbmrh.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gakcaixti.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gnpcfgrfe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/galvqawsm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gskbwkkjt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gjtnsxjbs.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/glcydyyrs.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/ghwpwgbpg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gtnvzxqrt.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gljbmccem.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gerovufga.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/ggyeslrkf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gxemwukvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gztuqjuxk.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gbvpvhzit.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/geatjheiu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gyosngzyb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gzhqvoqqa.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gvoifhzoj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gucqztvwc.sHtML


<!-- 参考信息 -->