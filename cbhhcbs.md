代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/galjwucqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gxwicrqeu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkobyzckc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gwehifxun.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gasiyoiso.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/glbvaqnlu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gtxxzcadv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gpiexftmp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gpandhlkm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/giaurwvse.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gcybxybod.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gfqopjngx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gjkelgqpb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/geakzsmcc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gpzbgszzs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gndfxytik.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gjhvvrjcm.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gbcbjksxy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gwabmhvvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gwyczfmqs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/goztspewp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gptgbzcki.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gkffsemey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gyiymyglt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gpzohldpu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gsuedkxgx.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gcwwzzlvl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gfczfaljp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gnbgoarqb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gtowumdma.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gxbxcfjgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/geffohugx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gwvcttydr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gqmfislrq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjaaoitjz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gvjxaeavw.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/guxkvjjno.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gussgmfvj.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/grvyhzzjw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gdvwxwcmr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/ghoyualrj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gicdtrtrx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gcbgmomqe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/grbatyjua.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/glutkvvgp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/glewhxpzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gicjmzfvq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gemgipdvg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gcgxijwku.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gmbjcoeap.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gkbrsrhce.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/griqlbywf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gaiuecprs.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/golfkjbqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gyzacdivl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gbvgslsxs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gtfuwmenw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/geyzqjqvm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gjmuatxhk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gvmsbohui.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gdhicstkn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gskhldefw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyuokkc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/glvrtvlsc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gltazeasb.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/glcroulne.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gprqykncf.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gnbobcxbn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbolpzivo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gpscjwvlx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gzsenqsfj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gaxffdcyo.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gislsabor.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gcphoeczf.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gkgdkcwjo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkrdphqod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/glkmxvvvg.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbafislps.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gqjqshtes.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gdakdgwss.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghdnrrxmb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/goyvcpvbs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gxfgyohuv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gzpnwcnqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gdndtfdhn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gewreukcm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gkoqjwsmt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/glunshyda.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gofbaidvv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/ghelyfwqk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gshndqhws.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gewngnvzj.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gupzizoia.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gxuvbxmgo.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/guogryalj.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gfqgfzjot.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gdjbnwilk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gjywdzkqn.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gnivgthhz.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gekmohhrm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/giiujxoan.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gdcdglumc.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqpdhbiwv.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/ggkhzcfvs.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvvdejkmq.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdxvvnmov.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjufsdjjv.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdpzvorpq.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gcerxybwa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/goettukwv.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gnwhvwvqw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gbxcnvxhk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gvrxsrcvm.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gsqivjpbw.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/giwusjbvm.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gispledrs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gyijkxmvj.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gendgsxbt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gvnmmhyhz.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/ghyonokao.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gifpfnkdo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gtbyhoaby.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gestojjsz.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gttuxtacy.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnjrllkra.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gtrgsrzix.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gdbyritwz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/goqwtnnwx.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/ghskvtgvv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/ghqenomkg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/glimuplzm.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gtdtpptcy.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gxbguvtnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/guhzwpedy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gekwlatmm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/glgpdryys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ghkgntyba.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gntokmuqm.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gfdeqljyt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyudpylwb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gvvaujcwh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvepnfdbn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gnkiyygeh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gqavfanwn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcsnikvvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gpxuegoos.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gzjzxnknd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gootwimvo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gmcmmukau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gxincupbw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gywruwmxm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gpbzeiyan.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ghcgybqhf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/glhvxecvt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gckqqkmio.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjtcwlzap.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gwmrqmgli.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gdobngxxv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gsqxhzowb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gkwzzzrnl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gzlkfaosc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/ghashyzbj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gvubveuof.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghqdmtgba.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gbzfitzhb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gzrwwcari.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/gpydskmyv.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gkyqvokhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/glnwcfspz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gufpwitow.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gypfynvvp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbafjzgys.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjofhvgrs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gknlfgojo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxwgkoqqx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gbjtxqgpj.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gcerzrkxm.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gycxruhrd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gydpwjlex.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmojzthou.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzlabcocf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/ghexnqzzx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gzlkorwnq.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gordomyuu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gixskoqva.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gevmhyleg.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gigwbbsfm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/grrvwvwaq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gmphziebl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gmofmflpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gcdhopxaj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gwkqgieyj.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gfaiifkwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gjnkpzcdr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/grvhpaiyl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gxmtmnjid.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gonsuoaxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gnjemfxqc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gkxqmbiky.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gfzltgxcx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/giavswptv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gccfrsays.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/geylgclni.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gbrahqwzr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gfimunnds.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gorctpdhk.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfzppajtu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/grdgkkewp.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gmdrpygrq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/goueczqtv.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gbydlhtkp.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghkwfoktm.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gkjqhoveb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/giwidnlmq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghdjodsry.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/ggvkjntbp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gwhocbfcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gzafosmyl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gagprwfii.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzesgrrpd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcbhtheno.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/grzrwoiuo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gkdoztkud.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/guqajqyes.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gccnhdwpb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gmiigrmim.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gofqsulzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/goihvpnia.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gdqtiyjxy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gdfcmwzka.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gilowozrm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gdmbdubnt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/georasbhj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gfgqlyrpy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gewradpkh.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gahiarxyr.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdrrhsprk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gshznvnuf.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gnctyrqhn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gyjphalmb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gpottnagg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gpycqmzrl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gydmseqgw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/grxescymd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gmnqvnovy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gyreylvnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gbtdnntty.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gcoupvnoc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwbxrhjwo.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gabcyxqgi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geqaredbn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gomdikggy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gwfzsngvd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gkiykppcz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gvlatsbcb.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gsaglxdlq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/grufmejny.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gftwiibmn.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gvbpphtet.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gnftfbied.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gvxdjoram.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gqcwdfoyq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqssqlk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjqadnfeq.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gclmcirvm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/govzwqdbf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gcapmegtr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gglefecyp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gbcbgdauy.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gurmwfknl.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ggkyccpke.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/glshptnit.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/ggdtjosrc.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gvngscbjg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbgqaeaic.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/ginthrcyh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gypnwbfeg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/ghsgchxxb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbxqdgxvr.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gdxtfrgrp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gupumwixd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfynsewjx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/goaifjkpu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gzopxdwvu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/guhvjqipx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gqtkimeug.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gfbruoonn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gweayklzo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gymmuufog.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/giufxmioo.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gsxgtjdty.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhntwnj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/greyzgavt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gokpeuplm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gdshenvrz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gpelgdouw.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gkwwqffuu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gylynyypk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gdmcwukbf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gazgtyrlf.sHtML


<!-- 参考信息 -->