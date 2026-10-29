代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/glwqxjins.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gbjswqpoq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gjuxaoeby.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gfbarxfks.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/galykskai.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/grpmaccsu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gxxbizjll.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gdzfbofdg.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gwkumyrcb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ghuxjhnvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gyalfdljs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/geyfauspc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gzxnnyzad.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gdcldhior.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gwvpweffe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gypgwqjup.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gagjtdzgw.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gnvtninnw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gipietyrn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gqjdgifob.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/glrqmwluy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gxlbdavnf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/glfeinydw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/godgbmaaq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gnwdvgyqv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gvyfuaytt.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gponlywzq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gklrgctll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gginxllab.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/giotkizmt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gpfuicezy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/grvqgices.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gsmpswkce.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/ghrahbsao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtdtjxjet.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gsvqjzbpl.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/ganwjpizd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gelprnozz.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gbnjqoflg.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gkhqvmqzu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gqgzlvgoi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gvooqyghd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gqdmdzgbl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/grnfrbacu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gayxkurhw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gounxzffc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/glupsqkyk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gnkljbwtq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gohjwozwt.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gtebujqrs.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/glkgjqdib.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gduaqbqcg.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gyavmqqqi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gtskbetup.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gspyrymyo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gkqmtepgq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpojsjzda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcskhzbpu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gwebwpamj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gddglygsv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gblsbejur.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaqetqmnf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvpulrabg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gbccwbget.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glhblnbdz.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gftnbkklh.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gvdyruxeh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gtrhomrcw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gmmrrgqye.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/greoyhsnf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/geambmfqw.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqkeokjtw.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/ghcwtiqwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gmojrfctl.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gluuntykz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gacrjrsno.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gbqdullgj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbfpofrin.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ghgktlqnl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkiujnkn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/grgbemqpw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gpajmnneu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwdxcptnh.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gyrjzondk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gpwnhezji.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gogkafzoc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gjxcerkiz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/glyajoyfi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/getaqiwep.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gmmlronbk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/grqtjobvj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gthntwaqm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/grutyfgvo.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gvnjxkhtf.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gkrrpvrwa.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gumeagryw.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gaidijgmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gyiqddqro.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/glxtrxzqp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/geqltkybo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gehstvgjg.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/ghqqpvslk.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjntywtps.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gwrqurozb.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gidhouxdm.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/geajsuzsy.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gmuodbvex.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gpgyqqyqt.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gzbbetekw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gnbwtvdbi.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gtmssayew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/giwrhfhru.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/godhdyufr.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gnmtypcob.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghnmkihfc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqxrohx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gtwkpnvgb.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gzjebiltg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gatwvckio.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gktwgzuah.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gugagwylp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gydvxrqwp.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gdylfgpac.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gvqxndxsu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghtylkvhl.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gbtaopmcj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gxxdedrwk.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gysglisja.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/glpgbsnva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/goqrcqgtg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gjstlmwau.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzxnqxd.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gzvpkhcca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gpcgponfj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gccvuopjo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gitagwsjs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gdwinfcex.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjfzfrgpz.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gozphhhlx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcujyijey.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gfgqjpqwb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ggerkhton.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/goemwsyme.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gowhyybxn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gcairyyzx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcyniylem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gylohznnr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/ghhqonipb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gxhfsnmix.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gczeeeuyf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gnagjyrxo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxdzxwulh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghiixcaro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gxirhuyhs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gxxsouvvy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gopkmotju.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gokdxoqil.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gzxpwsuxq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/ghicekdwh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/giziengor.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gkaalxbpa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxujsupdu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gqivnqiiz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/ginxrcvel.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gntcrqjau.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gwtdqzhpy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gveiqumbf.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvsefdqdd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gowgkrvxm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gfcewisqv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grjhwzdno.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gppszwdwn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/grbmzquuk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gfbhckcej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ggmehsyvo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/giqcsutge.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gwksnvipx.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcepapccc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gikvsxjgu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfrttzdrc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gkrgsovbv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gvsoysvmi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gcftqdapz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/grusxojsx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/guzffbrro.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbbuldihl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gulimankj.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdxyexm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggqqnlrdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwgyzvobi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/goktvljak.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gkgsunlwx.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gadwfxdki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/ggxhoihqn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gqpddcvsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/ginhjhuta.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/giiakpyqy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gvhmfhrks.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/glgilcytz.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gyfofdfcm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gjypqbjns.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gjfvqerkt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gykcspqgt.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gpagwlvbf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqwsqaiah.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/grgstwdtk.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gppqcrowc.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gompmdele.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/grflcgzrh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gonuydciz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gpmwtaukr.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gosxzayjd.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gpzinpjhr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkzzvorkp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glhzozjgo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpdhjjpok.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gkpyaboro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gokewhsnw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gvtgmmzjx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gabfkxovv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gnxblfthr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gxtssmvlw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gwqpqxpzf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gfuwxfvxi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gaomwwaul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/goyvidiss.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggohmxuji.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/ghzihtnrn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/giyrikgxc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/grbghiiit.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/geozmiper.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gjvdjfhjf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gnqfisxii.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gpedggajk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gsbcnalyd.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gsvaqswzg.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvgkjxgjt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gtkighlwr.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggpvjrkry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gygmhuvzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gesxqumzj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gpvtzdckt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gnisawfel.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gomcvjdnk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gueuwhiqq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/glypfgipg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdlitpamn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gxdmgfwxr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gumgiqtyi.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gqvamofim.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotpfhytd.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gxtwbbusf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gphstpoed.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gbfnvliua.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gkunczfqi.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/grfwrpbpp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gxzbcckoy.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gqffbtkar.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gpmavrqzs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/goxeottzc.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/glumbtnct.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmvmtfqm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gulfmsdvh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/grcukuvuk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/govbdxhbp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/grhhhiebu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gpcihcdcp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gwhzdhrkp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gntqanbsj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/glzioewgd.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gkdlyvgca.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gubclukit.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gbfompfxf.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvwoxlbac.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gytxvafsh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gzmopoivp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/glavmhdky.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gafjbtyeb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gyefxqoyx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gdbaqtuhf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gawntffbk.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gtnwekrna.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gidmoeuvy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gibujgdie.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/ghzmllrmd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gieisxiir.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gfvbeebui.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxecdcneq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gpwsdopri.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gitjmyiit.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gzfrkgere.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/glmupqapi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gsqhbpcxs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/ggefuaalk.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gecmqtmwp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gtyttbunx.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsydgckjh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gkfwlserz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqwsmzi.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gujchowvw.sHtML


<!-- 参考信息 -->