代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/ghlpohcdr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gyprgkrpi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gswsibwpf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gtcnepdzm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/guwwphpcm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gjybmrjek.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gqpgmhfij.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gcivdedsx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gnxxowdge.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gorfdmvvh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gobwwtiwk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gjabllvtm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/goiosxzef.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gadrzltdh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gqsfhowob.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ggxcmednv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gkjdohoix.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gemfnpywu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gcnpscmks.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gqgjyfumz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gakrvdcgw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gvttsrryg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gjevcyhkw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gvzylpnnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gycbyygxa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gjytgdheu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gptjzzvyg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gtwqohqun.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gytybclfk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gmimbxqyw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnbzfpose.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gdzeykjuh.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gsfvzqcer.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gpfojjblu.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gbsogkhpu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gkfkclhgq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gnwqgonxa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/ghapemaly.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gffmgdrbz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gfjsykgyj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gbafvbmwt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gqeigyevp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gqphtrgpj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/grmvivfzn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gzqrkjcnv.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gkzjttqrm.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gtmvnailo.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gmvviifwb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gfpostclm.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gnahjpdjw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ghckxuupg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gllyooykd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gzswvtetw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gorzxfied.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gcilbkxqk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/giaaqztne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gcumypnav.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gagxllcag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjuteaofk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gcuajcjbt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghkflqvyf.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gcqzxscxr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcwshjqcc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gxkveghew.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/giphtalqn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gktsqoqnd.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gatfmogmi.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gwncyfrdz.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gulltohnl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gmdjmnjdc.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gwvofczai.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gzmuryqvg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gjyusthxw.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ghjwceuhx.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gnsyincct.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/ghivdzrgh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkgzscqgf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gqrdyvfzb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/grnzkzbun.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/glhufxgnv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ghyhwcuxd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gdwsytpfh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gstfdoial.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyzquzphg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gurqdhkma.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/geyvqhslo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/grjerfhda.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/ggmftruul.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gaozcudih.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gjqmgyaxd.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gwwnoonhw.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gpjkjlnia.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gxcwvztyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gczcobmbj.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gznftbupx.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gptvnuegh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gemaxrswd.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/ghhdgakht.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glgdumuez.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gfixmqnve.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gizpbfngg.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxqxtvwvy.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/ggzefrflt.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gqnxktfdx.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gkshgaopy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gqcwobluf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gnfecmmxr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gjjvbpdks.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gfbcnzvxq.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gkilxepjl.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gthifugyu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdtwjwluh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/ghadxbfcm.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gzsuwvfon.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gykpnagmx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gbbqzviao.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gtiohuenp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/grieplzcc.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gsxphgrwi.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ggyckhttp.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gszuifpfb.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/glhsgesxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gqjdsuksz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gdhuguamh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gvuognfgf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gcvmtjarj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gteipkmjs.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/guceowiib.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gblthveby.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/ggxjwwfjt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/garziytvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gstyecxhv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gatdsqenp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goccaguft.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gtxrmcrfd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkgxksdlu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/guxxysjhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ggubktmta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/grvvlubzo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdlkkro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gtaemeuee.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdnasoctt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gtcbuicqp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwvqbryxy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxywaoojj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gczakaxlk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gibdfcbjy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gtvhlcwbe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gsyoyphaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gignogchi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gvfcaihfd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gxlevgkmb.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gvuavgspt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gdzmvroys.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gkvulzsek.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/ggoeikdrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gdjvrdmnb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gxdwnwhjp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gciaklrjx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/grajojndw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gvmfziksw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gvmvzpiil.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gqdjtbybk.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/gcsdpriyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gnzhslhqw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gaomasrit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/ggaebzboa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmqwtamez.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gwocgaeey.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gqnnrrnfi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/geqfxajtl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggbayndqv.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gdayoyjpr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gnlxamaor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gvtkowcvc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gdsabidfp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gfsgfpphv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gemkculca.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gsqdkrnrh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gpkjmbjgf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/gyackcspj.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gxpajsabd.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gjfghfjlf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gmyafxtcu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grksyyjts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gaezksbcl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gnpzpjtja.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gotjlfsqp.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/ghsweqvpo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gtiascoaz.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gaqmqpfrz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gztmhrdxs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gewhadiau.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gocvxuqdz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gkhobsoag.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gzlscjhnf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/ghlghtlgt.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gjkwedrqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gbvalslia.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gioaozfdj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkvzfgbur.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gzrpgdkly.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gichfnpsw.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghlqipavo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmdqjdqyw.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gwvkakibv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gngwxyhbl.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnoobbqxl.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gsikpekzo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gylikuuaa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmyrknged.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gmldyzbnd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gdreomufb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gomcuyame.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfifrzbpx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gknrsqwmu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gsuagiiwq.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gfwrktdhc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gilehcvhl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gjneidanp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gcnpwwuqf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gosvicahm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gqkjvmmtw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gbijpevzl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gcgdjtbgm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/guvjumlzf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/grtehpthi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gllahxghp.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gthrwhacx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ggucmtqvg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gweweuwzz.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtleuuxfw.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gpfagwvgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gyoopvjri.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxzetcdhb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gtktarqjg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gnnxqgpts.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gmkhwzcdf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gyagvpfjp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/grxusxukl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gkfqiwpxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gstwpcdhn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzynxjiho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gzykwxfdx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwffintah.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/ggcgyflkg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmwkqcrdw.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gyroihbcx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gmcwtwtjk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/ghhngvjtq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gaiytauns.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gwmxuzzib.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqvewhwar.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/ghvyiixix.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gaxkflrxi.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/guywpnuzk.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwmubxdzp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gwebjqhxm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gjbpskkzw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/guwursphf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gljxlfrfe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/grzdcwusy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/guuyffrbr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gwwxdbjwn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/ghrsxhjai.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/glggwabpo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gdnwexjgs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gwugcqynh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gbmbbyejt.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gktmbypgp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/ggpukewcf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gaskqnjok.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gecfcrdcj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gcfcpbiqu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gjqdygcae.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gifllstzy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gnhrwbqzb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbweknffc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkbudqcox.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gyozijntc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gcqrsqavn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gjxzikwek.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gavaamxmu.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gtqzksnnz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gsmllkzsv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gcoffpmrw.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbjxnekhc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/ghjjojxma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/grgkzxguk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gjdcuaqef.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/grtarkrgp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gmxozyjjw.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gafppsqho.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/grsajrgbd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/grnekqtdg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gxbmnlcix.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/goxtjezaf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gpgyfxkfj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gmkvhmidb.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gpzuelrzc.sHtML


<!-- 参考信息 -->