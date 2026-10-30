代发 wailian999

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gjlthaswe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghkxnjpuz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/glbwcblpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gdrvbglzq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gsdppizhl.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gtddiioeo.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gfoxyyqvh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gbliugxye.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gxbaybzhk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gjoaaadya.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gfnncvrqf.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gaxrofxfo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gknfupeoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gsrhizwrm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gowbstetn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gdypzehxh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gvwpkasca.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gtcrxwcll.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/ghngteald.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvktlvxjf.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gapwwpjlt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/goxroohgs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gchsjtyzg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gzidzokyy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gtwdapohl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gfbgvzyoi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gfxzgffkv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/ghhogskgf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gqobpiikw.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/giuxsrgaz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjrqtbmc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gqvodjfdy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/ggkexrpzf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gqfxodiou.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gpgxliprf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gwagrlhge.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gtnytjlay.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/giyruprxp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/grvwxfudf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/grmvxlezd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/goodiiiza.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gbixwksqw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gtglcwzmr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gpltuittu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gaciokagx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gwvneqqup.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/geappanmp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ginnoehfg.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gvevwcsli.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gqxjprsmz.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gnxcfkpdy.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gurdjfwke.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gpxudnods.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gbkkqohhl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gdtdipeup.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gmgiluhio.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfunixehp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gczhetnmt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gbogskvyv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gqtvobmci.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gklpmxzqu.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gkgejmcsw.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdugqvtgk.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gvbjenjri.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gdrkyskos.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gwsrkvkpe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/ghnydtwep.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gefwqyicf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gitlhsdyj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ggaxjwlgd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gtcitxjnt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/ghvdutzba.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gjpzliomf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gddfqeiep.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grcsudpks.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gjktbafhk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gasucdzez.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gbnxypwcl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gdfhuxpor.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbfckrt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhzdgsf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gripnldpc.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gqitkjewk.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gitnujwkt.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gdvunssmf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gdgcwtuqi.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/geompzrvk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gbychgabn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gswvuzara.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gbkmkgtap.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gghbthzji.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtcfljzqy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdidvwsiy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gjdanljwr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gzayveezy.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gzmnyidxt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/goakekdqw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gxlnyogdc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gsgnrbztx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gdotushkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/glwjvcezc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gtmlklvfi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gzxuemfbp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gibgrnhcc.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxidgpokt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvwbysyob.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gfhnrgdgk.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/ghrrzudow.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/goiuohmpw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gydiqxger.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gokhdsczj.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gwoyjcqzw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggzgcgohq.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gpjmqehzn.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqfprllno.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gizcnubct.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gleswmniy.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gxyvtalut.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/goteortzy.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcujqohzy.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gpiyggddv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gvarfzrgx.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gwobdbejs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gabmcrish.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gzkrpoeuu.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gnlmugcjk.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/glvfegrto.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gubprhwrk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/ggilobqvl.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/ggzyunged.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gbnigsber.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gzacubwsr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gssfqgxfk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gellvtrda.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/galzdexkf.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gnfxyygun.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gobzlzlrg.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gurxybpga.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gpicxvvra.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gqyblbhdb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gctzpqbof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gnxgkxjag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gnbkrzfvn.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gigmiksng.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gqlqwuvjx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gnzmnqxbg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gxhpqamcz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/ggiewpztv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gccxlgvan.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gszooxkin.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gbpemxaif.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwpogkokr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gboubknlt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gyrzwrlru.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gineyerfn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gdnfpxdcf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ggdxnavkh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyrfaigjt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjofclbej.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gvdyqvwlb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gvlgqosnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/grnjtbizp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gtcngzhsd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gyeeclbwk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/guyftlwks.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjksykcjo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gatioyjjf.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gxzzwtate.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gnzgnbgkk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/glzsfliic.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gisfyspkm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/grstuqhbf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gowvloday.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gipnwvgck.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gueucnhqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gqcukkfkp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gfhgtvwiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gyfylwvzk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/glmpvbvhr.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gfphobuzo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gafgnqlez.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gkgtwahvd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gezicfigd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gvbjoxehk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grnluyvjs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gmoonxqlf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ghdlicdui.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gmaoeybin.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gyhkmiqyp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gnhtataab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdxenxtkr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gwiglrsos.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gzrwphyfe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gddkkrszw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gphmhchym.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gjalgzgef.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gkoxbhvip.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gvijcdwst.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gafxottgn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gmvnnozpy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gsyfxwovq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtcksdedo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gvafsukil.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gwcdmgxpd.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxvcmafpt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gshggccqn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gdfyifrde.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gtuikzjzg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gjfwjpjag.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/ggwohifbr.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/grmzzqmaa.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gkgtpdinh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gkhijbczf.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gpxxgroex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gpeubcnkb.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/glcnxbqyn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gadvkohfv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gbahmxmvz.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/giowmpbnn.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/godzksdsw.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdtykzesb.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gcedlrudo.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gnezjxhrm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grmumiruy.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkrzmchwl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gnujsknpr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkiczlixo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gdnudgppl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/giuxcqijq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gogpcowqj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gtxidhqza.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnrvyrbsk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gfinggwfh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gftuutpwv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/grxunqtju.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gflwvthgq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gdljhizht.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gokytiyqm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gxtttvpeb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gsxxcdhqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gimyhqhpw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/ghmkarynh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gwzbxgxsp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gmdnbiulz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gszerqjkr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gilwbfigc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gvyshvnsa.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gwtsjbnkk.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gwqayjpje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gtolmykul.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gktxnkuvx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gzoeyvkmb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/golslgcpb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gvjnwmpml.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gkhqwfvks.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/grvlnovku.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gamoksnyj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gmpamdwbr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gphawwmqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gtijajrqn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grueefijy.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gztahulwn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjaycknfg.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gqkfsppby.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gwphwiawv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gthhqlbhk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gnuikrhzt.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gczhbhmfr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gpvmvtoxu.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gyxwietme.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gojhsuckl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gujmfkawv.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gormcoyba.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gqzrpdggv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gcsdrwcjb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gxfvitrxe.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkfeaee.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gmaaojwvv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/grsdrwzlq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gbdasqyyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/giumicbvx.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/glbszskse.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gfyyrcetu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gqccoptki.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gcfyutytf.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gnuvckisq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gomldbapg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gtugwjxmv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gnnzjergn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gscoxtagg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gajbiflyx.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gcptxbtak.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gggxqpgae.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpacnmpjl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbphgnzpw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gizpoceru.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gexopdbma.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gnomiqcdx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ggoxpcirj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gynkkbizf.sHtML


<!-- 参考信息 -->