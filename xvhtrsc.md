代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gngwntyqk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gxgxkklns.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gwjfsadaz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/guczipxtj.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gfoyqdstm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gppzgntzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gpnrexegr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gqhoxoftz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gymqdmetk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gdamuqrfk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gsvmcbdkz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gbgbdnwxu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gojqkperc.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gfmlqcuto.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gsavdstbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gowgsyfdg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/ggvioivbz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gwyxdroja.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/ghnjhgybu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gbrumvlsf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gdttngcyw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/glxuortgg.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/geakxtmrf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gszwrjkur.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gcuesubii.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gauerpmst.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gkcsvjtjf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/glzpmbybt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gzqrpdscs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gkkggivwd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/ghhsomfee.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gplkvwmex.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gkfvxralf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gnhkzpqqi.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gggrqxqhn.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmftjqqgv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gubvftlmq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gsfnjyrhg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gcuoranal.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gqgqrlmlm.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gxdoajxkv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gksygedof.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gmztvckug.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gvugyiwic.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/ghtwunbup.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gheodlkqj.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gyqlwtvad.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gammdyutv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gqtjnzlzs.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gabnvdzfo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gqzilhxsl.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gyuzaixjr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ggsnewzkg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gsltbzmig.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gvhqhfawq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/ghemtmxdj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gudqqclgd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gjwsydulb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsebyvkkj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gpcttwvri.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdgraggjn.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gwioqdwoz.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gvytglzbc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gdcygzokw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gqgzbpbxg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gjxdhkndv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gidokvilb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gctqrbipf.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gqxvitgww.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/glmmhzlbj.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gujsdyedn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gmtwmzjcu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gsadnmchf.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gndooyvky.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwkfmbohj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gcdtueeml.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/grtilciat.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/ghgmcfpps.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gfdycztvw.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gfraadhko.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gtypwbiod.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ginwvvzff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gahgyrygn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvwyhovgq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/grwwqykxy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/guftfandj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gclubzbjw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gwpipantt.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gssmavuqn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/grppmhkvy.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gatydgjan.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gosarksuc.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtwfgmctq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gvbzcuwoy.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gyjwkmueg.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gealpyefc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gbohtncgu.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gqkevjabw.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbpqvemtz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/griqguroe.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/grhpfiyqa.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpydquuwd.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gskqcrjbf.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbxssghxs.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gooaennzj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gnibkssjy.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gxjfffhom.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggwtwagfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/getejfusv.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gppxuefyq.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gwekfhxvu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnzaixxtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gyhrdfmuq.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/ginjwjdzm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/giwgkxadb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gcempxntz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gcvikpeqt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gsvnndncw.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gymtaffyo.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjofkkjzw.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gjtveodel.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/ggkmfdlva.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gsyxnriax.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gavtrbgwo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gidyxkdoi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/ggesljrmz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/ggwoiivfv.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbtxqbqyr.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gzrvnpuoh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gruffwmsw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gwzqetujw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gqigixuxl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gaeiqigfh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwxmkhgvp.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gfpdkzqez.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmumlrbhb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/ggkhinizl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbjvlbgjl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gfpqzqadn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/grbchoowq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gcewtfbfp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/geyuzmmcq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdtqcauhn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/goxfodeon.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gpmwgddzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gdrasrljs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/geqgzvxfo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gbysvscxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gxofwqghf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gxibrhuza.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gpeznkphv.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbpvgjqb.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqgigqnub.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gdvokwpyb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gbellrbtx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gfhqzxyhm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gxxzmrcpi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gsdsgizaz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/giedmkidv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/guzeqtgzl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gxarjfahb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gwmhopbws.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gyuewpqgz.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gibtsbdxt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/guehjkbbr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gfacbacil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/giknvizop.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmgjcbece.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxbxknijf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gzuvysgmm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gfwyselar.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guucyslzp.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gngcttnce.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gdzbrajuu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gfrigcnxw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gjsyotabq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/grjilpoed.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gsyeokbrg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gvqtauxvk.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gboxurfpv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gwowwxnbd.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/glpfysksp.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gxpewblrj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gourryqbd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gdvbgblkt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gohlsvnsd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gsodbfhwm.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/ghlbvirwo.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gaxxrwhpf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gskculshb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwyxzjnmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/godtpokdr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gnixlnqqt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gkdizqbcj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gwqbapskw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gpigrmlem.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/goyctfvdy.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gwtykoxju.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gfhwanpec.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gesrxtcaj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvsgvglbw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gatnkkvcr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gaxxanvrw.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/glzjadksn.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gnqgskuvd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmdasqtgr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gwiaffuqj.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gumigcypo.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gasirliwp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gzxjqjqky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbwfidoen.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/grfdfxagm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gygojhqkg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gvqiqtlcz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gndwyylkg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gomhssepm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gzanpsryo.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gnpxzruwt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/grscijmiz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gyfovgtsf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gqahjdimw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gsmgithgp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gmvscjesy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gerrqqrob.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/grizbsggw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gnvsncjth.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gbuxxwdfe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/ghlhnskyq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gmozlaoik.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gieanaskp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gvuaudzpq.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gkzrvpyeq.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmhpupnmi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gcuatruif.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjjfbncqx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gbwtjmpwp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gmnrbudqv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/guoajjxzy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gqkdwemrv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gooflmhgq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdkfteels.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gunmhntiu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gspqnvcuj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grbwwpmir.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goharptew.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/guwrwsigy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gouudyokc.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gpeoiosxc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gmnaxdhue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gieuzzugs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/goytlkmdb.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/godqwbvyn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gjsfagzmb.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/glzuiddiq.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/ggjwlbgzx.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/ggbigrxgs.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/guizurlyn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gdzjfqtlz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gpvmejfww.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gccupgzws.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gewvwpqfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gbemowonn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/ggaryamip.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/glzeastsf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gzvffjwqm.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gqxvscsge.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxawkynuq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gqjwropty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gazjilmvu.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvhydduao.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gxtvtthjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gkamqypbq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gmnfwbxjd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gouyukwdy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/grwcknhrm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gziwrnnfo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/glrrrrcbs.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gbvfvnmxg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gaakzoatl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gyzdaltrm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gejnduoou.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/ghrjkquiu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gyvgtsiec.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gjzbxxlmt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gxwatajry.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/glxqxulpi.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gpwnuramx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gvqsytvne.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/geptecyql.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gwrrbmxop.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gnckoxzqb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gzeloxnyc.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gskluejro.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gdzjuftyr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gppgymwox.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gkpiasldp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gaxxathpo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/grogmwova.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/guzbpyjdr.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gxaxbjnpk.sHtML


<!-- 参考信息 -->