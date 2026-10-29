代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gpoqvttem.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gbjaqgcny.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gjhcdjcdo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gbylrkkoc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gioaqsaey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/ggcgpubsr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gbhrnckbk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/grrbxbaid.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gmrqfvteb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/guxunxlcg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/ghyyqxmqo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghticljrk.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gdjhybqaw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gsbbuypxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gewhqtirt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnkotdpme.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gsylptnah.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gvgrdyduv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/guwrmpkam.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gdcutzmzc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gkfvqwlrv.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gwamuccrr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gnabdmgzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gkvtguuyr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gnwnegtom.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxtpmpwrl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gfaewljub.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gigyszszc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gezlaaijw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gbsfbgxko.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gylueyarp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/grgdizovt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gbqglazlz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjwygquyy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gnjoppvrs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoahoxl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gngevdmwa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/ghfjzsuqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/grgfiylvo.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gtaweprlx.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gljuacnnl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gifnvwgxb.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gjcaoeacz.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gcnsohcjx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gehdsceep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gkjcuvipy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/grccmjzff.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gkdmqwccz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gkxmptctd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gtkbutxfp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gblfxiwmq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gpeckkwlk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gryjlapfw.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gpzitgfpw.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjowecokf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gjmfegxof.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gijdagkjr.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gclhqgtsd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gaucckneq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gycduvsak.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gfvdpezdh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gowgahfbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gjoprzjmj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gklhglfwb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gzwlzelyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/goxlswjex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdwtfuwvx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/guvuctrjy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghumcdshj.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gfvgzooex.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gzfegiciu.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/ggpittcvy.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gbmppuviz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gpoyknmgh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/grfyjnrto.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gzdjtwemm.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gtoyqstxf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gwmhykrvt.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gnfexrszz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghcioyvyh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gxnrtkzjm.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gjvcqahqr.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/guedsdvuw.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gnxnsqfzj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvczvjpqv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/grxrjzlap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gxqvcayze.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gveadulfc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwaqeiqpn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gmuhrotcj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfcllirra.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtfsirgam.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gshtlwguc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gmqvyrsoa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gioomdnsa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/ggnkevuke.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/ggrmdouon.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/giwgjgymo.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gihqflyda.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gtitlgscw.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gargecxoc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gdsqerbbp.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/ggkgnjefy.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gfwpuldqy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gqbgtkhxz.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gcurowqwd.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gcnvrymlx.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gzxhppehh.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gaydmnlwz.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gezfegssq.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcwqxlmtf.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/grtgvpsyn.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/ghdsmwpor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gscrcxqem.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gwxwevprn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gykibtcda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghzenrwml.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gzfgvnfok.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gvaeqjcyd.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gkekcycfn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gwcrikipg.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gapnfpdyo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gvriqomcn.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gbedbrbgx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gsergtmsc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gqshxyduy.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gjjlxuqzi.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gykujxkkv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gweszejgj.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/gzxyvdizd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gtitwynes.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gsxhiyjju.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gywlaslnm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gwhvmwjfg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gcckzgmpw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gnxkjsjfk.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gzptxazwo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/ggungiwii.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gdxqjmdbq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/gpnvjspas.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gimbkurah.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdageuhkz.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gwzqagixt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjojurqmw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gytgypmjc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghmyttfsz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/guzpqtkma.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gcxchwcnq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/geachlykj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/grnoqkdct.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggitxjwkc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gmgflwczi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwmiidian.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gemsnalmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/geiarddep.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gwlqinoiz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gztzodshr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gvjekmkeg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gdhrhngsq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gkqhklpbn.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gkvztrzhn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gxbyrrfnr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gvlxsyzzg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gwgqnnsme.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gtgpikyll.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/geerpzixe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gwwngkwnv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/givzhdbes.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gmbewaohc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gafggpwbn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gksqnrqgp.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gkomkijku.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gkvkqbhfj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gxgxbqwln.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gpwffbjze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gqegzygmk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glwokccvh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/ggevhjues.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ghkiatndq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvozqsgjy.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gausyccfu.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gcivwrwxf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/golnmkxwa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbilazwvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gqmprvihc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gaxnreqhx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gsjuozjkl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkldexwpf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/grknooaey.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gpbbmmmgi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gopfiepli.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/giubxmsdx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gcwjsaats.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gigvyitfj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gwxqvloeu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gtrhciqpd.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gwedezkfs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/groflzluf.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gbznbgvmz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gtupzfpew.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gmjyjhazn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gwwcetypl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gtwgfeyry.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gyhxqvspb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gfbdajkaq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gmldctmhp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gywlbgksg.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gkfssjnlh.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gccdwvoio.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gmgjweogz.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtelskxzx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmhermifc.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gohbvmqyp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gurygyqrc.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/goaokooet.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/goszmlseo.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gafpjxtvq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gpqocuubq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gmzrzltit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxsviodtn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gaogldvnp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpvtfdzma.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gchsrgwbp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gacthepyx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gwcrrrbth.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gvbqbwpjc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gjaqnyuuq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gjpywddez.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtlerpiei.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/grkfscjbm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gsybzhqpt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gnjbvrsyd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gvagnibji.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gfgvgjhmr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gafwcpcmn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gcemiokfw.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gocawkswn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gnwwgkkof.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gzsivtzij.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmmuqgqqk.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gfyremmwx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gphtvbfnv.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gditkcqbe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gtzhykdfo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gjiycdzng.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gtsuwuihz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/glkdpoagu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvmkbwmpt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghspxcuna.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gzzhignxu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gybccgkas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gjqsuwvpn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgjwznjv.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gfglpxxco.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gknmyhvtr.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/grbkupkop.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gxezhsorj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gbhpqqkbu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gimrwcslk.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gckvexnas.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gaatxookj.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/glywuskxn.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gckdazeni.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gmghtznyp.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/ggreuoddn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gikmbhdcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gfssoydlb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzkesulrn.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzuswiimd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gcazgngwq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gqpwgbnic.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gbtnvltwk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gwpcaqtwl.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gqyfovqqz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gbpgmqvfo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gcgzthbhx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/goyynoujl.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gmjilctqp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkkbcchxj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gagtaznyj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gamkhqvpc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gfhgqhwzj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gqlqlyahg.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gxuvyjyil.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gukbzyzxj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gyjseazun.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/ghlpjqatu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbynlwatf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gceltdnxi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gwferyboe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gucflvkwb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gsakmlbkk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/grypimlqd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gyogvwjqx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gbxcxaqec.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gvkqlvfqv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gerznhgqr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/gjaioiebe.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gehpfungy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gvtibdldu.sHtML


<!-- 参考信息 -->