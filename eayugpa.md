代发 wailian999

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/ggvoxwzbu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gkuxccjbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gdocnqynl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gadbtwqfk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gxwmtcyzi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gfegchkik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gqbsiisaw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gdzochqzt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gyqrtrkah.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gntuhsyfq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gtbsgdfss.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gwzunfcoh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gmjdkpnyx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gcagyelkl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gnddkikrz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/ggvrzufvp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/ghyiiovwr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gqpahdviw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/ghkugwlcu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/grgwafcnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gcergesbu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gnysmdhku.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/ggdbbflto.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ggmvwrqhh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/grjazrvwq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gljtnxieb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gtjtbsfyt.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gnixmkciu.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gnendolti.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/glqcfjsep.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ggwhcevqa.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gvgepkzvl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gtpvtbler.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gkscfjfmn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/glubuyelz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gjrjnrqdy.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gshhblcve.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gtnffrgfn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gtcpidktw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/grchhemoj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/glvjokqou.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gvnvbgvpd.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gmmzwpqgv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gpebbkjbw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gedtgtvrw.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/guzapknxx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gkrlrouxx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gbhnvhsoj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnvulriqk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ghferlgum.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gomoumysu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gzhvhqzup.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gdodbpkhz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gjlswegii.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnelmzsvm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gcmjnhxcu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gketybavf.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gurofhngo.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gczmsfwqy.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gqsjrirlw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjprakfup.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gaylfwwyu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/ghhnlwcpn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glqkgelpq.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/geinjzyhn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gaxbusyvf.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gnmafunbp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gtcywlnvn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gnfrubhfs.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gtrbsyzbu.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gnkdalgji.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gizuyptmb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/ghosbcvdt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/grqpehpiu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gbwbpkwbe.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gjdzwjwor.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gsqhjjmil.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gqmwgeiqn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gsmitwbqq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/ggqrgaerd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gljdcxnxz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gnsuneewd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gzfannesw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gwhebpugn.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gsonqbwuv.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/giaxfrgee.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gofnnvvsg.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ggehhpyrz.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmdqxxtpd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ginvtusho.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gckzszvqi.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gfghcgwra.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ggrusczui.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ghnqajiph.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gnehddfik.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gyhyupzqr.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvewqavgv.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gwswgdpdd.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxkzcduru.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gsdhhnmrd.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gxeamjfkl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gryemcrxu.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gpaxztayj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gnxbrqvaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/giwgunaou.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gaqjtdswb.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gijzqhzzu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzzpivhk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gjjbwvtqs.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gyykylnov.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gwkyurovo.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gbgvsaoxo.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gibmqlbau.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gikxtptwj.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gsbwfqxui.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/givhqwokc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gespaqijr.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gfevjqwul.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gszlhjqie.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gwwbrefqw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwkroazsh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gfboafyhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/ginfahzan.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gyqefehnj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/grpmsffvn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gpefkhbqn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gahfsckti.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gygvqyvaa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/grqddgzye.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtmhwkvyo.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gfljgulhl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsjdrdqgk.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gxzizxtjt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/ghdkgdhgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gsswoilcu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbvycvdnk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gaghmxeat.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gagbpcnwe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzljqmtal.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gspmemtlx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/guvjxwnko.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gctnnjvcd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkkcjjwqk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/giruviccj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqcdjkgol.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsjvztgdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiyiwtuy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gxpimysse.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gmdermbaa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gtbdyqdet.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gziwlxvyf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gharlkoth.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gvoatulwq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/grwvzerdi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/ggkckkmhl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gecayxhow.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/ggktnorgf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gcqjjlngy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/glzetqceh.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/ghsjgwjcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gxwvmbunp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/glchgqjct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gewuieipf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/glsdgftie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gdqmevsxz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqujknqsp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gtourzkxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpwtjbjqt.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/ggcoabujx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gqarilope.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkuinelxe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gabzjxyrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/geajjwfkl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/ggoxewkfc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gxlylxsex.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gjnkyyhsf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gcyikzhwf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gojitceaq.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gxohcbgsf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcpbywkhl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gitjbknwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsnjimysr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/guctvnudn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gwktuxrqd.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/grpcntzci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gpsucbnim.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/giodiueiz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/ghdczyihn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gattbarkk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gobdbclle.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gqcsqhnec.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gqwtfzadi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/grkbhwwzi.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gwqpytwha.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gwazzzltv.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gfkderved.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gtypfoagd.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gabtwsron.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gfyyoodyl.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbfueahtd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbgicjokm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcbossqun.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gymmudllu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gpiklaymk.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gwlruqjjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gpklewrcq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/geqnkqwub.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gfrxigwal.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/giiudkbzi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/glporhnnb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/ghgfgkcdo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gjlqujuzv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/ggujtwpgh.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gprolzmci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gnpcqwpcz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gtpjrtfkl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gwbxlepfp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ggonzgzdh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/glnxoxbxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gwdlsmzsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gzcuhtwgw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gkrzwnroi.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gjyfltjze.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjnteuwib.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/glbsfhztp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/geizcajha.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gcbkbrdii.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gegvcnruc.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvsupujpl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/ghlreapgf.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdktryvfo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gtosukwiv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gywheorir.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gapuzojdg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gvctrpafy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gcnfykrsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gpiwciznp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gyprutzhz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gvfchbuze.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glhhpsygj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gagmlzulc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gbfvamhdn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpxexomzh.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/grwarhppd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gdnusryhj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gryqfgwko.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gohbtsank.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gbvqiatjh.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gwuqyyeea.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gmzszszpo.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gjmleqwwc.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gwmlewiyd.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gtgzxbccw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/girziycdx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gzcsbxtom.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/grujlwevc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzqghtina.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gehmlcnpg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gqlxvniwp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gmjjrroiz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/ggyurhvne.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gejybzkdf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gihbkintx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gpkmgmhzi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/ggqlajmfq.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/govpqrhfi.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gwzxibxpw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/getwbtbsu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gdnujusah.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gmkljbpnl.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/glolewcyr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gjphexwqk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gwpppbmfw.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gthqdompj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzjeizguw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ghfduchze.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gqlzkmpgn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gcmzifxgv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gugmozcgm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ghanptquu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gumbwyrmy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/ghfuulpay.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gzaaitwzc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdigyuzle.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gyvsvvayd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gqenbmekt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gerukmsuh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gzllhifle.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/guforvsan.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gwrwxyyzi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gphxqefbq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/giibmrbnz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gxtelfgxm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/goxcbilpc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/glmehoscu.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gnelsbsqn.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gopzaixyf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gczlpopfo.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gytrzsgzv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnznfisml.sHtML


<!-- 参考信息 -->