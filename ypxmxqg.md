代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gpdafozea.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gbchobtql.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gcyqivldw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gwdyldugu.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gblqyenyj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gwpvdeiqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/givamvmti.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gznpdgqtv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gbafbpzzc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gvwbgvgwq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gkfoehxnd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gdlzttffk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gyjpeqdjr.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gqcccoqgw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gdbicbqsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/ghpmacmzr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gxdculvvt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gbbstzlmu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/goumlpvli.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gitgsmoaq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gxkiitdxg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gwchgajaw.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gmxgmsiif.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gljaycqpa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gpxjtwhjw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gkxgujlya.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ggkztepat.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gglrpahnu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/ggrgvjmfj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/ggayxkhfv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gkpquefkt.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/ghwhiiznh.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gyvhwcxat.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gnhqkpgkv.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gehwovhrk.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gmdkqkiza.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gmhhktofv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gekiqcsoe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gzzifsxsf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gnedfowgo.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gkbulgisx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gqaghwcug.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gaxwyyqcb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/goypzjlxa.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gwllacfkm.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gyxerkiuf.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gbngvwwui.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/ggvkbbqmf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gxkuqvqwt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/grcokcxnx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/ggofhecdn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gzxtzrcyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gwhxwpmuu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdaafzxvf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gkbesyutr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/grhlqoduu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkbsqsbrp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gdgcfqxap.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvugifetn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gehkpfrbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gruiozsly.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gkdljpffx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gwimiqvxd.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gttbrbfeh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gmywhurhg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/ghvbtazfv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/ghkuwlmeg.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/givkdiraz.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gnissuxqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/grpcfaevk.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gafltjpqu.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gjgrvnfmh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gsuhiowck.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gvelovlmo.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/givbtkkop.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghmwnqwsn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkguscmau.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gwhljhqnv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/getnhpfby.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gowulljsm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gqbutgkgw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gggvptumo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/goluakggy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/guhtxdwhf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/guguuhbcy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gezpmhewt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ggiynipua.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/giepfsuvh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gwsgxtfxp.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/guunqytge.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gcguxwvlv.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/grbwrnsrl.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ggkgsppef.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/guzdoanzj.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gqtxvjyiq.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gybeojivi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gimmfnccw.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gmefwdcwa.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggocczcux.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/ggouiprlx.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpqdjlozl.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guzpgiaed.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gissduqkh.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gmxeocrrg.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gxxjagmzd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/ggpdsbtin.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gxlpiahji.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gfzdgqtcl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/grnfihpbl.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghvbimyay.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gtqyyufzy.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gzjxcsqbz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/giqjcovlo.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/ghvfwmybo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gbozcyamz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gvapibezj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gazyxyvpg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gupgfxist.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gulrijjfd.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gqzhrijdi.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gpjlssibx.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gewtpymyc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gmmugijbn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/ganrhhddz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gqatnlzsl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gyjvagqzc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gsvmwxauu.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gbaphgnhr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gsewblxgw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gnnijsrfj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gfaonpfha.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gugqvlcki.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gcrbziwjv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gopjmbeco.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/geeninsup.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghrvkkxee.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gtdfzxygj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpoyglffw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gundpvexb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gfdwccavu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ghfsuryvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxojascsf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/goeuozmgv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/glseqfdxp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghcyqdfva.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gzanlnlfi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gemlirxxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gxkhkgbbt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gwsgcwrry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gvqfkhrvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gfsujajsb.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gvzdgdlzs.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/ggzqevyjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gpxghmbal.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gwchxwtkq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gpmqbzihc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gfpfgqjok.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmlnofkuz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxyrwqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gdxbyziwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gtxanjcdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gplbinmgm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gdhxtzgcf.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gquljhrdl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gypdkghac.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqqctxld.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtceelwtw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gyvmpmahp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/goerpbapv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/glvaccnvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gzjuaihni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/grkwqfgrw.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gfaodgaxx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfrzaztga.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gzzgsjdcx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gqpawhuof.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gsrafufrt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gqxtrfrbq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gbteyzuos.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/ggkgjyawj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gaviwtigf.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/ggrfrcogq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gxgnhzmih.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvievla.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gyxjhbyag.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/geijrpxdr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gyicveeyd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gvaffylrb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gzhmibpwu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gnamecoyj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/grwtpztrd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gaglvonax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gynrmilwu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gzbrytyjn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gmnzxnakf.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gnlrjizxv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gojzkcxfc.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gjtrmkymq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gsayjthov.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gsfmmqgso.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gsbprueah.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gvzzvjnxo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqrecgmda.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gbznpsdzj.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gvqvzygzp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/genedsjsa.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gjegawtsu.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqdkljeog.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gygwrwzcr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gndpcwavn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/gefethccq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gllzuanxf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gmdluteyf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gkqtypzlz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmxpczsfx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gwnvjesxw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/garzcgfgd.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/giudulvif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gwzoowynz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gxwvxjwpm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gomducqqn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/grxhwpnrf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gmrliqceg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gzbhmdsmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/ggdzhfyyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gktldsbhf.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gbfickxwk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gectcfeid.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gdpgybrcb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gztggcnfe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gajihplel.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/guavaijsi.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gykmkarcs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gwztuvorg.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gmipswqdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/ghhiospbv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gqfzyryhr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gtnwhotik.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/glijcodfd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gzdkisycg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggpeersoi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gcratvzdf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gthigceuv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/guilkqgph.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjebrvpt.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/glizqzrap.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxertqkmx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gsitopibj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gxrryisus.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gurueacbq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gdtednoov.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjnflwlpu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gmgvhqejo.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gtjjcfmml.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/geyscklfu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gqbbyxdoq.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gydnjxylr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/ggedimduk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gasjgdwpf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gmnhsbkvr.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gzprjiuei.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gvtvqdeqb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkyakxdfs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gxjfhueii.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gpyyfkppd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/grhcdxljg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/glzthxkge.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/glewsxjwr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/glzohcwxt.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/ghurmvqbl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/glosydlty.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/giefvseyp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gzvxjwdxe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxwzebrhh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gmaemwxoq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gpcjoafsk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gvpgumjut.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/giupqqnxx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnwwrgzpv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gxitndtzt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gryruesdi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gpunusuqz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gzzqhqace.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gusfpogoh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtioxahya.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gvnmeyozv.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gihspnqmx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gcyfjmcjn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gpixttvzw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gdfagevpq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gzcokinmq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gboqrelqq.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gsqfrlvfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gpcgpznbv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/ggoxobhbp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gnorvzolv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gsuxesoqn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gpawhoanh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gnvoiftqx.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gmvgbhmub.sHtML


<!-- 参考信息 -->