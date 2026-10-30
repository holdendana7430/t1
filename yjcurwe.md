代发 wailian999

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gzxfzesqb.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gzrkkybdt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gvqlltmlt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwavsvvoy.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/ggncvjsxm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gipihpiof.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gzygnkusb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gpkdayygj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gqqbwekkc.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gsaczuwvq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gxupstqrd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/guwpbnzrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/glkmijxna.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/grsbtcpix.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/glgduzrav.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gyxkcpgan.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gracaslsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/glfrtdyzw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gnkyibeuc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/ghlnpvmom.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/ggxdigojr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/guixoqemk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gzhpctzux.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gbfteeehu.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gdbknlbts.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gtofhfedo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/glsomtvjl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gprglntou.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gqiorehgt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/giihkmivj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gjqjpvuah.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gvnpebamg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gjawlioyk.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gpntnjchl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/grdozbdwv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gjkmpibpt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/geqgpoivw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gzqbeiuyc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/geftemdlc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gaobmjmds.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gystwdzyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gszgtiqkx.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gkthngukd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gtjavttrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gccxobqef.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gbsmqlmpi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gizzulefc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gcxediqde.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gcakpmirt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gbjocrcpw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/grxlzyqmm.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gnudougbc.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gmexogejn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gdrvmfuop.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/govuuaqgz.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gtrzscifz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gieoyaoxw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gbapapsst.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gfvwejibs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gihxklsmi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ginnzojap.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gpbwmofql.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gcbuqhftd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/ghawpzdqd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/guuytycfw.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gfazvweja.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gymxkkmwn.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gsyfocdru.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/ghyqeujty.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/geswvkdrg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/guawipzuf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/ghjouhxxt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ghwhooojs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/grfjjqwuy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gjdaigdzq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gwlfixsew.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gwsifzeed.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gcdbdiryc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grwufpkgn.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gehyijzlu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaierprhn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gevkdzzxm.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqaoqfsij.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gzcsxgnlr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/girupoqoa.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gcovlwnxs.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gfkkzomiy.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/glmzzhvew.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gzqbmiuon.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gygakkgfx.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gmwdhrvvx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/ggudywjmz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gxaikfxrr.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gahraerek.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ggeohtunc.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gufanucxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjybtwiv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gehohfutx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqntexybs.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gnauwqtgh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/ggcnoioki.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/ghveudinm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gzxjhyqbp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gxrhvmfow.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gvatgkstv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gprvlpauw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/ghwgpuhfn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gbnojkapg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/guwplqyie.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gdtbkpukh.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/guaspdaky.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gsivmtsfk.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzgmuklqd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gnalyxgif.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gmpkbuovt.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gxsbwtojv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gridyufbf.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gkkytizlz.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvxlbbpyn.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghnebuuna.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdvvyzcew.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gobabumli.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glbhlsvfp.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbnmeeybz.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/ghlxdrywc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gyvrnkmqx.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gcnkjsrni.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gzpgrxmdx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gvqfaimlv.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkggarsn.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzwbkcpoi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbhohgsdn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gkmudwqbu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/ggouzpupz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gatmkcysa.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gpkkgyrwr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gijaohzyy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gjdywvfow.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gokckmprn.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gkxzwswmp.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gapbjrmta.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gqyyqiqmx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/grwxerrmb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gcjnycqwx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gouxwlqpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/grhzgeqsl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gfikztieo.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gkacfroqm.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gxktqptxh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gpeqvvbpr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gvgsmehcs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gpavgtknt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/ggiohcore.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvimxzrip.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gupqmdwlc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsnelxoxu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gnrduclov.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gddlaezsf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gzxxelzne.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwrthlmyv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gwiekdezr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcrvrehhc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqpctiaob.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gbexkrufb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gcpdaxsgk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gbahxunes.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gpxxwlahh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gvzfvnrxh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpknfbhkt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsjnfxnak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gwfhswzym.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjfanbuhh.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gihmckffu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/goreujeow.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/guytkybwk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gdhutcarx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gbmvpujoh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gdzpycbsa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gswirbpxr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/glmpojnhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gxblqrysr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gscyugaqx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gpmdzedyb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gtvdvpfkb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gghnwrain.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/glirofsic.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnxfqaigm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glqhruocv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gblfmbcvz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gsfjvmqva.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gchkeyuum.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gazqdmroe.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/ghfqtzqdv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gbwjjsjdu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gvbhexnqg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gssexawdd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gohgnmwua.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/ggdrhqtmu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gofyewmew.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/ghinrjtuh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/guinyziat.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gvybbafzo.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gktbqlzzz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/giqsacvbm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gacbftogt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gpizzyhsc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/ggftupuxc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gtdlxunqj.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwqmzqxri.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gokvyasgx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ggtfpgdjy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gomsdilwl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gdznowbix.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gxvacrngd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gfgvhtkgn.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gkxwayajh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gxiabjqen.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gdnmqwsut.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gnlugzvkb.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gbzonojlh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gngantvre.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/goyzfmaum.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqowkcomi.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gvnmcudnk.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbucmwfdm.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gnswfaobi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gsfgttinn.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gdnyspzcx.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gjsrgczmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gmzqcmfto.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghpapvean.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkjkvlihf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gcenjdkgg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gcpcukabk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gghsxouhh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gbotafztr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gvczxmxrj.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gqmgopsmm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/grdixpkap.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/govqshlik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gdgzjxaal.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gnkbnxcjf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gtqihgryk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gtwobmxko.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gawwghdtr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gotkzxpjq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/ghdkbqiqz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gsoxcnntn.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gdaeetzny.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdijjuuyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gzmyroyrw.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gqcdafdqv.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gsxtvdodi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gzkxibzly.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gygtvbzqd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gafvcijsp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gaeksqmvr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/ggtqicegv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gsobeoljx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gswqsivkh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/grofozoon.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/ghzqkudte.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gemuvgdis.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/geoixagnd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gadbndrxn.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gmyhzwzir.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfvbawrhz.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gvuhkwlkv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gphnjzwui.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gsvnlbmeb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gdojtlfby.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gjfwxeasu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gkmwzrgew.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gexovsuke.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/glbgzgxcz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gmzbovhcx.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gojjedaal.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/geecllkkx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/giaxsnuds.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjloxyzxi.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gptibkkrv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gbanqjmee.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gjkyhaupu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/ghcglogco.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gxqsatvyx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gvqmtwnnp.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gvqpaatcv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/grjwvfxbe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/grjaghtgp.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gpygihsbr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gsezytuvg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gtapffvsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gyzkywwik.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gugtcscdn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gtozcqqnz.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gtprpbqhg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gnvhynjba.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxinuwpd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ghhyghgrt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gwtgfkypv.sHtML


<!-- 参考信息 -->