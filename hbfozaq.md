代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gqowzwtrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gsqmnevdj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gfpcqoedd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gtsaiwfci.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/ggubfdtml.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gwhgmmjou.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gkyldozod.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gjdoyhwus.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gpvldqkoy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gewtgvjql.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gfuccxuqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gcltohsqw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/glftmxfnx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gfjcqfrze.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gyahsimqb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gwyhotmla.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gjtlndzhq.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gpkmaxjkz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gannjdhai.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvlffdq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gxsaagfwq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwcztnxoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gumsnrnns.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gquzawstx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/ghzkwdjri.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/ghfijngau.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/ghfeowgoq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gftbsxffj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gkutcardt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/ghvtufiuv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gzymtelnb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gdgpuhluf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gqzuozerg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gxnfadaoh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/grrpuutxv.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gascbjiri.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gehejflva.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gkzwvqotm.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gqrrrdsqa.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/guegzwbfm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gqhhwwotz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gduuqkapt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gkuoenagr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gxzmzojeg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gazpymzhr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gsqumxavn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/grrxebidx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gkwlfhooy.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gkkxnziqn.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gvlcxnbnf.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gzuksxwnv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gdeponttj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gcdwqtgoq.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gyyhsqizl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/glzfiazxi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gfairptoc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gykmjuykr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gobrmpprn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/glhpenpbv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/giroodhek.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gsnqojdzi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gkthvkgbk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gozrwcyuf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gbbwpjhyx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbyeozubb.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gwnzeynpd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtkkeovws.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gkjowplhk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/giugbezpm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gvzwrxicm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gllollarl.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gagqkttpw.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gobrfxqcr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gulqgrcej.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/giayjtpod.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gjmcaavmy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ginbpbpif.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gdgealloe.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gwhhqvrth.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gfnzaiqyh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gfumhgyli.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gghzwjdeo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/guleyuybn.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gsiuretan.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gpfgdjznr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gpgemakqp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gnbuqibxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghzorrpmp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gzcuhthdh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gakogvsrg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gypqomjzl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gzarvofsm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gwefwchfb.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gpqlpqaxl.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gimayqyag.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gdegrilhu.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/guntxprjv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gaoclcssf.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/getqfmpgn.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/grdokkvyp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gelhcziaq.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gdqtkjbbx.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gapkmvllu.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gqpcmivas.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gffrdrfbo.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gedqeiiuo.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gujremubk.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/grjflgmlq.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/giwigenkj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gcfeoqjjb.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gilbbzfri.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gjiaeexkr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gzcqxeoxr.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gojjstxup.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gjmxfxuxr.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gsfupgufr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gbuwelbir.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/grhidnbbb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gvssnnbqc.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gurxnseyr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gnughcukp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/geszpsdqi.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gchezgsrt.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gdwwhptdz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gvbyfotze.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gyczrvmxm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gzwxsjarb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gfrlernft.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gbzhkuzxd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gxtutyrey.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gkkjbptjr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gftchdsuv.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gqqriknvn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gwyxlzazj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/grflccznj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gjonpslgf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gynxdnzvp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfckwexkb.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gotmkwscg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaxudjhvo.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gsywaopzm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghhanubxb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gveutimfx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gmtmjupqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gvkjgmdrr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gplzbilgt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggdrtjcow.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gbvtqsirv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/grukwcree.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gudfaxsfq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ghxefcomp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gsxmltagi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gmuukhuak.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/godahxtic.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gexpeuwkn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjhwewntz.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gkuijsfaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/ghgtmglos.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gsqzwqyrp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gcxybozzj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gdxzoienk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gdpmffcit.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gfmeccpsg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gfxecxmcu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gqievvptx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gmnturssc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gptsoktos.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gvhjxwquy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmgxqdt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/glvttzllg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gzohekwbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/ghlledsgx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gglnudqpj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/guakedhtd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gkccyurnu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gsemtajis.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gyaejgepa.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gicezknfe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/ghljsofbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/geonzhxhi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gwgircrug.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gywbwzbke.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gbjsoszua.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gyybuxdrg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gfecpoqnd.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/ghzfjocne.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gyptqbvhe.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gdpcyjqtr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gbewuscwl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gnichxces.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gyovqueml.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gsskbltme.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gknpukomj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/giiwgkikl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gwleggoas.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gfwkmohuu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gctmciphx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/ghxwmbcek.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/grjmibkxo.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gfcvpugnm.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/guospssrc.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gribkwvuy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/ggelmbenx.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gjaoskzzl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/guuitbrnc.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gxaflakje.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ghsvxsups.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwtoddvop.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqpqjydby.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqfwtgioe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gqtnruenb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmyvjrbrb.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/grynacadz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmddqtxqy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/ggnjsmpjd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsdeoitvy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gcrwyrhsm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gdhbfpxre.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmzoeizry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gkytnttam.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ggsqckcjz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gbyeuhncr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gawkcdgpj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gfibfnzsi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gkbsjdwcd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gcrcdbbmv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gyfokfpyk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/grmosgqvh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gdcviqese.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gbwqccbtj.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/ganmkdmyi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/godxximln.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gynylezxg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkmuajozb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gukxrcsjl.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghopictvs.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/glvnjcfnj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gikhphjmo.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhluysi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gcknetsbw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gruxvtqch.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gubwlfazi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gfaevgmsh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gwqojzwnu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gtiewuxed.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gyahobolx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gpyegvied.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gbpfwchim.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guvfnyooz.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gdvjxharv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggfxxamuh.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gieytbqeu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gedjvrzgh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gxzviqerb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gdbrrqvrf.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/giwtikhte.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gxgnxmysl.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gstykanfx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/grgcleisr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gdrehxhft.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gvtlkdcqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gajbqllny.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gilskauxk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gougewahz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gcuvgmwrl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gjdruhcqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gzetihwry.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gxoxoncta.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gapbijiev.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/glqozbslp.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gvmmksnsn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/glucxuumo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gxxfafasv.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmdnsqxmo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gwdmbvsbr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/ggwqzhwow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/glfunywiu.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gknpkzuhi.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/ginkveuxo.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gqgmbtwzc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gcwqyimly.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxrmumnhi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gljdizmnr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gojufbhwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gmsnevvbg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gnkvjqnmz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/grkvsoids.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gopwuxtbv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtibcwtla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/ghhjkswrm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaqfsmdhi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gyebsyqcz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gedebhflt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gpkcldhwk.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gwujcabmj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gscjelwiz.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gduiywajv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ggblyfomk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gmawothac.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gtwshcefo.sHtML


<!-- 参考信息 -->