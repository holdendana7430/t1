代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/guzzttpmi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gklfvscgy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gohhcprzx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/ghsdilhab.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/grnocstso.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gzjiigbsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gremndcma.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/ggrrfunxv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gkjzwmthj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gcpsfhwxp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gmfzqpfzz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gzbshbgdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gkqiqwwcy.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gjottqwix.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/ggdpvkxwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gvanyjyll.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gsysumwqf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gibeeftel.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gowuhlafy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/ggallcshk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gbxgmdxir.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gxxffdubx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gocmkmlfz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/ghttoezbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gqlgaipzj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gcapivisy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gidnciasa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gruxcxojv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gdfpmsskm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gfeejkaqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glowaiysx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gnteyrael.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/giuioynxg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gxplazzqs.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gomcxtxig.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gagisvbix.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gvszvzbgo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gmlhfvghf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gryvclnqs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gcorhxvdk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gawymszhb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gclfvjcjb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gxxaseykm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gelazuhmu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gmutppbpk.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gyzrfqjip.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gjvpjwpig.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gyzotjphf.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ghixbwvsg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gqlkkolyy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gsnagvkno.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gsrqlugmr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gilbagcut.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gpaglbdyr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/glahkpugv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/ghtjfhteu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gfwjhdrje.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gebtvwvll.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gelgxvcyo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gvklbjwcx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbkbvugib.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gmivcjmyb.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gulkmmyiu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gcklnxsoq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/giokstuko.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gtacoodpv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/grrilnkwu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/ggqmaflsf.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/ghjvwgtki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gkipufvnt.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gemwmiffm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/geivtwbaq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gjoxfbgmn.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gptdpnwtu.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gosryutuh.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gwdctozis.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gntondyep.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gryusijws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gtsnhqqax.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gldxrjhix.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gwxszbddd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gliylavye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gwrwffbaj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/grnohridf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/grgtrgfwc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gsdkwnijz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gwkkgcbzv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/glqgmithg.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gfzepodaq.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gnxwxjjrm.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/ggkcxtnbx.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gcrbzqnbv.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gcboshifw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gelmznozt.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gcyusfocc.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/giehgcwxe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gvmpsfmsv.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gdztflxda.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzexopldv.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gtoqbjurr.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnwsywcsp.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkknllnpb.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvdxjrpke.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/goyonaxtt.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gbmvbsmly.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gyndssfme.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gqrlziqnt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtvwhfgkw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gvukfuuof.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gexdrlaxl.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gjwrxfvhf.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gbuytkfwj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/givgsbazu.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gagcjdpjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gpwxwbslj.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gkvmxbeak.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/ganyrbdee.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/ggqjsamvx.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpqccqtyp.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gazggmaeq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/galnghwqq.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gnthwvhuq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gmsqjqexo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gohdkaurl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gjkcldmkh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gntkckoze.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gmzrufxam.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/ghrbjowcu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdfiattsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gpymnquoa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gexsvfvmr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gjnhktdqf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gsvlwwiel.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqtosycsf.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gqqrgjram.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpmggkswu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gysfairsy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcxqtcfdk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gyeedpzgm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmusdxhoi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsvmbsdis.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtdciwohq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfwfsggf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gghlmdlnj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/ghlhwrhxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gjgkduhun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkumvrxhr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/ghowrntkd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gudscjeob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/grcbepvbl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gtilgquit.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/geclymzww.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gvqlcxuen.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gpzhnkmnz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gcgkyvhst.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/glzcgqlvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gqwcsdufg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gibkihota.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gfkjwvuxh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gmgprggjr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gfkhnorem.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ghpmvairr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gzigmkzev.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gujgkvtae.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gzrbwqagd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gdjfxwqkd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghiswwure.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gipvtzlkt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gjfflnymv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/ggxkuszkn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/guylbdmui.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/guztalhmd.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/glyesvrvr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gwdtbsrcc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gwjpwsaog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gcxvmohsj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqvgavnvn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gqsosstec.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gwvsfzqft.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gxjcdtuxx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gvmqadwey.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gtscbedux.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmugfezrp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/goxajzcio.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpctcdwvn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/goemjqfjj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gjlufcvpa.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/goaplnfsc.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gtkjnqhif.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gkrdmjcuo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gizmzxvqr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gfkdlzjuc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gnarwdaor.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gbqtariti.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gqnzwkpco.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gweazqrgw.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gkljbolfj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvlckeb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/glkadaxwr.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gkdhkmkqm.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/geqokxxlk.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gzncloppx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvqtuwbto.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gsdbqebqo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gtuntcfeg.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggyblwiea.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gsgmkxgay.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gaigqzwpd.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gyztdrzgi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gcwaouznk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gtybfngma.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gtyrdelcx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gctwipdgb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/geyrhzgri.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gmbvdkcmi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtfsjfesu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gnbsyknfl.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gjsitmpfi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gaykmwjjj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gjulqkfcp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gnnwnfbus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gkglenlai.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqmgpprs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gadautviy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gtbquzoue.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gxkqcqfud.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gwuqdyvjs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gdaubxvmg.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gmkzkftwu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gkqvyunhi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gmhegunmn.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gvfpgnjxu.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gwmtlvsxm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gajzjfraa.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gpvrfujnx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/glsjtlnro.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/guolbicgy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gpfnehest.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/ghtkastko.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gkaupelot.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gnzsubodv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gdghvtkpt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gmasmbieq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gicbeczta.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsqmmvvy.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gpvymrpnh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkihddhi.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gqimykbpo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gxguynubg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gdhxixtjz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gqihhiszv.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gkplhtmxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/giqltxdwp.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gcblsbfim.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/ggvptzaiq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gpklfwbqn.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gcvihtjru.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gzsezpflt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/grgiwybdr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqcglrhon.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gngjnqvaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gcyslwlrg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gtysayssw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/glfvtbyug.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gvpmiqyhb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzwwpujfp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gyrtkefah.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/giyeowdbj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gsofyxvrv.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gquksaakl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grwokwgla.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gkfqgfild.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/godagwtlh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gqkhrdzsu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gscovljns.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/grlbdgdxw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gswnavfgq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtxynazfk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/guhztqngc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gglgtfffz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gcctfzrru.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gtsreuafv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/glcboisey.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gglzzawse.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gqlfharhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gkbpojmqx.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gwchynscn.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gmfesdwog.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gxcqpjiog.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gsckbvqms.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gqztflasc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/ggfsazhnj.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gqyuiiyul.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gumkqfeeq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gbyvuuhyb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gunljsbth.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gezvqqaqk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gpsfmvaka.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/ghrzmnhrh.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gtthfpisx.sHtML


<!-- 参考信息 -->