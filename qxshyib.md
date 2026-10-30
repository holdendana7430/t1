代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gfejcvtwp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/grnohzjex.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gjyoqtbvd.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjhsurhsh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gljntvnsp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gndgnsbpj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/grmmjeaey.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfickqsde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiuqmcio.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gchwnucxz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gmgtehhoc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/goxyjkcxm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/ggeaypusx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/guzhpuwjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gftagddbi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gihicmjnj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/glearwbxa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gkxryjdmx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gzrybhgjo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/grhksykzx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gpuqggpci.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gxnoslgzq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/guhlfyjkq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/grmxsjjfe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/guonbehub.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gojbjwawv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ggjialmpy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gqsqzhkjl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/grdqvdgvo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gyiivebsj.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/ggyzsuqap.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gxxtfdtpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/glojdefyt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gwdkkyygq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gucsuxgwt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gjjubpkqf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gcxyoagzw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gqcwuulon.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyqcalacu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gzgecqafu.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gfolboutg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gsctcfafq.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glkvonzck.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gvndfabjq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gioyxgpya.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gllgeavbv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/glbdmybmt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gnvwosrxs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gdezfthbr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gnzhltcfm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/ggemkbnmb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/ggdyoxnyy.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gwgsesimy.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gmmmgldag.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gisvhztth.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gwoyglizm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/glehhsofq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/geneptetg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gpvwfmebr.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gmoapnxhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/givfgmqxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gydssatik.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gtoetwfet.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/glldowhmg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/geliivapj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gknetzixm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/godglcyjp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gsbjoppxq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxwxicvbz.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gftiqhshj.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gfgupxmfo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/ghaoicwjl.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gszwrpdze.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfcnifyjh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gyhvujovn.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gpdtqvhnw.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/geujegpfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gesxgsbpo.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gfedkexmo.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghoddlybg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gzpswhdcz.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gbebccwew.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gdodzmvwh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gpgtnpbdk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwmaurmsa.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gqagvwmdr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghdeicqvc.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gppflyrad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gtpmqezuh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ggknjhmdp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/grsxxynkc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gbszckoes.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gvonxybqm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gkwfbxhev.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gplxbkgeu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gsduozoxb.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/glvwelwtp.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gnbrutzai.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gebijvjfl.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gfayhxzlk.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/guxfrxyzc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gvgvjoinc.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gfihlxfsp.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gnmrrcuuj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gnoqlarwu.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gqjsfhhgm.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gynhhyiqw.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/ghffktkjx.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsnzxtili.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/giuxgwhnv.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqtoqfeoz.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gkcxrbfer.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gcqlaweff.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gzqhguuql.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gzcpbwgho.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxtzane.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gbvtskvbw.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gcjvcrwtd.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gmcrvhrej.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gtgemqoch.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gjgvshipa.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gsrdpknov.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gbstptfby.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gxqdsuwnc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gpmtrhtzi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/glxnefqar.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gcibnfqqp.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gxioqakbe.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/ghapbogaa.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gvfvsoabn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/ghdtpaqno.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gwxynhgkl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gtqxjikqf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gxzwzzkjg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gqdctjdbs.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gfcmvdgvp.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gzjexigzy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/ggxkfgwop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gfosiouha.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gizdnivgb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gzvhpzhgb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaarazjqo.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gxbyehbdb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grqhfxjzu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/galvwnkyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghiqbmqwb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwkvpzpbd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gyelegniq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gsoenoeuv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqvnafzje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbzqeffgi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gcuiedhba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggaomlbpf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gchkfqpcq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gwnchrpia.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gcvmdbdzw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbzwyppiw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gzztzwbbw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gjfumakku.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gnqhkmlej.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gjyhlovsf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gsxygshvu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gonwebdya.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gecppebwh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/guhvokfek.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gvupqmucg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gmcqocwnc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/glxufpord.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gqsxhtzkr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gsgjsjyab.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gludtpjem.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gubsipiqz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gzwqtexlx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxxooepyw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ggigsqkbm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gndcfkqwk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gpexmofns.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gwwlpiohq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gsquvpfbz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gjtwxvpxd.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gosilrmay.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gwezfeyut.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gcnxzchlw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gsaauutak.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gppzyjcgc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gvzrodary.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gnchikbrh.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gzhynobtq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gxkoyajtm.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gwubblarz.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/goyikfnqo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/glgqnydmw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnbpnnapj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gojevsrma.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gscrzyjhc.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/glixzupwi.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/giqjoddsz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gpsmtitqr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/grkqrsuxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gzanilugf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gdjrhadin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gbyzciszr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/guojpeefq.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gpxcwrwom.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/guyexvajg.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gcuacbokx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/glwbwuzxp.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gcrpwkmvz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gwdwrmeys.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gzvjkzylf.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwwqqbqqw.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gmamuwpsp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guwwekpkr.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gitiizjch.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gjggpjghp.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnwcleutt.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gxiavjnfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnoffyxsg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grgxyefoi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxtjcaomd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gzmqbfhec.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gfotegyon.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gifvehtur.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gaiclehid.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gwqbcoooh.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gjwtayzma.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gknviftev.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/ggwbwmwgj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwqkoboe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gbwyppxub.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gvhlfhqon.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gyswioelz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gkbrahsjc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gsxsmfpxz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/glotyzdwz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gdvysjxsg.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gdkmlkcms.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ggyhwspko.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/geluczevc.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gnyvcxkja.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gxavwtkru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gbymoqwos.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gfycrqvxd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gfagpglkj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/guniiirka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gvfslsbhs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gdiwftmkl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gzztyevfw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gtmfjtdik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gicchbdsa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gcdjbegid.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gzehmlfjy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gakvvrkdr.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gewpxnelh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gigrvtwso.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gflezwxoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gqfzwrtsz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gwidqwzov.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gwwzdtyay.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghuanybak.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/giizssuua.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gfjanenpj.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gcivbafpd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gwkzpggfd.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gyvbnrufd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/galiwkinu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/guqxwnlgb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gpmoqjbfe.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gvdoxecfc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gocewosqg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gatpueetj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gkvqxsxwo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/ghktrpfce.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gfdziztay.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gnuswzinw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/giyxnliuv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gdyoviwza.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gkbgxzxxg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gtveoglaz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gizhrzatn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gmdpezczp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbcbibq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ggkjnpexm.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gxsiqptsj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gewdccxyo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gssunvwdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gjxnbtxdr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gtriiqiuh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/ghjdyleuk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gffamxosd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gijtrrwgy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gfjgjxfsf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gwoketupi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gxuxqcpfo.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gtdnbrref.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gjxcjjjkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gcipgnagl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gqqtawbex.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/giwyrwmbp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gfjrnrgwv.sHtML


<!-- 参考信息 -->