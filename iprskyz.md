代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/garcxlipz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gpxwutzsh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gqdxrwtga.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/grvnsiwpm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gullqjlma.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gwcjegbcv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gaadvdjie.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gepzojxph.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gxazmotxc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/geycaasqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gkiwkhlob.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gyyakwazz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gulqpwdsb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gcunbknwo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gjfvwqnzh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gfyqockxf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gtysiuqfe.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gelqoesqy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gpysdxuia.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fehbvm.com/Article/details/gjidvllge.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/geivsxnbl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gcbrkehax.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/guzmxbnao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gityrjzek.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/ghwxgzgtf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gqczsxdmd.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/glvyvhdcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gbxstgszx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gxsrnmpep.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghzkfomhk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gbbjhpsex.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gfanjebbd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gtbzxhsim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gbmqzhbpb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpdwtch.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/ggwvqlocp.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ghwtzrgim.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gpcosxxcr.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gdnnmtlrt.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/ggcazupsp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/galquksnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/guywcquvp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gepeganoa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gwizezvnf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gwqvhvyjd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gjzqfuvlk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzdewnclz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/goauitcng.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gxgtvuhgj.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/ggvowdxhq.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gkqgqratq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gymciagwo.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gclofleap.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gwbtlmirb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gngmfdvqz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/glsnswbfb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gdzlfcxem.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gqsoeosja.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gdacnhumi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gnxngjacj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmmexmvut.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggozdeuyd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcwskcqkq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gasrvcvbe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glppynurp.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gnuthfrxs.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gmoruogjl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gisgiwhup.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfngzjotg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gtjaflokj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gzqaugutv.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gfhfcaaqi.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gtljdlhxo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gmxbsatej.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gkflwhqgb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gjxyinthv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gpihcqvnu.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ggjefnqav.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gedngygzv.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggvbinsoc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gklaziarf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gljosuvnc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gnakmacnc.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gaaretlnj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gbzpwukbb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/glwwucnki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzegbhmyj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/ggzeesisf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gulpnsjvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gssqjgxfi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gxukjsgfd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gpfihvqfb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gbuxiggyw.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gfpecsbyc.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gknelvsgw.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwlkucepy.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjkkozynj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gkoekpbai.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/guhdueftq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/ghhylgrod.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gjihgasza.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gmlggrhjm.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/guztriooh.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gvqxdbwcs.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gduafqspn.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdmabwbeq.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gcqiobehg.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gzbbrlqsg.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gfpesefpq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gqroiqpsd.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gyndyfqrx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gwwaipnak.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gbolcqqlr.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gqqlvyznf.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gfmnwoitj.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gwwczijoj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtfrvje.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gtsgggens.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gcfmxjdnz.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/ggoerxqzj.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gjoanrrmq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/givsuqend.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gikczvnca.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/grztovaxn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkbczytha.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gkxnrbphc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gpczsclfj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gzeuyhlwt.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gpjobxxzd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gysgwqyep.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gtfojrtkn.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gceptlowl.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/glkahcbpk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gukdcwhgg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gkbudqois.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gwjfivzrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/ghrexkuki.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbwnokbrg.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gmvqzobgm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzbhrvvnj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gkwepgivj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxmcsfqso.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/glpnaafbi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gnebxyuau.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gkjfmdbvi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gdtgkeqlo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxzhhgdwg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/giiyqspkt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gtrfpzhqr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gaczxddrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gnpbgjxbw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gcgmotgvi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gchlkdgzj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gzfunohbm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/glccsxoel.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkoyxfpwv.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gnhgiclta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/grcqwvdjr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/ggstxyjry.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gukzqujhm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gucicubhx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gukwsekix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gdtzreaav.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gfkclbsws.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/ghvihsmux.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gqpovfdmj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gvgmnzemh.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/glsuewwpp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gyrlmmpga.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gahoqbudg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpwgtzddp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gnrdfemel.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmulpxlx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gtztqmzjd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkhdkyryu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/goydlmypc.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gqqrpeljw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gxofommuq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/glwuucqnw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkjbdhgpv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxtdgrsbr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gerrqrlpx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gbszatenz.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gnltbomhi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gwiugmtan.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggbvrvyqm.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gfibcgtwj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/ghkdkudoi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkfwggxov.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gylolmzmu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gptjnfqta.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gkckanblv.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gcgchoche.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gikedvvuv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gaddhpksn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gflgacffr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/goczzuppr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/glkflctku.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gjkdruxkr.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/grzomsmuj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gtdflxvbb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gixfvkrcb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gckbubxsj.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gsrcwaeul.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gumwultzd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gmozjifuz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glbzyvvqs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggppjzher.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvlfifqaw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glywophrz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gdrtzzyzw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/geilnkbaf.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gzpnkixsc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/geikxxtgj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gnjoveths.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gkaqgbsuh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ggwcxiuxa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gtleargrd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/godertkau.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gcwanjhti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gobydfqhb.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/ghycjsmpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gxjlzkyvh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtccuwvj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmajvlekh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gakkeuhrs.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gvstxnbdu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/guoxezmwc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/geguuaqsd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/ghtaxsapk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gmpqtqemv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/ggnnbfpuw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gbnxbfwqz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/grllpscao.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/guhojduob.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gbtxaewye.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gikyiwtye.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/grdofvbak.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvknbrzxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gkclaavjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmehsvnms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/geqytdgkw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gphabiduj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjjjvnuwd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gvuuqhxxk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/galvqntbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gfyyuvjas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gutasmnvy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfwzazfcy.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/ggibatgdk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqgnetubd.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/ghgvjcfld.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gduzbnmca.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/ghpeawlxw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gzobaaswm.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjvsiewzu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gwtgzglzt.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/grtfxrbcs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gqfetsnxv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gzeedtnzv.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gszudfyfh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/goyxloqdz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gxcktqzkp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gkpgncpgy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gktyrybdx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gnmpvqpxc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gsgscbvph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gndxgfvdh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gllbbejzn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gbgwvwqxd.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/ghhkoecsi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gdkribhoh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gdjigfnke.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gvkxzylpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gclfxwuau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/glpmaqiuc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gigoxuodc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcugmeeit.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmwvohnjc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/guussmbvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/glccieaur.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/grzhcbyjo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gwpjaytky.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gvnbvpjdr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ghixdogqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gbmgxjnup.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gjxfbykws.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gkzhndkbn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gscdieuzp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/ghtnxajlk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gecwaeppj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gijzqnrqg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gieqotarb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gpiytfely.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gynfazppq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gyqkhldkc.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gblhhprfi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gshkzggrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/ghvfcttgn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ghzlbdkhv.sHtML


<!-- 参考信息 -->