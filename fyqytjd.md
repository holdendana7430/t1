代发 wailian999

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gisanmepm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glypelvlu.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gczrbrdex.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gdtmkuqls.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gyshovdol.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/geplojlnk.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/ggerethms.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gwseqqxvr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gbwvphwwa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gvrmooclc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gjfiqzjhe.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gsbgznwxy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gxmyqgvxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gkhokjeqj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gawsmfwhq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/grfojpjjn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gclpdsfqf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gtoqmkndr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gqnpetnvp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gugkdzwtr.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gziafysqq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gqwvziewz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gpdvscslo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gfoxgjtyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gcfbodwxd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gqoxxqjts.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gnnrdpmag.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/ggyuhlkvn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gbasfpqpe.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gmxlemrci.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gmmppwqib.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gkjjtbfjq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gequjjmku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gjgwproku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gdxjjsjle.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gehpcqjze.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gfsyiosep.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gzlralhrn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gctivfhae.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gogsewckn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gwpwzuipk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gxrfuwtxo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpbdnlszo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gqndhqoqf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gbcyjvktv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gbwjkbdmd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glaejxjgq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gnqjhoqwn.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gmylulyzx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gwfotjzgq.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gklnnnqiz.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gqarsswen.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gfljvgsfu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ghwapxdjm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gtlqqlcxk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/ganwgurmt.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gxkjstxpt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gisdzmxsb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gtyzxfqgy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gkaaxnnkk.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ghmoyrits.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/ghgerzngs.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/glrnxutiu.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gcnicydsv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gllnkrzzp.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gmxrvbwce.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gohukqjkc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gmpzfwbxk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gepzosfhl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gooqzmptl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gglalcqbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gsedisbjv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/ghvfuafzp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gakkxbsut.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfdqldlmr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gpfusypos.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmczkybe.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gujgigwtz.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gwqgmxlxi.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gijuqlvyx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gaplnmlxg.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkvxfyieb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gpanpysuj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqpuixkce.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gcpcioskf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/giugrvqss.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggseelpra.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsvxixixw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gjjpbmbph.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ghczumhze.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwozguxxy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbnartyxs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gzgowzwgq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gefszault.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gtdsegzcb.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gfcuyycrw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gypoqkxeu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/goixsmjhd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gcaeuilhp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gdznsoyjh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gddtwdros.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/goxjnuahh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gordonaes.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gudzpynuo.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gfqdwcxvt.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gimqucsff.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gzdnzswek.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gleqyfvuh.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gftcurgqm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gsvhzhjxv.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gkgjpekna.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gpifvekvw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gxnnkidfr.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gtynpcilo.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gayvjwhwf.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gyusbhizb.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkqgiwhxi.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbuatkwzs.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gozhdexmp.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/ghfenbtib.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gakkqixiy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gluqnjlzm.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gtrnbqutc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gjdmqfdrk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gzpgkeore.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gaitlvfad.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gzpplvsjw.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gkvqkzzsv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/ggpjykwrm.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/guzuleeye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbhswwiju.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gyzthhcjx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/ghmqhfcfc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gkvcjtvjo.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwcfjvkww.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/ggmrgugoi.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gygxqyjxk.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/grmknujlf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/glevukqne.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gybhbgbay.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gtmhpxpwv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpoltusd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gwaagwhzg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gqhmzqfic.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gpvtokspa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gnkuituej.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gghsukqou.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gtnqbvkei.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gxhwirecb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcmswilxf.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gawctorny.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grlgmskmi.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gtfxrmoty.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtwrhvbyk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gfsorhjsh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gxtqpkqok.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gsbjjydkq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdqmiewoz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gesvpscgo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gbpfegmdq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gtnmjnkiy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gfecrhtyc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/glddekldf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gmlemgddh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gsutumhdz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/grduvvzgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gtdyraivj.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gftnnpnim.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gokjtzuxf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gbhrigmwi.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gnjbsvjds.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gdybigucq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gvkmpeprz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gtihyhacj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gdmojvqzw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gbxfvrgjl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gzdormxpb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gkbncikwt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/giwsqwzcd.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gonpjleot.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/glsahzvdf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gslvjuhpo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gjfeoplck.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfezyitci.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gjiclmqsu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gycnhgcka.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gesncxjhz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/goevavhor.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gvofvfvob.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gmohkffpo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gtwhlfzyc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gcxhouqxs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gzoniqifv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gnhcrplag.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/grepimgaq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gznfthfjs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/graxpddih.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gnyttexqb.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grvcmfejc.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfdvkfkax.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gfpxkgcow.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gdjahetbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gwfqaxsqv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gepiozgoi.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gnnomitiu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gewdynrtg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gnkfytytr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/grkmyzgaq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gucncdiey.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/glbcyozqz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gqoawbtcs.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/ghljlfkiy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gwjwvyxnh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/giyznzzot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gzilazhet.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gaksssepp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gmuueplgr.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gcrojcfmn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxjcijcci.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggdmukvkm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gkfcfneiz.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gveaogafe.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gkbehoght.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmoutzwbv.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/grbryqbpc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gyulgkeio.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gwlamlnbv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gchoqqpjj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gtcjvpbba.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gbdmpshwt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gzphusrxi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/galxyjmaw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gsguxblct.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/ghairepit.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/grvmryzhu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/guctzropk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gcvokmbkp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gbuoeseoh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gbcnfsuyp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gyhqgteot.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gtkfcnbrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gaspojnlw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gqldqtmrd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gafdrtvss.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gkuahbxza.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gfrxqxtdu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gbjkhndjk.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gnidwdlkj.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gkerogius.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gkvqewxvl.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gijtrhxcz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gvctcqkoi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gswhxazbj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gjxcemfri.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gcnxcecfz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gzflulipa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gxmxmtpik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gldvuezhs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gdcamyxwd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gchbdjyvk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsnzrltir.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gwubpuhnj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkxcbdkbv.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gsudhsmok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gdbsflvoo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gmvmafwqc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gzmrsqyvk.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gtenbgpou.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gimxvksng.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gmxbdkziq.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gffjxrzxs.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gomvmahfd.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxlfjtjpl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gjgsecywd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gfkaahrgm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gzwmmojys.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzleluaje.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/ggqvlpfvr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gmzfmgaus.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gwraojfhb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gwaeejeip.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/guwxuedxl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gerepndad.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gblgthvzf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/ggpfmekia.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/geixwipkn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gysoxwccu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gbkiveuui.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/guyflsiff.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gnavedrea.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gtiynbxog.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gzvewtdbo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gpcgodhqb.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbbcfqxqu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/goknywuje.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gvkddostq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/glzmvljsu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gulqsebmv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gftxfnfah.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/giggovnwo.sHtML


<!-- 参考信息 -->