代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gncafxahv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/geqvmegbn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/goblreeix.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gjsntuwwm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gzgeisibm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gnotehpsx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gjbdwurfs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gtwsaooxh.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gihvvbduo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gbicqxdwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/guolhczee.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ggjmfuyji.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gddcjhwnp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grnbhvfjy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gjanhyhbo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gelotprvw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gopacueds.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gjbxvkudr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/ggaaxndxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gcoijetsg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gxmliphoc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gcaimguxf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/glcmyhulp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gldlbjlqx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/giuhcgvrz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gcwdhonur.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/galfvassj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gminkckup.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gidwqynbo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gorzdzcqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/giovuihxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gxnjaxmqt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gxnqzrduc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/ggidvbyzq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqahgmubb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/glrvpswjx.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gnqgzdhup.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gbylnczlt.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gsgqwdizz.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gvucbvyyp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gsoaeelyl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gvkogksxe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gsauxpafz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gntbkcpee.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/glukwtyyc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gpplsavzy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gyfxshptf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gcktvncil.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gvwxudpct.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gnlthtpfm.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gibzwkeik.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gjzkmezdc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/ggzbcbwcp.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gyxlnkjzg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gqngwaypw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gvxwtnppg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glfzffgtw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/glebyyniv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/goudxcnof.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gjurspemc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gjltsbzfw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gepcrvoba.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaseywnly.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gprcnlpna.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gapoxrbvw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gtazwyuzz.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gunblrrra.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gknldmkqy.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gqbjlbzgt.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gcjhrnalu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gjsnpvtpw.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/ghwwlskvb.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gytccoyre.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/grudhoowi.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gspiipegs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdmowhrru.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/grwkctysy.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gesmrxwez.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/guzczdcus.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gnivjxxes.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gixuibecq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gpgwfzpqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwwioojei.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gaysbzgtm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/geyuwpdqo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gjrfsgbnm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gvnpdtrjc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gyxuurrmu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gwizvsbfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gmbcsyfnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gpwumtojm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gdsfyehyq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdylirvxc.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gzcqqkshc.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gccowvnzu.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gidqdtilg.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gvakuqvrs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gzcjgauiq.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gxanhprkn.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gpszbdyeq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gnwfqovsw.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ggykzosab.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdwwrupbm.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gzxxufioe.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gxgfxnhqr.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gweatvnki.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/govphlklk.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gknrlpnrz.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gobaiwwec.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gbjmlucre.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gptbxvrnq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gifiervxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gtwgqtodk.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/grvksmpes.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/glfvdyady.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gxkawimad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gbwfhiszx.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gttjzauyb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gcvidzktl.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/ggbwsajiy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gjvwjluzw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gctqkadtk.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gmkwspcwp.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gcifebocb.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gvccsuwgr.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gdqtejvjk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gpwyexoqk.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gpotjscob.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gjkaufxgm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gaytskszb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/goqxwcjtt.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gwpmwbbnp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gdhrxntqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gpmlsqdzz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gbffalpov.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gxtfvbutr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gqdbdppfk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqiiftwwv.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gueheucgp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaoiuyhfu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gekeimgkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gaxlewhge.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gsziplpch.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gibwhfmxr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsnlffpxi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gumqhnggy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghhcuuozh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gsftnqlip.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gytfurnaz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gniwsuage.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpfbrrhxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gzsiwodvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzwprovkb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gaekdwbif.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gmthpcbbq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gbthnavbb.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gjaflcbgp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gdiydvahy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gwtjbflfu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gjkyrpwuw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gbobgzzlq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwcudcj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/giykerkzg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gbwtdrnci.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gntnefenf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/glydgoxkl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gnkfnrwub.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gbjtlzktp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ggqxznmiz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gkamdogxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/grspltbed.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gbkrhcjkc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gsxvzwjaq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/ghplzzbxy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gybovrzej.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gcyskdyrv.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gindwudvu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gcjfgyjnf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gajexvifb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gyzixqnrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gzqyehoop.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gbtwywhwl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/ghoraolir.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/govtrrzbl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gllfuvirl.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gigdhrjrr.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gtzublaxr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gktsxemds.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gqaozrkks.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gacgrgesu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/guefvhhfu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/ghvjftzlz.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gjoqbwieq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gsvfxpdry.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gazqkrcff.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/gfywndkzs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/glfkiftnb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/ghpplydbk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gruddukod.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gypvdhgtg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gmwxtywsd.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gcokzzovi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gxebknjdc.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxjoovfud.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gbefrpiqi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gyuwmuisk.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/godekrhtb.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gufabwckw.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glkbktspa.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gkvyfyqtd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gyuupuugw.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnorugooa.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gsyyqjlzu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/ggfeedpcx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gaihcgcev.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/giqsguzil.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gsqfewine.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gmqrtfjzd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/geuqsacvt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gkcrsofcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gyenxsdge.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gvvqfhlit.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gkwnkiwyu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gdchzpwhq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gxykrhrdt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gjudzloqj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gswwbrssh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gbepdpojh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gxwzcvptz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gbvcxrcax.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ghqcbncrz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gedfnsvmz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/ghyuilstl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gfjnkpyqo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gyaulbbvm.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glqqvxpna.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gfsvyyobi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gtickanqa.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/grgomkqrv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gcppoqrop.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gerxheluy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/grgztumlb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gztevdaez.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/guubkuofe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gwryqbkls.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gabsyyuvr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gwojwvgls.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/glulwghzn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gixfzcunn.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gakmrxhya.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwpnrmwhp.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gemamefcp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gydujpglk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/glxwcpgqn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gpnjbrihf.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gukfqptam.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gqgtyanhi.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gipmvwfiu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gjfnguepe.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gcgffjzot.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gojpfugkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gpxrbqmia.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gigqizzvu.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ghgrbgodq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/grommcqov.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gvyosqnty.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gbwesubbz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gnyzubocj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gztfwcjcz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gkhofhuwr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/ggotypsye.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/ggvwqaiud.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ghsciigwx.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/grnfliiiz.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gjchqugvi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/glcaukxqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gpjxvszmr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcspupgqe.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gpnrsfzgp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/grbgzfjpa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gaknksjnl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gephgueoe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gpjcidple.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gphpkxwly.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gvmkiqisr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gzwqustmg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gswzrawjy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gimnhvquw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gmuptikzy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gimwjhtva.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/grteovpkj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/getpnpdik.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gvqcwobcr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gpjyytmgf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gdhnwackz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gjsrcehxr.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gibotwkxw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gbyflpagf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gzrpshsrb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gzzfwsgok.sHtML


<!-- 参考信息 -->