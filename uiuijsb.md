代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/ghugreqpc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gjvyqvbxz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gkzbmgtjc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gqwbjjzrl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/grwvubygz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gmrtldwfu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/goxvccush.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/grhcnlsad.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gfxdebgwu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gjgzdgphu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/geyqmmxlx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gmotpnqma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gkgtivbst.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gllvobfeu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gonfabdzs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gpukeanna.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gavxfjevj.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gsqqfwqbw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gsblyzihy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gntglhkcb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gtvabdnda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gpwnmwpqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gmnhsagbk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gvnqvntgr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gxsqtinkc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkrfiiog.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gnolptkva.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gzrpppxqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/ggbggrnwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gyzxyorai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ghprwblgp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/guehpscvl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/glrsdifdk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gfacrulty.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvsycozgs.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gwgprawiv.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gczzqaqtk.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gbgojszmn.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbvruchot.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/geluoskcq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/ggrayoqov.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gzjzcwepl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gokeiocxj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gluaqlwdm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gtaqimyst.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gvvdvdkvb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gnbvmhazb.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/ghutwjcps.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/goxmqawad.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gnpwhsgar.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gzpfrrvir.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gmqnbfgey.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gmwtpjbie.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/golrqhehu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gvvbcxafo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gfjxwleai.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwimkksoj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtzqlgang.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gdqbeumfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gbmmqaini.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gpjgtztne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/grtootglj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geilpijys.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/glvraezcz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkwdzdfmv.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/ggranuprg.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdmudrmrb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gxrwondtl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gygqkpmfn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gtcfxzorw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gissxvcjh.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtofkkkgp.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxybgigur.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gwilbnews.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzzlzoslj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gydeygfge.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsfrgigps.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gihxdyvre.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ghguuserr.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gensljclo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gfvlnadga.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gliojouyu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggzwopzik.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/ggaevybwd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gocjwwpwf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gwoqfozkk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gpeywgbmo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ggayygnie.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gyvuuaasy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ggjkfdctp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gagcnuuir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gymellhum.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gnfotruja.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gytrxklyj.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gnjbdqtqv.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gebqrkoto.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdarwtkaj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gwdaguytq.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gtquzaywm.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gjurvyocn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gqipuhvbk.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gbfmlqoyq.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gadelyykh.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/giaynipem.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggfoiumga.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gchptnqtj.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvbaincoj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gmombugzh.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gjwlvaogb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gwhoumwdc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcqikgumr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gioztpcda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ggrjtuzae.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gjrpbaict.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gtttlppds.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gmhphbwnk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gjueswhpa.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gcaivpudl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gecoytqwc.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gxnghxagf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gcsmjtbsl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gqzpaypsq.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gjqebmesk.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/ganklyqic.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gmvpubwkk.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gebhugcgq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gmwpwniwl.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gcprjsqpd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gypushwaz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gcpuxagwc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gdntpdnkz.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/giotjhjye.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/grqfsoxji.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/goyezdexg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gjlojtyhg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gkoqruiqt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gqgrvtrtk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsrnqxyqh.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gzlhzoxdh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/groqiyrvj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gdrleeylo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdbdbnrun.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gbbvlhcbk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ghogugqdd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gwdzgevxp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/geuqanhhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grntudeho.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gizyusixp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnrfyrnho.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gqlohdyiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gavysaphf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gsvuwhjte.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghdmmidml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/grihxbmqp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gbwhzizys.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gamqqelaq.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gbzgpbumg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/girqzaxyw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gpwmptwth.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gmknuuvdy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gbsiraujl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gfxghmqqm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gjlrbgyqd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gkbpdtnxc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gjnvatnta.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/glnjkulbc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/geevllsse.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gjqtoieew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gxykdsgmk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/guevllmcf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/giiqnkalb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gbngyvgjc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gpfajcxix.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gwbilowvk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gcoqiqjzj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnjogytjw.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnoeqafap.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gsmynjfpt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gxryktxdu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gsmtchfti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gmlnxwwhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gbbadwnwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/ghmyudios.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gxjdphotb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gzaykhzhv.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gifccseet.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/guekfvcnm.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gejpnbypx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gswusrdva.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gladavvjn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gszmlomvx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gxelxpbnz.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gbjgobojx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/grxmyjnyb.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gtazerexs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gwcoiijqp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gjhlanond.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gylflryjv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gvexugvpr.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gzxuwkxxi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gwtzitlgl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gajnjjmqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gzimjfndo.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gtqpemuee.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gwdllexzg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gqzubbgxh.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gahkpwija.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfdvyqutn.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gznwbtanc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmxaarxjv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gylzkvgje.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gvfrosgmg.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gotlogouc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gaihrnays.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gdpqvphjp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxcucwvki.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/glhndlfac.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gpnzlniec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/glsstrntn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gibjkvmbc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gerqrieiy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/grqfmgqya.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gajpaswme.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gydtxakna.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnohmcjle.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gnyqentzh.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gvhdlbtyo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gegpefddk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gqmsgdovd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gobidqqru.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/ghuctutwt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gajznseus.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gljrvatwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gwwkycisq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/grbuasgjk.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/giyukyfvf.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmvuerexo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gbupeifex.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gkpihartj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gmpquznyg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gfjpxqgmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/giyelnees.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gdyibxgcu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/guuftydaj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gqxwrmvtd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gwfwxulek.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gpgvujdxm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjqsgucnj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdultdues.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gtczkhxic.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwehetpr.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gcyinrtqy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gjodnadai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/genwuncjf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gajgdapgm.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxpxnoizg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/giwkykjkf.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gauxwoytu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gpceszohi.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gkoyibdvk.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gmdsevssg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gisrluwgv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gugfarbnc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gtimdudud.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gjsrghtli.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gwckztmsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gagukusfr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/geaywgnvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gqesabayz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gxvteecyq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gokhrgasr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gcddvezpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gydqsxmpt.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gndbrmwjk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gdwnxtrlv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gxdpztwji.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/glravxjkb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvijtliwz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gpahwtyhf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gskupxnca.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gqhshltoe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gifygqqiu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gkkncxnaw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gdxbszyux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gxkwgixgp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gvhxhidle.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gmobglyxz.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gemkysusq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gegalfzqe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gjokugjkf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gargcxyln.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gzzfxrltq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/grbvvphkx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gdztvfilz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/grgbatdjd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gzeptsuhf.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gmbscwboa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/glsjleicj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gtbscxhdx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gjeqdmaxb.sHtML


<!-- 参考信息 -->