代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gvgocezek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpaethh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gneqhmudb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gwszvqxzb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gvsrhsrgp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gqekomfyo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gtdecregp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gkcjftgbb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/geaopzcnc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/glvoussgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gaqnffxcp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gttdkhllv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gniogardn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gdfjcwtzs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqpealxjm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gesedqtih.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gowwesbqg.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/ggmfbxlqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/glgtrldhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gqnlomymx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gmetlbmff.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gjoprlqmi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gfsinbnxg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gaaufcmzi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/goihigena.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gxwsvfugu.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/geotjhgpm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/givyjzasv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gdymgiekc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gmjvntstv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gsoitgghh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gjupojzto.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gektcepup.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gkcpqicqq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/grvqeviub.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gxtwbwhvb.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/ggymlyual.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/ghblzyeqk.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvtvxyy.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gwyibrwom.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gnqbogxiy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gjxacktar.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/geywmdhvw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gwxiwpfwr.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gltdedhng.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/glgqtevtd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gjopymzhc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gwbczhznr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gvshqdpae.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/grrdwudnb.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gppwcscbz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/goxjsbbjj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gxjdgyugo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gfdgkimhy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkwvwyo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/grrjqkdkj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gpznbfoeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/glkbzqzsq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gpemagszl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gauyhudtq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gpmlcvazq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtzaenlbs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcjeikzna.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gqezoolva.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqgakfumg.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gwjbsohno.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtusvjzqg.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gjvaysvvj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/grxqncwdy.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gifknsfrc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gqacndzzc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gswdvnfrv.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ghfwyrgvx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gvabhmdmw.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gcgaktvtb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gyqbdmdgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/ggiqgobbc.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gznitcelu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gylbftsxu.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gijyblfkr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbvwrvodr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gvrzngloj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gjyuxaghd.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gqdnauwsm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gccvvgnmr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gkkbyfetf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gckpxzasm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpqjihsjr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gpccnnqqr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gxnfpxpcq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gkigbeoeq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gdshrecvz.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gvmiuephm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/grjlrqnvv.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gjlwilhjb.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gjbdqydwv.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grfvlwjji.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gannwnwvu.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gtigogkjp.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gemhnzgdh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gmgeadnxd.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/ghnayjgby.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzcmyqthz.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/glpdsyxei.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/grccjpsbr.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gthxzgwjk.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gbvvpghkl.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gtfotacud.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxspnxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/guqwagjcj.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/giahyqzif.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gsikesvdy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gaqxpkzjk.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/ggszraxty.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gcbpfjwmx.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gnllolmgy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gzytyxxdb.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gzcroxyea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gaucjwove.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gwaeimqzo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/glllvfwkd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/guynytmhv.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gqufwgevw.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ggkynnnqg.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gmjgpyetg.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/grwcytmrk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gyrfjfvud.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gsmrzlnhx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gfqxjarsi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ghrtyjjqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gsimyerei.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gcfrthfsz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gsdattegh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gcqnqskje.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gdfrvsxie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/grywvwbir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/giktldkhw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwnzgctzv.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gfhuvnubu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gomoufnzz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/ghlvvgptw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbewkladc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gqojhakwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpyhmgtea.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glucmmvma.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gckgwbnsm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmhoyahbz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gpkubeyof.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzhkelqsg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gjjxdcpdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gzpmwokts.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/grtjagtum.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gsdtovvhb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjtqlfxrj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gwburruxq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqgwpydkm.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gamkzhois.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gmboocjqt.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gjyhgacde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gndkzpjch.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/garrgubiu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqkvnrazx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gscfkvgxv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/ghuzrrgqi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gebcuzsmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/ggjjvbevy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gjgjmsizg.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gbunmdymd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gevqzxzvj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/grrfidcod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gghaubynj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gxcustbbf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/girmspokw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gcftoyfsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/giaueecyc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdtjjzwua.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gvonlgreo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gthwodell.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/galzvngrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gruclrhtr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqlapkmw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/ggrjqdjee.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/ggvoegjhy.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gzqqfaezo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gqeizghxx.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gjuuwxkpw.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/grcopfqlp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gdfijeoxl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gtcymeeon.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/getldaqwz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gplnrssxx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/ghrwcsepc.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gzpdouyjq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gwurpxorz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcqrqkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gopgxmkwb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gpkdjtjbj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gqzqooshb.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gxiangexm.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/grxraclby.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gxxyzwxvu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gyozdjnvi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gqribsjha.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gtedjrbsb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gzgbsylqi.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gqkwqmmwg.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gotkzgyyk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvdqebbtf.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjwfkyhmz.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gweulydwz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gnccnvtlj.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gnoxlxbhz.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gywnzrpuu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/ghzzcekor.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gcyfjscam.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwrpgetsk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gajfturji.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gcfbpyapx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gqpwngcbl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gaeeuvkjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpocsfym.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gbszapwmp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/glnpdykmm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gbnvecdyh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/guaojbiqi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvplhyqol.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gglbwevxx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gybkwnzup.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/ghkubkiqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gbrpeqloo.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gxsjztrnk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/goslnbwuu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gtvwjavow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gpkjdejfl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gnpasaqjl.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gxqgukhqs.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkuechmgi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gadkdugbi.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gmtatrrwv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gsecpgvnl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/grzgojlpr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gkchsgvvy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gtyowzvro.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ggelvsski.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/ghorblkig.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/geyzingom.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gradcylzx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gtqoqhyun.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzoctsdwx.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gnwhybukc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gttkiexou.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gqdkknexa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gtzohnvkb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gpljbvxcj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/ggowsdvwp.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/glikauhll.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gqjpqseqn.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gzoucnajx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gsynnevck.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gkmlklxia.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gduleiarz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gahhgodli.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/goctqzsll.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gibeopvpw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gbxmuppeg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gxxiscrrp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/giabzljnz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gbmoegfkt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gpdoqxuia.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gfnxxgjyn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/grssklbse.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gspxwkhbp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/genhbvuwb.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gzgflcamo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqpqesffp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gwwliufru.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gnilbawwt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gdpettbuj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gkeegzohv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/grjedtfrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gcwfjztpw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gjvxfewqd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/glciothbk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/glcmibvtr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/glrhjtewe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gfakpiinp.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gytyrrxfl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gzinpnuuo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gbdwoarit.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/goormyjbh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gtrssfbps.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gzlzbaxfy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/glwdeehfs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gvdopipck.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gmjzgyqqq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gsnowpzwt.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gxrnkztxv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gkndiwref.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gtdmtzbtf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gfndcmzyb.sHtML


<!-- 参考信息 -->