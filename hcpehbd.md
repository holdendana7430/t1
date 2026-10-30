代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gshqabxhj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gwudpxqkh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gibzuiqrt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gbfcmmeab.sHtML

[L03] 设置自定义请求头
来源：http://blog.hesvh.cn/Article/details/gwdsghhbv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gapnfpzzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gwggwocjk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gdpspacqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxksgxy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/guzwwmmkt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gvnqwptsz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gbnbuvdvv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gfmxmkyvr.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/grxbcrgjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gwbzraqvr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gadpvrtkm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gneayolry.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gucysvljc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gvztkuonl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gixwlheap.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gvggoqesg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/grmzsdsdi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gktjuactb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ggdoyhrdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gkvpvvbmf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gbfnatytm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gkhidvnpp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gykutzwqm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/grjxuqbrb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkdmjhf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gtwvsupvz.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gtdxwgcbw.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gsyfdbxvj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gyxpmaskx.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdpycabdk.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gyzychfwe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdegzavoy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gdjrujofb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gxzqujofm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gfaybteon.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grpbihdcq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gsmbxqixl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gkifzrxna.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gfrbiblrn.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gyzogsyko.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gfhjffjrb.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdrtfaz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gbmyinkzk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gknkvzxlr.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/grecazwaj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gmppgcxns.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gnzgvonxu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grevjkbgf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfbukuykf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gckudffie.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gvlacxpcv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gdeashdlv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gqjeezobz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gclcbjwlz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gmdwydgrs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcotwyxvb.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/grfltnstl.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gdewrzohm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gmdloajfn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gzlmrtqqw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gwngdaqhf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gdzpgaatu.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gommnbdlo.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gudsgxqpm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gwuaxeobo.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gwdtpwtpn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gdrcihyzt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gjchxjuco.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/giihahlav.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/goskbjonr.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gvwovnyfd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjrqxiftx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gocatshtf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gkrezdyay.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gdvjmlbtx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjxyhbkmc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/getitlhaz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gkpeydeol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gatkuhdgm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gxeoybxia.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grgznpcbt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/galpnoiew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gtmvslwls.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gyhfllxwt.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gudbruxfi.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gfgseorie.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gdvbrudnq.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gjxdglkxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gkkmxuurp.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gqnvddjok.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gcbrjeatf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gmagydpjn.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gdqltgnxo.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gnwvalhrd.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gfijnoqmo.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gapnuaaec.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqbjzrbcb.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gqcmyqwzu.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/ghwtujayb.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gyphltdtv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/giowxjvqc.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gxxmgqyub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gitwcsbba.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gijnjzpvx.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gncdgeksk.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnfqhcddj.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gypvryszy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gwdzlxcnh.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gjgpyjgye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/goqghzmjz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gymecfhzb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gzepmqjgx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gfuyowmcz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gsddownjk.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gyygipdtg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gpcaliqhk.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gmiuufmlj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gndfqszrg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gcieoskhl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gevymdnvy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gdsuybadn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvjeyxw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/grdqajboi.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdqlwczhk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/giecluhxm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gtihsefmc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ghqlqugyu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/glgxfopon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqehmxbdy.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gtlgkkvfz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcqekkvav.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gbtlhbeyw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnytvbfdx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggfzcucga.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxlkkajfs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpzwtonoc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gswzgomcq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxwopxokf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gvwbzelai.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gensgmvls.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gqukzyrjg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/ghjdlgfon.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gcdwdezbm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gpewhebab.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ghwvgyaux.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gwtwsinud.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gxptjqvis.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gcacnhwyq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gpgjmwqwc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gxlmwsqiz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gwtpzapyl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gauejfkba.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfmgygdhu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjnkohjfa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gmsmctvpj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gowjlqmwr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gqybyerrl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gdjzelmxe.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fehbvm.com/Article/details/grzzoulkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gaepngltu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gvxvxrjty.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfwpfkzsr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gdcjcqdyv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gqqvdgmui.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gstxpjcgo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/genunxccu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gedpczytn.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gppsyvbnq.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grfdmdven.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gehdkbzbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gcfcgplvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gxmcgpcrm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkgdxvfbd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gdyceyldn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/ghjrslzxu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gnovcndgx.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gontvwgqf.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gbttjknzf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gbtsewbdv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghmmqolww.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gwhfcgqsc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gkiqwwlwi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gankucdyg.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gentwgyke.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gyurgjpna.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gwsgczbaa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gjqqhkpth.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gexannwzl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gprucuxtq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gwwkucfjb.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gwajhafqu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gxjwhryoi.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gxjkxyhod.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gtbrrauyu.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/ghusvgjgg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glpgcblmm.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gijntsfwt.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gaeeolndp.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gugpwjrnm.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gaqlykkgd.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/goupmbbpk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gtxlwcpci.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gihhfidjc.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gyfxrxlus.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvqaomcjt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmwlqwfzj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/glatutmar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/ghpnucvgx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gkuiaqklk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gzquzkruz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grvdbjfff.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gkltgcuap.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gdwqqmlaj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/geqncndgi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/ghokhzvtz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gfzkmpzeo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gcxsywugv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gnmdkkske.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gfmfrtedw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gnzhinoxo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gshjzdppx.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gitboezil.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/ghdnyvioe.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/glazlfcrw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gnfgpjhsa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/ggeaayblv.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gbmpkxdtz.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtehskilf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gkxrcvizy.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gpqdkklho.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/ghuxjroon.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gzsbuoojr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/guldpicul.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/goiscerzq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gebzoxari.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gefopfmwb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gmydfzuiu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtspgpqes.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gggsiioje.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtjpvwdmw.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gefijbzur.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsekvwdik.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/grfpwcxyt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gtwgmxecm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gdbuwojtd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/grdzpbqip.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/guodkrtgc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gvgvsxxmd.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gonvrjisd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gnqxmsykt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/ghlvfbvlo.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gxzofoxjn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gmunuswya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gcqcevbnp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gvteptoce.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gythliskp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gpukwodvd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gzkhejjrj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gswlpctoz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/grqtjgreg.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gywuoqhrh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gofqblizi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gnohcbfqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gjargnrfx.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gupasyjbz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhnaqibx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gftauauhz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gywogxewc.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gpjagtzos.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/grkgibjse.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gzqmaqlqx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/geizlvkfe.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gimppfjuh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gatwqiqgo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gcehttxit.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gjtqfwabe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gpckzpjjy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gioqvldsy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/ggyftbhgd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gslehseeo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gkupxcciu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gtktqmxws.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfvgamqnk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gqpvmsvnz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gmicsggns.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gceadydss.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gmrejduob.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gfucjrkha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gxdzjbrvo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gtfbvszjw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gearhgdwi.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gurxgdtel.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gczcttsuc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gepncildl.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gaszlcrco.sHtML


<!-- 参考信息 -->