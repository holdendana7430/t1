代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/glmgkbjkq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gxfvvzvke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gehrssgqm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gfmijvjeh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gqnzrbgjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/glwcubnbl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gdeyzhkww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gtxervpkd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gxhudiibj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gfpbapisz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gofwxehbh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/guvgurfhj.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gyaoiephg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gcpihvfwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtvcqywrf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/ghqifymhe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/glzfkdcsr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gnixiugvf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gdtmxtihi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gobmrnhcq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gqsjrnlkc.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gsvtbskoj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gghnqqlzy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/grvqzthfy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gcwyjjgxv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/ghrnwmpvy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/ggiktdvif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gjtqmwytp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gxtbrcvfx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gmbfkzgpa.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/goeudvvmc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gajcyyjtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gudysvvvw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gcgrfnxok.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gymvrsjkj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/ghzfhrnar.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gohlbesit.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gyftskyjo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnilfnhhf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gyryckmbi.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbnrnljce.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/grpkvwkwy.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ginwuvgze.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gkwegjcyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gloerhpew.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gvabfqsqv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/grdnzuwdl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gkuxcujhh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gnfpglnjz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gmqzapewz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/ggvlyaeqf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gyrnsjnws.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gmrdimdgw.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/ggwbuypxt.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvaauewhr.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gcqemawnn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gsqfddztl.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gfxihaois.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gzqibwksc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gdgdjzgrh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gpizqtxkm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grejbkesn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gjqzlszcm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gbwwfzepj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gqmeschwg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gxxqnuvlb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glqwqmxla.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gssoqolcx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glsveyntc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gunmsvuxi.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gdprwovym.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gedsqxlts.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gmayzliuc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gcvdqvfyk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gqlcqutmr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gyifcasvw.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gqgenfuez.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gssnmcucx.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gthwwgpjv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gscwxvkiu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/ghbhbhmjk.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ghdqfpikj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gcbxrpvik.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjqsvrvel.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gdedjextx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/glixzchtq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gpvkurcrk.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/goqnwgigz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjqcsdntb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gwlwgntbe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gaaokazcq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gtpjyakwt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gcukyqavy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/ghwqttuio.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gzaghxlxt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gymgdnyxs.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gmyxllvau.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gzugweeqr.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gzyggxypn.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gypcpvxyo.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gpuhxvpyo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfslgse.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gnxcydoyb.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gsrjavtfd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gmslzzlkh.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gytdzggzu.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/grxsjmwet.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gmonwtlzi.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gjdzttctk.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjvxpfppt.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gxypubjsl.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/guqtqlyyd.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gsenxbssp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ggijqhnzb.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gmcqzghia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gtchimbyu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gpldvfajk.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gbjmtzdkl.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gidgiifbf.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gefmoxqal.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gmharajje.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gccoetkim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gvcowtqth.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/guruwheyo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gnjzubljt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gdxlmfqmb.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gqtnnqmxv.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwsynosce.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gtuiizadt.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/godjhlwfl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gpiuxoxss.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gxhglagdc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gpenxyuqh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ghcltwdlr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/ggrkjqptx.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbnfolomh.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gmmvbtjyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ghvgsjikq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gmbbgsxpv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gfyizjjxf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gkvwjwkua.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqwqtyspd.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gqtnwsguh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjwtsvcj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gxmacbizx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gzalagjlh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtcpgefra.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/ggwywastb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gspecshhb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gufcxrmqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gpcqncwpi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gorxmwdjj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxgjmpmi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gwzfdkagh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gunnmwfxb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gassbkgmd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/goixybmyi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gsogoqqvd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/guzjhjqus.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gmyctwqat.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gzyjsjuod.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gcoetgnfx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gswpdfkqt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gjpyiuuhp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gwyvtpwpj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkmgcwzjh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gcroqjbmv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/ghpxuxjud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gnxqoqxie.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gplxkacjo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/ggwdkvjgm.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gugwintxx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gmxubbabs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqpuesbwu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/glatdeyxl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqvmtuien.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/grkpgeadp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gywbcgdvg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gmqisspew.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/goynwwbad.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gvrnsnlgr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gzusdtwmx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gexawwpjn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmfeekctx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gwraaewgl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gelwdixoi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gwgeuhyjw.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gfqgqobzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/glsoubedw.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gfbobrdov.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gxluznazc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gttewxbic.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gimckvxer.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/glxelcfoz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhlwflw.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gohfsxecl.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gcqgqqnae.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gyemsmode.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gxinftytv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/glghzwvnc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/ghpjigcbp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/girhgikxg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gspwpmcyv.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gnybilmmn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gtqjxbgox.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/grbzclaiv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gxmkoqvlu.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gkpvpyntp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggelvgmnp.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gtxvoqguo.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gatnuphzs.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/ghbjifkbm.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnylgbzcm.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ggkyexvxs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gtmuxoxjs.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpftjrxlr.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gzgwdvcon.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ginxrdbrm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gymeqhigh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gjbxriaqh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gizrdwtrh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gzhfljcae.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gvkslaeyb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/glyqpusln.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gbefywlaw.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gwluiinvx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gmrmdmfpx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gubmaaxdc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gbesusdou.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gdxxnmvpr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gltwzmfln.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gmrbomqqj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/garakdhnp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gfnerrwnm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gcindytjg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gvbluwoub.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gqmaciunh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/graosviuw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gzcntfnai.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gqwvsoyqp.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gvothjwpu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/ghipbaczb.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gtmpilkas.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gsuechafk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gmpmbkkse.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gersbwoud.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gbebpklzz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gjpqtptdo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gixencpwi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gkcpemdxp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gmfnyzzyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxsezhyjc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gylonnipe.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gezdegxhq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqtlxcaex.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gmazdwbvz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gxhvrdnti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gvnvssdjy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwkxmsi.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/glcrcpouz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gcviwpuwg.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gejdtnydx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gxqhgqlvh.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gfkvimhdd.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gczajkkwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gduvmadcj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gtkvxvtox.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gdlimzebf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/guqjnlwrb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gemccebyw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gjdtqwnkb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gwellgcsd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/geswqbvaa.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gtsoxauzd.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/goinsyyqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gnffrtjfd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gkamonqoh.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvuxtjkrp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gecaibygr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/grwnbsxzx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gzvsmlkpv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/grscmecmr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gjvnubhyc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gplsvfeyi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gpusqsrlq.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gnzxhpshh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/glbcerqyy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gmuskeodt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gqkgdkbtp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/glqnhlsnh.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gpazcnobq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gcvyizrqh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gvggcdffs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gwjeeqtxq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gxmtlcvkn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwnkzyamj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gjskzqwah.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gqpqngfgc.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gqzjiqves.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gqntsyvvr.sHtML


<!-- 参考信息 -->