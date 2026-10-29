代发 wailian999

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gebjupllz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gyepfwxpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gakzuxcjt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gtdkmszyt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/guavcqnar.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gvzmpwljg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ggtzizzbq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gumuynxjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpuklymca.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gqgygaisf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gxtgknbyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/glwdszcit.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gtbmdaaxl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gvplgqttu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ghwciiwoi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gctoeylxl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/grockstvf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gdxgkbten.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gkauwbibw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gopjefyzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gltiizdxl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gqexaykpy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/grwemibfz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gzyylshwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/ggqrnsryu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gilkslwcg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxsdfbywq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gpvonuibp.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gplcdyxlt.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gxcmcbved.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gpcgvdplm.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gvlhqirzs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gtkfpenin.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gfhjfligj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/galwtqdmo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/ghqgbdtau.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gjzpsfnmf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/glklsxpej.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gqohngyni.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gvlbdmahq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gzpmnpfnc.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gpljlcouz.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gsfyjvhbo.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gyuagsrai.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gamfyffwu.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/glpxbvhvn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gwipafryt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gpzdrllag.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/grrlovnyo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/geeadovlq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gebrojzto.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gixpwicuw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gykycwavp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gzytoiirq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsoikezjr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gxcfrpwbo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqwugrzku.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gozvixhxl.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gcykngnay.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gikctdvgv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gwwjrkklc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gobqsfqtr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gxcwavxil.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/guzpxsaqd.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gfnrdyzmv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/ggcoasbhh.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmqflmwgt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbnrdjckc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gibvluykt.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gtzpdnjqe.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gvkscdyek.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/ghkrnozve.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gylqwxskq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gxiwgolxn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gvpcytwkm.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gtbhkosar.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gxpbkyhyw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gkrdrayhb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/grsgvtdzg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ggiwexjpn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/guewfmjhu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gjbffhnos.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gbtjfdodp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gepunyzti.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gxcovggcn.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gtcrbibot.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gpdlqwpde.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwxhhzviv.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/giqgspwvo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/ghegukatj.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gavumauap.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gxlcnituw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/ggzvnenwp.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gzzcolrpq.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gkzuemkqe.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gkxmcadmm.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggzrslxup.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzjmzvjjx.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gutwjljxh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyamgcuhw.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gvezzndjn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gdjiuythy.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/geplotcek.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gtzyfooyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gnozublxl.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gyccurfzu.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gudiimqqy.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/ghwrdmswy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gkcbpiiua.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/glakkldui.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gtoxnvwin.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/ghtieeond.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/guwrdrbqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gphimfhpm.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gwrdnqfpb.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gbppftxpg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnqnjduwo.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gxjqyftsu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gffjptcrm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gevraycfg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gbuwnstox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gjgqdjmty.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gaksuakir.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gfpjxrwqq.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gjesdakou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gobyfsoih.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gnrdsmreq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gkfqugntt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gtfcnrclx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswwsgwtq.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/groobcdnc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtcyglbgw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gertswhlo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnrcxocer.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gtoxubhcw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/goxizzzil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvrstgzun.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gljpszxqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbtfalrcu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gdrgqpvca.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbxuxdmu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gecprwnsn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gqkubwfil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gqivqkuwy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gfaccipik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gukatnqbm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gonphynqc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gufhnolej.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/ghzkqqggm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gxxsddlel.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gnoptedgu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gufyjlhtn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/guadukcrx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gbjwzqdcw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gqlniydlk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gjxebxhzt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gpkdwdnyw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/glhornnst.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gvyvcjraz.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gnmxglcoa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gmixiatyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/grmwvxjnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gjjpwpxaw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gsqbgoymx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/grkdhobpg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gghdcsikm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gxfrkcomu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvkgzrsto.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gexciurxt.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gcqkofqiq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gtvubvujq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gacjrywsk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/ggxdpbavf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gvteadukq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gvaqxmxwa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/guakunuvu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ghinxtasv.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ghkidnehl.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gnjafbptn.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkcxujuij.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gxoyszkhy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gtpzpeftr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gwmawjexj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gvhlncnlb.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gjzaskiht.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gzdlxpesz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gcnfgoypw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gcelxbiuy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/giicbkxso.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gfkbcolfe.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gcbxsqhbi.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/gsdylaywp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gydstjoaf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/geclwlbmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gwjznxurw.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gkjpxhteo.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gwietxkqd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gxiisdtzo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grfxbxdzr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gojitioua.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guadkedqk.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gddqxpjvu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gjlhdvuno.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gdmcyczay.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gamhkfohr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gggtvfhnw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gnfpwitxb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/goruzbywm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gpiscfdqo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gezzhnhuz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/glsimocwr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmcxopxvv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gfymluyms.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gcshazyaw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gtytbljji.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gicesnvtl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gcbudbirm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gqzuatmxr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/guilblgxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/giwkmvnha.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/ggkwrinlp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gynayasex.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gkptbttte.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gtmyfpnoe.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gmxalakly.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gyhputcnj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gphjdayiv.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gaxkpvjjp.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gdegtagst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/glwlxgdum.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gmitpnhzw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gtdyuvvyk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/geoemypuf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gacouswud.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbszlhjtp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gqzyceqhv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gtandudmi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gnuijrmzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/goioojnxj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbbwjgz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdkluekep.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gdnnkcdkp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzpxkiybf.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/ghnvtfwdg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gnkzhkhjs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gpemwdcfz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gzwbwmace.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gsmwunoyf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gwdyypabl.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gzuldwssl.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdconuave.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/glbbjmcro.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/giywkypbq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gyxmdqzqe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gsuupsqzn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/glzdnptjz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gxvjabzcz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/glzrmnejq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gbcudnwuz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gmxsjfkhu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gkqwerinn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gjnbarqrh.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gllvjdcxf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gzbzsmcxb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gpadtrtyv.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gvhdgppxf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxnshmqgk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gptousmvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gdyhhtamp.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/goyfxqnqp.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gcqfexddw.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gxysgifez.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gefyvqaqz.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvbjytxjo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gndhojfan.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gskycpnoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gdmhsrtjg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gslbdgplb.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gaayhyekm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gbwblenuc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grsanjetj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gqzdnpzka.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gedobgsvo.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/glvzrygsd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gysozhzis.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gtumojlem.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/grrfuegzg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gwkhtdzcd.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gyckbujwi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gwtxrjzms.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gebxebdyd.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gzxwqruit.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gecuxjomc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gxjackori.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gxzdjbmbg.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gqfbjujmw.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/goiytfqpa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpefokenr.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gpcspekow.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyndkowqm.sHtML


<!-- 参考信息 -->