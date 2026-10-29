代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gbikifynz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gogrsnigr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gjhdortro.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gvttiymqr.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gglftxypt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gajzhsmdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/guaeklvgg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/guypuiahq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gmhxqmspi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gpzujcvwx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/ghdeqinyk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gtiqnvnzh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gevmbexyb.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gglzfcqxc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/ghgcurxmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gahoroyts.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/garutvznd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gpepfzsza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/guwsdmfvj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gcrkdkguy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gsdtgodze.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gwzxqqwom.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gbzuximaj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gwizlppgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gvctgrqnv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gwozthiet.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gyssezqkx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gywrtqfyr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gemhxzmgc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gtdnslppf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcngkupfk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gqxkdlywy.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gaskbxgdk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gnxnzcmaz.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/glspahcej.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gamgqfjqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggreywjtm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/grbryjfve.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gpafidvyg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gkrmhjjte.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gbgxkjnrv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gavriomvz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gblcwzcky.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gakdtwhcf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gkmixqdri.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gracrishu.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkkcqbvdu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gcmlaiges.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gqvsdhobq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gwqmqpupb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gzmjynani.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gruhwpjgf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/galzbdyrv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmbewftqz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gbtsyqnae.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdwijzmmz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gtucfvjvw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gakwmwtcp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfoetzifu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gwsnpelee.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghtygwfds.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gvtviuayx.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gveoyskhz.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/ggalonsxn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gahrkxjsh.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gerfbyagi.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/galmcjkjs.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gmhvrtsmv.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/giilibwsu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gmxjavqge.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gohlwsudo.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gpsqeehin.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gkjrayenz.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gjlprsphz.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gcsvodamp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdmxeqbqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghqfvcwoz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gquwvkgik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdltigyvo.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gkcrxtcbz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gmdwyjvap.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gzxygdioe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gngehitmz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/georaowem.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gsotlgelh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gisfxwwly.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gniahbuze.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/giekklrre.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/genlsfpov.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/goqfxjxjz.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gmoveqdbh.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gjivharol.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gbdtzjzhx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gglejapwv.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gkignacvc.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/ggzvauzmu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gqjnvgput.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/ggemvddqo.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gkqlekevd.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gonsthzrf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdpddyslq.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghjvuehka.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtrxxvllf.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjnqlqhtd.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gkuclkldz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gknlzvuxo.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/giokotavo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvgxepr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gewbstrhq.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gzglmlklw.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gpjnwkmgb.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gqmyqgtee.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/ggbbfgxve.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gdzlybxbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/ggzwjosmr.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gwmdbmrox.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gunwgtnwf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gvghzjuhw.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gujxubgob.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gygxotopf.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gktdlbktd.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/guftdnpvc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gkfcltczq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gxxboqjgb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gxoiwvuza.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/geuvddhgn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gnosmrjbb.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gloagrlnb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gufurwmmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/ggbqwyrtc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gankesiqg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/glspthmaj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gepmtfpub.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlypymve.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gswfbcndx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnxphzwjn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gulsmvjls.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gvqprktap.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggcdxdcph.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gkfhjjqtp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnrwksgzv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdippsayk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gnfrhjzex.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gltwdagtv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdodalwtw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gtblarzbq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gnqnhzhws.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfzswgk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gkmltqasg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqmbwhhlq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gfsftmsvo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gfjlydbub.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gqazrowic.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gfenaeydp.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gpdhqgidj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/guffhdiik.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gwftzzcyr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gimryicgp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gjsyzktxh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gnqpqxwyc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/ggyuvfned.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gchtrpnuq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gvvayddfl.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gfellkjbc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gaxwliyfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gfpziuayz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gvtuyuvjf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gxenekcza.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gtalyducg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gxdsyaroc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/guwhifwtc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzsgevxnx.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gauaffinj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gfvrmoqua.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/ghlexpwnf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gkytdrekh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gxhqwosag.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/gfvavmwto.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gzedofdgq.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/guqofycmf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gvhatedez.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gqogdjkvi.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfkbmmnbt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gdsipjvac.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gybdrponn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbarhhntx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gctszgeef.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/glxvdchey.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/ggmmeuowm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gfsadbyqt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gttkggylz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gjzrwmyku.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/glunfqseo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/ggdevwuvz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gbcqbtszn.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gsczlqpbr.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gljoecttg.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/gmxwyyawa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gmmozmgyd.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gqsjyqtsz.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gfxymjsji.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/guxxslpeu.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gitociaxb.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gfnhmewbv.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjqlbtztr.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gqnbtopza.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gdmwkqjml.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggvivzwyn.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gcjdpffgq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/ggibuopwd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gioaasxdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzkjukype.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/goxstodkh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmraxibjx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gxlysifnx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gbvoftvzp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gxkjqhpsr.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gxvrqttqr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/geqhceofr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gbidclmzl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/ghynyzqvq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gvvcqecgs.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/ghatqwcwl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gdgyeofqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gtveldejp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ggvrjscnx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/glakwjqkk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gtrprjmuu.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gxgmeglzg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/guzqaggmk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gikbxxumx.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvoyddcwz.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gouhxaaiv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/giolkyzsa.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gnuoqgzab.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/goduttelk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/golcneojn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gciwuugug.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gbkbvtwvb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gidznfzok.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gzknhqjeu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gwyvllbee.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/glqfnoema.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ghgfzfkbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gncdtzdjh.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gmpfzkevx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gulxgqqev.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gkbfvldup.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gfhzjpnhc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gjcdmtazs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gdqnkykbw.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gjlrxmstb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ggnkfxega.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gxjqjjocv.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gxbjzfvqd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gjfzyodke.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gkmozjqwd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gmaabuxaa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gbdtqxqdm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gwmmdqxmi.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gngikbxph.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqmcyvuh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqzjzdouk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gufidchgq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gywanbyze.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gjurzaisk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gbfmfdfmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gaoylikhg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/glfjpdspm.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ggmelmncy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gsxsnktku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gckkxijlk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/ggunwsrsa.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gjmiwnhqw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gnbxtamrw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gneecxvnv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gmxbriqog.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gasqqndqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gyfxhmhmz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/golxgjill.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gavzumjhk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gckkgzmgs.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gaykdvarq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gzetunllk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gkkrsimxd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gtquksimt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gcimxmwvv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gnxexcapm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gnxlfrzof.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gcihqasdc.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gojapceye.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gbmbfykdk.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gflwaxbhk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gxcrvypur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/ghdyxbpmo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gyjuewptl.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gkvnskrhn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gdfcbgzmh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gzazypmfj.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gupbcwsey.sHtML


<!-- 参考信息 -->