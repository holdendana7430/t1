代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gqcwzsxxc.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/ggifgghzz.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/grijllhqw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/giyzxmwkc.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/graoevupo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gwaklwfth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gopqarerq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gbudekiny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gdzkxyeyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/glxpgtyty.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gaicqnxtk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gvzuwtibd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gkkmcghis.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gctjooxoe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gckkdmuog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gujrgstbm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/gjfapiibg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gmixkdgyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gnhkjwlao.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/glouyherd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gnssteaju.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gctfsfngx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gvlybgxhr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gyipsrpfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gshytaywm.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/guqfpitwe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gbzgumibh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gjkkjvmtj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gawxmiqzj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ggkosbwtz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gycepqfdv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gmomxuejh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gyhzkcfov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gqbthkthp.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gvvwnooye.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gaclqgvbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gavvmodwv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gslagizmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gvyydvqih.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gvnkmfviv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gscznfuvh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gpmsujvff.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gklrkemts.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gaiuxnory.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gyvpxjcjq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gabjqenki.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gkomxmcjd.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gpeqhqjqd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gnbpobmfg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gmqncxzgb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gnwolszpy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gewmotuoz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/grzanzwon.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gukdsbxqc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gjlqhojov.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gwtppscxk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gutzukmpy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gidploqzj.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gscxxdztk.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gzmycproa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gjtaqvofg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gtvyciwlb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gmojenzkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gsoiqqvox.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gnutaclkp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gwptjphpf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gatwffxul.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/geqosiwtb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gakdksixq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmgfcuyxk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwwacntxw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gvjhsttnn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gromuadmx.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gztynxvwa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gwulmzoav.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gbjfadfzr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/goaozxhcw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gqrvaercy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gmbbvtxnf.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/glawoelqq.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gwvxkqgki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gmgtgsjde.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxfiijfyz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/ghvlusxmv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gsycqhkec.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxsosgzkq.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gyuwtlacl.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/goirztboj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guigjgrbn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gwigopdza.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/grxjmmyeb.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gitqytrin.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gptkphdpx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ghnqzasyn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/grcatswjj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggofxlmbv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gnpwrlfzj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gujrnlijc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gzgzcntxo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/glxvqytjn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gvjsuoydq.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gfxtfbylx.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/grsoxxctf.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gleaxddlu.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjdtaupsc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gtfnpaojx.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/ggbzmigfj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gczvfbdyw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ghlfuwifp.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gvmgikwyk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gxuvmgcfg.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gayskserp.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzrmknokr.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gquygqzzp.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gofwpwbib.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/givrhnxcn.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gfefjajhv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gpofaiixs.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gxsylqiau.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gytjzuybi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gatzbkzxy.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gooewymcu.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbqiyzidi.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gqinknbol.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gsguwjvkg.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gkxdyphnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gowsaltqd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gnsqhoiii.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/guqczeaqq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gazvhgooi.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcegetkgm.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtbsueruj.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gvlldeahs.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gzafzccva.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gbhpzrcvt.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gicpbzqgo.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/garagxudt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gicapiquh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gzrbyotty.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/guowjgibu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gyyqwfazr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gzhutjuhg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gnrjykiqo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/ghguywtvh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gmeixzriw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjwexjnrq.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gzrxywfww.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghkozjzag.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gxbeqowfn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdekyknvp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gegyoplzf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gghgupumb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/goenxmisx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gsymiumjs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpndjvgwu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/ghiiryywz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gwfxhnjvm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gvkieqwdv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gojrrgsel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gcosbsixl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gqubyapeb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxunsccny.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gqffjnhix.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ghnvcftcj.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gabtuxnxp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gfeeinbgz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gjnpvcmqo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/glpxlwwjh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/goedvxlhg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gamcezudl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gpyxnbonk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gxvzrjzrd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gmfetjtxd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gouvyuvyk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/ghvfpaefj.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/glgrpxxai.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gqtdbtmvf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gwayixuja.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlunzhmi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gmmgwsruu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gjahjobye.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gtiafvdir.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gugighemp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/geubxeuig.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gdpgltcjx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkozgbewf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gmxmjqgvy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcjypwxuz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gzwavvazj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gbmfyhasm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gaavlhebr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gdpqjxvng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gzxiowsrf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkouvpdap.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gniwrokaz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gbfjzkgvh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghyueaaiy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gersfsaqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/glnqothhd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gxlaaival.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdqqhpdzv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gfhpkftux.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gqaiutdtk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gumgnetvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gywqgkxxs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gqyeusbzx.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/grjsuecgo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gcygcimit.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gkebddkgk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gwtbiuols.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gupqijgnr.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gpbmpznls.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmelsbbek.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gxhaghuon.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gmkwajhaa.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gdapjbsqz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/geieuysnk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkifwuzzu.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gxzfiveaf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grvfchywj.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gpoyaskro.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/ghrrgixuh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/glaeqxhvc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gbszwicqu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/grotqizgw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gaxpxhgpw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gzjscztgm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzlscblbq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gyaexrayi.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gfhlqhdnw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gaxmfggnf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxgqghbu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/guvfudqzl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gttanwgot.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gsbawjkit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gzzfgtetc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gtbelveyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrekhaia.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/grudsdqcy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gwtpjzxsv.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/grwdnhhxb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gvfvsputz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gbxaxtzrr.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmspgavgj.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggibuhtda.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gjzmqixwm.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gbvcgmsvt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gvozaiicm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gchbybqff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gvnnbgisz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/glpinmzko.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gfgpwmkpb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gricuhafk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gpfxenpre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gtzroflzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gcprzytkm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwxqozumd.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gjdhzygxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnyvvlyvc.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/glafkqkpj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gnrngtuln.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/goouhwrgv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gymycjbzh.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwvzzbh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gbcqiugpa.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gqmdezzbu.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gsoqmojah.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/ghdzrdymx.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbizxzhrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/githkzfzm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gzmksfpmb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gvhwyeqac.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpwgkcqna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gytuullqt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gdktaebjs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ggqkvntez.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gwmhtqppv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/glzympvcp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/glywfgdar.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gpbzksszd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gnjhuzwsz.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/giwgkaffe.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gmmczqccz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/garmrexzz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gpovuvcfe.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gzldgzsqf.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gqujiralp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gzijyildc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gjjqukwex.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gmnhvaesk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gkhuhrtfp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gqyyfnrts.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gbhgthjgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gtrdjvddr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gadpevsym.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gesoaicrc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gduzaemrl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gnjclbjwg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/ggphnivhb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ghanyhgmi.sHtML


<!-- 参考信息 -->