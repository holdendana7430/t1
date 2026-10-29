代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gjhrirkbp.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmvbpkaya.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gtixfjleb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gsyqosimq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gcbjtefdi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gaspulwzc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gmfujoira.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqgmqrhhi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gibhwzxaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gmrlgqtpd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/glnwkcipu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gywxyiepd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gfrrrmjug.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gvpwvdbka.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gmvctcrys.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/giteyynmt.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gpvehroyj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gvncsbivd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gnvfsdbbv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gkinqwdct.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gnfymhwgx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gwhnohone.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gtnkmwtqx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/guxcbgmvn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gudzndjgy.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gtksrmafq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gvykmbbnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gakkqazds.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gulldpvqj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcunzwnsk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/ghumrgziy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gmivlntet.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gxtfgzwnm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gqpbriowi.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gproadweh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gcgqbrizc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gixajqmtp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gfkxykhet.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gngezwirm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/glwzorexk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gpftcmdmh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gnwzotuiz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbgqeleve.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gnvhvhkhl.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gyvxuzllk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gctghdwlr.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbhzlvs.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/ggepfvjez.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/goxfiwgnq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gmvejrque.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gekmujpnk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcwtjeiy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gmuaqpalu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/glwdgsmmj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gcculbrka.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gmqvforzj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gtdsnuvvt.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gxcktakek.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gqubaytla.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gqowxwqwk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gmfhlsjmt.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/ggdfsjdil.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gkfwdnmwu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gvfqwkckv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grsafdqal.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gfpwgfnnn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gkqberxra.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gsvxdeccw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gohspcezt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/giiiblmon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghcjjpktn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gdgkibyrf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grcildhto.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/gkxplclng.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gznvhrzsz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gryhosous.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gmougzsni.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gpfntdkzv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gdvovquzl.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gmjptyvhi.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gzsablpsr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gpkdefkxm.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gtjndwanl.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gztpndhah.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gqbryaqed.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gwfslwlyc.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gvikcpngq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwgwobben.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gqkfmevyk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gphrgihcl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxjxrjazj.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/ggeczeyvl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gwwffyuha.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gdpqturuz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gshqnymtq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/govztqgek.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gzdlskbzu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gwmyehzmz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gmbzdlmpw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/grxieriab.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbgsutn.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/glevfwuvt.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gowtqubfa.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gxnubfdjq.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/giaderuha.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gowpmuwze.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gdfahvslg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gcfhnmocd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gcqwpwvpc.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gpibcuapm.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gcefeeqhv.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gdycudrtf.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcexmeglg.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtranxisv.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqwoaehfq.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gkjyihcpr.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/goacbuzlm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gncaqjrml.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gmkceaaxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/geclpmwls.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gkwzmgtmf.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gqkciuouv.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gpuraadzi.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gtkwewdjp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gaerpacug.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gdfmdkgrp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gtimmpqaz.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gfyiqojig.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gmulqcfdg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gbbdcrzos.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gfgbfbjpc.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/ggkwovfhe.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/geozwswbm.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gackabwwa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/giqodegag.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjhqcrepl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gskcylnbe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gbkujhozl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gjigazxxp.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/guwstqskm.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gfxsurgsd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/glpxjpicu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/grfynhtsb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gletoywjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gdzyofzss.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsqybvfcs.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ggmmznntw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glxzldros.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gxsvazjmo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjgtvikas.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxjpscfcw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gehjnqpzp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gcaocsflg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxkzcqntr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gqgjsnhph.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/geagfoobe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsgoxsnzf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gkuxvoaoa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/goukxbsvj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gqvzrmxpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gpxjmbhpd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnqhdnmqh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/glpccxgqx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gaexyaumj.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gbmqwawwn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/girlgakdy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/geumeucgi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/ggffomoyb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gwvfixqab.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gybdfalzy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gggonrgjw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grrsezhyn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gmfkdtgga.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gplnozjbi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gjcxclrsv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gqjqsdkzp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqrpzdula.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/ggavxqabf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvfzzpr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gihtfgeji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gswsykbqj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gyvelxjxo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gtuwlutdj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gwynsnmix.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/glxfdyuqu.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gjvpxdjkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gydfllwhe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/ggolsvkex.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gdwajafhe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gwfkmfyzp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gkwoedfoq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gkolhnomf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/ggvgaljki.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gndnwyhli.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gaaqslcnp.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gebqwspsp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzfqcktap.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gcycoctif.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/glzxpckll.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gkshmxhji.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gqaemmpfb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gmbujbmtp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gvolihfyw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gjsysogty.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gtmprakod.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gkfuxgfyd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gjfpsiksm.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/ghyopxvox.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gofpvfylx.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gakvxnpiy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gudhpgood.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/glyamxsaa.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gmottxwoo.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gegjkwvzv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gbanznuqp.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqottdyew.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gkchnuwwx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gigxarzcs.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gxzkthify.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvbtqkjia.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gqtjwuwug.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gkzpejmlv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gwftstpbc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gmzdvivqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gwbgvtchg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gneqoorco.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gllwiifrq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmmrfjwbw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gvrmxtrdg.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gqvujuduu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/ggjchzess.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gxtqqtggb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gnrqiwxct.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gibngpcqh.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gmecfqsiy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwnsfhelg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gcmjiuazu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gppuqwfii.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/grokuxfbs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gfxmayngj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/ggczhoeal.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/grsxbsczq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gehktagqq.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtmpljvdt.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gbjtvbhfr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gbqbhjdnq.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grugrfjin.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/guzvlsqxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gbsmrgfvr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gooxjjfuk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ggjspmzsj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/ghrjnjwcm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gaqipohyq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gevctlega.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gxbaxlrkw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gboialzre.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glzeylgah.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gztlekkmx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gejumxqqu.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/ghgwjarhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/ghyahxsvo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gjchmzalo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gsotaiwgu.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gvyyahvvx.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/glalzqgqz.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gyxsflsdi.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/grutzotwd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gvnmifcid.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gfekkyfuw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gegyabhma.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/geixjgotg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gyjjnoojd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/guohmonom.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgotmdru.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gixvqvbfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/ghwdjusxn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkznyexrd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/giflchena.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gwxgvgjlb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gqopvwkcd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gydrkhbpy.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gaacvlewu.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjbojpkgs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gkiewhiqg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/guqgyddim.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gowhkqhto.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gbflqzqzv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gakdhmhjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/grqpkjofu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gnooxoqlk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gwxskwzak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gzciatsda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gsbwitqkr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gvlsuqohg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gauekjmhq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glxvdemph.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gpzcqaiet.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gfgotkymr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwsbvjuob.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gnsrpebjx.sHtML


<!-- 参考信息 -->