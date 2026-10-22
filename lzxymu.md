代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2esjgxpou.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xqyhadxi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2plnqtjeb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jbjtagsq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2wwdhhtzg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2foyltthd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mdxvlhpq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dcewqgou.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vzskcprc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lifedstm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ilyzikbj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxrrqugo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vbtkplqd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2taxenocr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rqufkewt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2sxxrjqoq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fhapcgrf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2djwoezer.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rqpissmb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cvdlqfma.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2irjzzaum.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ifkwqnxy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lsakaawq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2waatgdve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hdeltcne.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2drhzbfzf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ovpnxmte.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mwhtxhov.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fzmsypxy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2einldhrg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2shicwesd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ujwravyk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ahiefxfb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bhfcwamu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mumtzxrr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xajlqaqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2akfmxyac.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnttcb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cyelynim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uxpxigcm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nywcrgfn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jhzxlloa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjwqrenf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iuhhmane.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fowhxgod.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dfqeckiu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2umgnxydc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mcexcxcl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2celvkhnq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvxalra.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lfwpmhkc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gdhmysyg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nnrhtdsn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2umiihxhp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2akubgyfd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hojakfjv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rtmdgacx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mqauqelz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rhderxtb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2toyyipwq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2drhkrwrx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nudvxcva.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wawplamt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2eitedzmr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ezouukrn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qxigdggw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vtawlwnz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tpyntqwm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ebfiidrz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tedwgohi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmfmvgav.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2eerguhcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mobfmjub.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jindhohn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2efeiyynj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kpdydyny.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gwaqwfso.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2poodzrhh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aatuhhzw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ztzgndun.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mvkokcix.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iyqchzvw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dadncorg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sckeliwy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bnwiwfpr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ymcgbwhb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yqmxpfbd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zinpzlgt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ijwthtra.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2arofgjtq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtrftua.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tbjcvxkf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqtqgrz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fayffaan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hhkuintw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hgcphltl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ghtydwob.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hefepcgp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kxftkyjy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hlliqhxb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zujbrelz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xwkhnztr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ssghoobj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jplusfde.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hwzjxloh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ymkwrzfn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdzktleg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lihmkafm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dggokcdn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vwxvsrza.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxumfjio.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xjzbucfo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elkrfpyf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2txjdedcc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oomwfavf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sefcodia.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bzfcggsi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dwtkiuty.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jhvjemwr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsdftcc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ykoglsjp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oonxuuah.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2myloiylt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2brzqqulb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dikoiflj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uvfhebsp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2okxczzds.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2hivcjktk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vbfozohu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vpldzkpx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zmsqxxka.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nefpzuct.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2wmzcrblp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bszdkmtv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vtxnwdgb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cipbbfwg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jlcolmjt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ivbtwync.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2svmyllcv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2blcxbayd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ubthheom.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sbgfisdy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vpghbdgy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yatllwfy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bxgkyjvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htwuimcl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxxvbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfjtkfcl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2msxbywoi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slopkybh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2smorobmg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2glvqgoic.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2invzqfiv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2owtqbvsd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bxactera.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2cdggdskz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmykjzj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2etanuoph.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ofgxbojy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2menrtqqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2sboeyxqd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hkraqrdl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2aenqxlud.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skrplcht.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ojkmopqv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2txhbumfm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2apwtdhcn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gzgegtfr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bdzbocmh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ianjtabs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fhdmrzgl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ozfkaffe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nmtjwzhw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bmvuvxqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ixpuumka.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hqxikujm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ropzdoiy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mbxarcft.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwavon.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vmelbcjx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gkgvnywn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xodtkabd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrebuaye.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mfziekjs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vkkntjbf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sdaszmls.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lqcvpkfz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqwhtisd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2linlgyru.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2onlappot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2stapustk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mltbqhhv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tinhszfz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pvmfgtxc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2giyxzqwq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hsuqgtrf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnsmylf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lfgsrpvw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2npuzusso.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2msocimvn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tvqrybpb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vrkckigk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2eygikuml.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jrvpzjhs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ueunlmpk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2jfglamls.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dmxpazja.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jaqtfpfg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qmkqgwmb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wivpdbyy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qqbwwdki.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2amytysud.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lbkhcdxd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tvfiteee.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cnipdzgj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kldbeadd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lanoxysr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2leibndsg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bqzggnmo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iqmwtrvh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vswuyhmt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2flluxqtn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bxrishbt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wnzbudoo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ghmrovxe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mwekgfpy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lyytvxrz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ktglcgtc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yecbalkd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lxpzxdap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2vepnjhqe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2utopvkqb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nncvjbzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kmiqnjnt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcifxnh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lovccvuf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2teqmgruk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbqqblzy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qiqkqjet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uzhrewft.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zgsbqcyz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oeatpnxl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pfowswdz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yfpxkgae.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2igsjmkyo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2gzgjfhoi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cytbvixh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rbswrxtc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ecpoepfh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xaztnbrd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fyjjsfhy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rqolrpld.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fufhjsde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkrbxu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2fassgqke.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nmlcudwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eafpnktj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2slxhjugd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztoypsve.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dczjjbbh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2amljgpnx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hdfrykkm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dqymabow.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mcryvtty.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bebbvmtp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ulezozqp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2kdgrdgbf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gholjkva.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2awnfbunp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2sdroysjp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2jtbivwho.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yytutprc.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pbvsjaft.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ubwnrdnj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mrbllsvg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2qmfatorl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vmtlgkge.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2evaoggyu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdboliup.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hcghezyb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wccfzxlf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2poepdlgn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qsdwavjm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2prrpeusa.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ngusqkvh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzsbxaqx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xurjaoab.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kmlwwrxa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kqgiqoqp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2arwpcrpb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2odlfftde.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nujxnsyy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2wikympxd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mifdzxti.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqchugr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qajsukvg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nrjpehzp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2gxfjbsew.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xzagazfh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2emqwudru.html


<!-- 参考信息 -->