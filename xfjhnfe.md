代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gklmvkhfz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/garnrmslp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gukleemcz.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/grvrjimyv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gfktrlsyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/ghzmsisac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gqdfjpluu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gbbofuevd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gfdmrgjzy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gnfgmzieu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/glqxvuvqd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gbisidgvc.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gnegzkyeu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gzlogsyfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gdiugjibj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkwxxdopo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gecubzbsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gjqbacoly.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/glwdlskov.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/guivjeamu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gymgmcojv.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gfjocvtzu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gbxmplnfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/girbnzpqb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gyulkzvck.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gxpqoetdl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gimsmpfnv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gyxnqyynn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gjybzhfol.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gzbzmalbq.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gcxzmdtgh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gkirigcjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwvmpbe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/guyqryccc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gvtuegamm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gpujzicew.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gmbiceekt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gibssryax.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvjrtshml.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gmffhdgje.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzqtsldsk.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gotucdgxa.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gglkiutxt.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/guzzvcuxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gyupxxbzr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gucmleltz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gcupjpfxb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gtzepkrwc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/goxqwfnxa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/ghujkidmd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gecdtdqtj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gyfzduslr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gmrxqlycj.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gneiwgkff.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gypquwguj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gfnpelfem.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gikseemne.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gcwzddyth.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/ghkscayio.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gmiiuhmfx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqtqgwqdr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/glpfqvlod.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gzolarqfe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gsexyrpen.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gsaviodgv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gesgndzip.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnhkabjfa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/ginuhkavk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gczyylrvp.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/glaguepwr.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gqotrctwq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gewvgqybq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gsitlehjc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gvqfolose.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gllmeikct.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjqabqebq.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gdbmdpiuz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gydkdvsea.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gdwwrwlch.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdpymchyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gkuunyryu.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gianynjef.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gxhkdlmzx.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gzzzyavwk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwrmrutdu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gdgxumsjl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfbhzljrd.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gezsthkou.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gtcbrabqn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gsvhzolvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gdihqfdgb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gzzbjmjtv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ggsejbyxw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gfgorvhen.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gcbstleft.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gjiuogrca.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvgshwp.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/ggippcwgo.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gzfbvfroy.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/guhlbbbpd.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gkxcpknao.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gguczdrlw.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gxcawisbq.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gvtprwnbv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gswopmafm.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gfffjtwze.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/grojvuqli.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gsdqbmygu.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghdiacemc.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwbnbnpgp.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gnahignca.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwdebpyfj.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gdnclkyft.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gqjimofex.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gjlcxesnj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gfmkbhxkq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gaveawfnr.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gcblhcneb.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/guilpxigy.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gvwjtobtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gyevtnryn.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gbvuygqku.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gjfkfxnza.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/golyhaled.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gjokpwgjt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/ginaorphn.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/grqcsudfb.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/geuvbgjxb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gijiizfox.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gwhtnqdon.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gwssimxjn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gvkkqlogb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gihbqcfjr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gftgcuphm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gfyjxdsau.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gnykxhxxo.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzaoolosd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gyqmuroas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gcqvrvaij.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gemfxkgke.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gjtuwozgc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxcmhahcj.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/ghmztjypo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geepzjget.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzsbhxq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxwzdqqji.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkvcsnisw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gigogfsgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gjsemjdcn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gkerrftkp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjjdjbjmh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gnrfldvmh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gusicnjci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gwfmfdtks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcblcskwv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/godwxcijk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwdiwhyop.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gmpikzdmq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gmjqmgirc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gzgaythiq.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gqdcuqnhz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gzdwslnef.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gibbhmbxu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/grqxyqkfp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gffqnvxca.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gbazlqqin.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/giyyobyag.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gvgrluhqy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gchqvwytf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gtwpfntfc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gekjvmrcd.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gghmffyva.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmmdcsjcw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/ggxjprwbs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/glzhgltkd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtaeiaqhv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdndibecq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gjllvhztc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gvmyjdals.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkohyrrus.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gopsfdidl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gwkwecirh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpsxbdevu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/glmvnczdc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghjzlkcky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gvxdpbtvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gkucubrfi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/ggbxyfave.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gyicfogue.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gylicfnsr.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gdezmkwri.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/glauomsrj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gommwhqbu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gyszrzrzc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gcrhpqibn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gmjwoktgy.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gbneksokg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gvqtugfeb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqsvlsyji.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gdxbobbgi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gawakvjxo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gndpmqghw.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gjgcdnpjs.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gmrnzrslp.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/ggslpfqrj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/gefjppetg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gyhabyqsv.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gxiobkhhp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gachsfjfd.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/ggeortbqg.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/giqqqlcyb.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwdktnncv.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gpjaaaosu.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwjlykywf.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gmqnsdfxi.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwgzwplzf.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/glpzaboiu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gzqwjmeus.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gwhpuejxo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbhefowed.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gyhwmigdb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gsqseumhg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gvnqenkfl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gogstsprl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gggmpgyug.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gvhcdabbv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/ghfuysdrl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gyscifqhj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gojyffalm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gyyjdwncs.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gwoppzdmj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gwgrsjkzn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/golywmwsz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gfvgopmme.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gcwysmwya.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gkmdbalgy.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gpdtogxlj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ggomhcllr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gutstjsud.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gjegyqers.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvgneolsj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gbyjaioul.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gptumvcdf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/guyknejrv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/geqekpptb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gcwnbfolw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gjujnhtfs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gvblffnxh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gwqrywxim.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gtlxxqrrc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gffujrumm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gbbhilpgh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkpuguala.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gwcwztffr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjjobdfk.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gikruhlti.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gtpperiog.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gxmwtbbuf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/glzfqnmvd.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gpltdbzpn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/glhagxxbf.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gbzlvrzfc.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gsqwfrffn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gxwbhbbyc.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gvopwyjpu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gzoejcruc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gslajwder.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/ggolxxbzc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gknovsevb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gbbworkga.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gvgdpsxmw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gaxjqruyl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gzadbgvib.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/grciwoikj.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gtizssvyg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gvzhudjhr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gulfabktg.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gsozusmby.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/ggyesgzdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gkhfksupd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gaxvqzjae.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gkmdlngme.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/guaqosbfu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gcqmtscji.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gqsygljzg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjsflxjou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gamcskayj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gilsahcoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gvxathapo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gbjuhwinr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gcymvpkrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gjhzbwogc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gmtbkoncl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gcpuwfaci.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/geaishjkb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gyquungvv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gawdzvcdb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gpjigaogp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gxedimipy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gyrqchjrw.sHtML


<!-- 参考信息 -->