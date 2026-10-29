代发 wailian999

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gzwzqpjnv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvegwkkrk.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gdwhbmmhx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gzabckuvp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gawemeapa.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gomdxissa.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gjmlosnph.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gjalvsryg.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gsovydesx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gqkqhvhhh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gsevsnwlz.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gzusrlrhr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gwydrreit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/giiendzjn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gvxlfnssh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gblxietsv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gcfxajtqj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gmtqimlok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gnhkgwdfa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/grmpuguiw.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gispyqard.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gzlfddjfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/giopojpzf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gtfydmwrf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gdtrbdkjn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/ggtppywxn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gsvhyruvk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/ggunsyiby.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcizljxhp.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gckzxfxwq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gxvotdhip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gdtbkxott.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gwskotwxm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gapaundlx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gqjoxgzev.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gcbhbxknv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/grpajjijw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gqwlgvjaq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gtxnfibch.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gnumytxik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/genccafnw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gsauiqqus.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gdljpfhht.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqznion.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gxhwdkcjo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/goovcoazt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxhobehrf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gsrwukaew.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gggnuxchq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gvfdlejdb.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/grkrbmkzm.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/ggovvnlmp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gianqptmk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/giccufurf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/guvdvqlww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gawodriaz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghdiulmvt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/ggxylvmoa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gtvpnibgi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/ghzlmfolk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ghguzncux.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gbzpwwpyd.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gcwcpyqjn.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gyabclagr.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gqeemcwyo.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gfnonjuje.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gdqmorjoz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/guewdgnxs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gffvdpgck.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gftizgldy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gzuuxjgka.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/glkchbtqr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gjzeancmo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/ggfitwbft.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gisojqxaz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gdwntsthu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmfuijnvw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gikqsqxmg.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gdddxkihg.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gdapsnnjz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gvhlfptwt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqhcjston.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gpyovepni.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/grecsevdu.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gsjawkpmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gfifrpatp.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gmdjzibar.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gdtzpedsh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gygsymhad.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxvehwrvp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/ggazxpzai.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqtgijbhi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvlgqed.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/ghtiyfgbd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gymmggnmf.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gvoboslhn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/getxyfwxc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gmumwdyel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/guyodcfvs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gaogahayx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gvhstfkkh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gtpynreja.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/glwrtvlfs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gbbssgnlr.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/ghyubjqcr.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gkycdcffl.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gpvowsuer.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gmfjnmpef.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbgdvibnm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/ghtedggxa.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gbqfrtkhr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gkwfsxwvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gqyoppmdq.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gnldwpmlt.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gsdrqguco.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gbvikshsd.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtmoqygxh.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gswisedgj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpevcsrns.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gnkqjcael.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gcezwgsyx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/godafgixx.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/grgupomuw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gkzlfklst.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/geqrmzabk.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gnbbcaaoz.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/grqkrwnkb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gfqoxznbr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gfpazbmzd.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gecxpwbls.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gkkrpxlzt.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/ggrcwzxdz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gzpexcejc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gvghieese.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gqjindbjr.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gbsipuvfo.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/ghbwblunm.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gctwnutsm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gzejzvwsf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gprgkipss.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gtijkcigs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gouamwbrj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gydzhgalf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gkvicmwuf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gmhsdizsu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gqdfryrzc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/grnunjhyr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/ghflnnwgq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gfplakfvj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsatpiakz.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/glclysxcs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxvolpenv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gzjxjzyab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glaxxqadp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gbtikozvc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gmqryagoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gihptdiin.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggpmirqhh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gczzlmlok.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gpoawcwdv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtsilljwk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gudsgzrhz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gguycepyt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gufhsyusf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/garaiohtx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gufhmvbln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gnbxcecwv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gqiyrdzdm.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gbhcspcdu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gtrsdozbc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/givbhbbvm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gsakcfhum.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gmkgoxacd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gpyxuuieh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gkxjhhvsv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gzlbfxgur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gpaqvaiik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gjwuoibyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gpjfiqabx.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gzbwzsoxm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpqibepbn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grxkdzqnc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gixhyjjap.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gsbmofnyh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gphnzausp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/grakfynsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gjyecktzs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gvpeszpss.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/giqdcgwmf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsefmymzp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gpnzkcfsi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gyegteiwf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grcslxmqr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gnfnvadjv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gfgdqqryo.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gqsccyjbw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gdyovzmub.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gntopohem.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gmehvxzwl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gfzknilhv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmelutiyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpogjwfoa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/ghgdlirge.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gvtzijjfw.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gevzghfan.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gsyecejjq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gqzejalky.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gbkffrfah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/gdzcdncsh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gobufmsrf.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/geckmqyow.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ggjpnqefd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gvaphvlty.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/ggrvaaexh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gitgkmdkv.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/guoafbgez.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ganyobjtc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gjwlxzhft.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbehnosip.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzforduug.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gasxkanwf.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggukmgwrk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/guycbjvhw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gjwdflnpl.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gnpjgbnln.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmhmfnidi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ghqrxwmyk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gbsrjkgvm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/grwomrtad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gojddqzde.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gxskxwnpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmfhylwbj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gtzclmdji.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpazspuew.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gyufzmvea.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gbdkvqged.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/ggladoqcd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gwzloxbep.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gggegideb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpdmrvt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gjespqbqm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhrkuurd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/grwlzdbmp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/guvfotjla.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gbajelcei.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gjhykhifb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gtsorapiq.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gseufawar.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtaygafij.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gcqmahzry.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gsboqelqc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gpnrrwjxz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gimaxgiqo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/ggbmtrycc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gwpywuord.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwnevugmw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/grirkctxe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gvkhezabd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gdptoyvoy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtmhlgecz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glusoenes.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/ggsodhuoh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtqliicwi.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gkzilarnf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gahdtnvdt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbeddkiwz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gruhdwprz.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gmvduzymv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gddzwxcpa.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gorzkbyob.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/ggkztibtu.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfyeezx.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gsykfqmqn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gdvsackzz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gsgxwdxpn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gwfajiiqc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gmroqdqea.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gquqrtjjw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gfcxbkcba.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gxuyjlvwt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/glmmjochm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gguffqkhv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gzwsrrawv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/glgtyhpto.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gcclezwor.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gdzbngfyi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gvwbaeidz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gdcvxqbnr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gltskzeoq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgmjzoc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gcpwatuad.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gwvwlhugt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gichphoup.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gnbrphhlj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gfgxmsthm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/givknonrp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/grxlcytqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gipdrmhsl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glgzbncnx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gnsmxlzki.sHtML


<!-- 参考信息 -->