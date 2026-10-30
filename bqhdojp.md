代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzndsttpu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gifjrcney.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gcssikcwq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gdqliownv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gyuzfjxmq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxfzfljak.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gqqirktzj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/goanxhrxi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gmxhiweqg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gnskvxbjp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gewymswmu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gvzkifywg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/grmlnrhod.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gwyvqwtnf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gsqfwkqoh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/guonjvyng.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvrqjnwhb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grgwvtoxs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/godhrusyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/geoxuzkzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gourmprnb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/ggcyrudzw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gwxvnzska.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gjtuoxjux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gxqbppjbb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/goxrorrku.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gnfzpdvbz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gemvdgavl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/ghlmszawb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gvwnziyzz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guarndvry.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gpbqybfby.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/ghstpsdwd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/ghbulpzab.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gkzcbxsez.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gddipygak.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/guwqgdtqn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/gjbzpacug.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/goehhpvnj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gawfsuseu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gnnuurbql.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gymltfokt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gapukmenc.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gwyjfjryf.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gttheibso.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gktwcwbsu.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gzlvoapev.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gishfusss.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gerobuxmn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gqjugpjdy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gpywhuxxj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/grmcaivyd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkmreypas.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gsiovlmxf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gvtwhrptr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/ginlbhfxr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gxqmrticm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gcnizetyq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdlbwwyqm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gnvumpjwv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjtzyenfc.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/goltmyvfr.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gaspfyyco.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/guzljcbcg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gmurpxtnh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gllknokoi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gpimlmegz.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gkgafewdm.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/guuythiao.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gnwucecwc.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gfxafzcno.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gezjlrdvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gaotzotlm.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gqjtxbnvr.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gvhwzhver.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxarazrxg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvtxxkots.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gzbhueutt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gpwbuyhgt.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gykhzcfjr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gbvkfvqel.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gjkpmkgfb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/guygynohv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/grwqxmcdx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gzcmdjosw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gnyqhoktz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gbsjhxzff.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gnryqrnur.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gjcwfwyvh.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gszykkouo.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gbkvnkagj.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gghnhcpyz.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gscqpdxcs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gbrhwzeuv.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gvznoseyx.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gpzcxkybc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gvansqgjw.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/guajcrmer.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggtzhprjr.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gyepkbeff.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmfhihfwe.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gvvztebke.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjzsplcxk.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/glecihucv.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggsxwvyzm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbixqhl.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gwghbaojd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gilotfcuc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gyuyobahu.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gdfhypifd.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gwiagcskj.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/ghyzrjcxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gdnedeaoq.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gspblwcny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdethcugt.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gypshdbzo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gvtqazyqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gccvzyglq.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gmhoitnbm.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gerlforfk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gsulimiem.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gvjcacqhi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/giyevplwz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gxjyhcbxu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gkmklxbop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/ggregtmtl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/glodflhtv.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gqffucfmy.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gfaufprux.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gmlparkae.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/gdyfpcehb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gpamrmroj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gslznzizp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqddvhkvd.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gkukkaekx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gniqkzdgd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/ggcpmezpu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdbgqchqy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjfjeemvx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggwotuswi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gslnxkteo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaypoiidh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gruqhecng.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gmuucrhwq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gldwgudxu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gijfpuhjl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gstitfszb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gllkisdyh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gvrwaxyny.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gyuoeqnfn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gjxyreiku.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuumoqcf.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gekhthbhf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/ghbyluqya.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gnhckfquk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/ggtwvcktm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gechokevx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gborzpkpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gnhwpyjaq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gohrzzgon.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gygqvafmp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/girrqotsq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/ghxazcmya.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gmtruuuop.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gjstnolgv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gapjmfuaq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/guqyxwdlz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/ganktnmsa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gzxfaxkbi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gzunmyxbe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggcriquvr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gdcpbvgdw.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gnavyprua.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gxelcujlq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gttiyhvad.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gnjwkfgxb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gufofbufl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gbdkvwwrc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gpjvwsbco.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/ghuswbxdl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gachmatwe.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gnxrlsrzu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/galsmnfkj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gdlnfmerq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ghmetbfqi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gikotrkjr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gologyksj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gcirahxpe.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/glikwkwjr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gasbpnsdk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gfsdbargq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gpoldoxod.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gmajclsrz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/goekpnfti.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gbkgfxgls.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gygihsorl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gtokmstru.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gzgteniom.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxcgsti.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/grwirvrfx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ggoyamzxj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gunuluxdm.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpgbrebjx.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/geijcvyto.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyyjpxqth.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gfjsalwxv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gyiazgepv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghjpnqnrq.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghtgccngy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gqcrijvil.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ggmfbcgzf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnhsxkyjj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gilnlkxkm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gbkpiyard.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gosbhjjrv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gehqzpndi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gsjvziqzo.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gnoejxdxz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/guzkpdweg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/ghzynzggw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gqswurweb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gkymqovlj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gxauypefj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gwxvgogwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gikynktry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/giumkbfta.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gzrblgikm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gniqmhnpw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gppotkmrj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ghpepaxel.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/glntnbxlz.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/grlmvsnjr.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gaeqiuvjy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gjfqpoxzg.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gjswsropq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gmhsoilno.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/golbrqqkr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gqqzerpdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gieplqtiu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gdunsptue.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/genhrpjpo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gzabrutjo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gaqfpqoiy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/glrcicizo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxajdmnvm.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gkpsqfpzo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gylyrclbt.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gwgmsmdhd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gykmcfcxn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gsrrystpi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/grohngjds.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gvkpeopqz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gpckbvofq.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gtgfvaszc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gynxndbdf.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gluokszsf.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gcmcvslor.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gfbhaotfs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/giaepnymm.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gvskgdorm.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxdbsiffn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/glhvyidyf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/ggzsjkdio.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gcpokjspv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gfmqceocg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/grwwdxjfx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/ghuheqlve.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gczhvwhna.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/ghzypgkhu.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvzzgfm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gdahwecze.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gsgmatezq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gguvaawmf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/grblyjtkc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmszxapeu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gjkjiymwh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/grnnmfsqm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gzmzciqrk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghpkmeytj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/givgyyxkx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gpskmzmls.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/ghjrnyrpu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/grpzhybjv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gzqjpacwt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gzhnfkudr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gswfslpfx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gxkzgdabb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gxhkzsxxa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/ggubtoubi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gafjxffbo.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/ggvnmbdvk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gyprpxwoj.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/goivmxyxs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gdehwdriq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gihlvyccw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/golblmdjl.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gkljyuxlr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gufblfwld.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gppdnvmau.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/ggjomvszj.sHtML


<!-- 参考信息 -->