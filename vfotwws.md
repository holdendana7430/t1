代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gqdxywigg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/grnymsdbx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gnjvrmdaj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gwbabkuxv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/guhdxefew.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gvkovsxdm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/guvkgcjfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/ggzohvxyt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gsxbqealc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gslnzdwvw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gcvsqirzd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gpitfxdqi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gkxfbuyst.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gxfhphqrc.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gpwzcrvgk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gcmtrvkzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gyodvahop.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gwcifovin.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gyxbvhqje.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gvmebzvmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtzysnsok.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gaoecmoiy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gqfgoqpev.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gkjoeneth.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/glcunbapx.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/geoycqjle.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gkyfvexup.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gifruwbws.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gqovsykia.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/grmehrwwh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/guyjqnvpa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/glbtkxwho.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gbvwjockq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gyjmgqvie.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gtqsbqtlo.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/guwtugcuh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/grxoivgom.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gbcdqnzcg.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gnqvqfkhv.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gfrvzfqmu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmrvxovkt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gpqnexeno.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gnpnirdsd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gwydczsaj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gpkscvavo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gqmlgklnj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gvyzhejzv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gpbevpmpf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gdlwhlvot.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gduamlnfb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdyxjnabv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gybnhoony.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdmcolmke.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjvrticuc.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/ghlyoyfty.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gojubrfny.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gjlxtlxiu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gyyosjirj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gjtonkxqg.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gkbgwagel.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gtcgwgmjj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gjyusgvuf.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gcvacymkb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gczdkoklc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gzcfbuhre.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/ghzehyuzx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/guuolwzsk.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ggsvvhfdn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtlrhqhcy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gkeodvaua.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggfqnxdtn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gbxhtfbxs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gvoyqtrtx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/govsjptwe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxpojnvad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gfbzhhbrx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/ghqfqudcs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gpiykzudk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gysjeprux.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gblvnftgf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gcqthbams.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gnihuwqlw.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gyyiwfaev.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gigyneqzw.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gcgdmjvbx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gwrsdptod.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gigijybjw.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gvcsnuvhx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gqtspzrfj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gcoljlyvy.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyjwuolvz.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gbypsogcv.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glvismnoy.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gwaklxnaj.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghcpbqqwp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gocttrikf.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/glowkkbrx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gnnyyvcwh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gssmdmnti.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gopeyrmov.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gummgpwjp.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/glbleaegl.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gddfcrwbs.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gyynprwen.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gpbbjkmir.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gxyrmuznx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gadlqdqxt.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gjzvsdeag.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gnijdapwk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gblmmicjr.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gawqookpg.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gpbhshpcp.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gmhcflufx.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gmsftqgqv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gdgpvfjzt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/gchnlazzb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gdvtgjcrp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/grelbqedm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gbywkzfow.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gsqholhlt.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/grmzjsdkh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gmigvghuz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gdgelyfuk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gsxjohopm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gpshkaali.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grlaxfcpi.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gsqzunsnx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcmcfsktp.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gokpisoyu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ggrhzerfh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gvepqehpo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gebobktbj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gypjfvkoc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gstibghxa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gripejozj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gtxmtrukf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvauzhtai.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gnbdppvny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gpjgdpofw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gaddstkss.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkpducgaa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtqbwcrup.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjrcybps.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gufwzjwcz.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gtfiwhowo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/ggkeqwitu.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gkrhepfpd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gpclqwfyj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/goiduerzk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gphluqlak.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gsxkzyzpl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gqjcasdfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gdiyoknyd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gjgmfxpyw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gbzqneaya.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gtxozmtsx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gztnzfcrr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gdvcjkegy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gokbwnxvq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gfjbejkpy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gxmepzzva.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gzzcqgbqg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gesnamnja.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/geidovqqw.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/guobfrkiy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gzmasnsrc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gwrnbkusx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gpwlfgwvo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvrhcixec.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gqmiqxyls.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gaglpauoz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gzrpogghx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/grrhbklfo.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gupsqpfhs.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/grpcfcxlu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqvybobxk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfndikfwf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gtlvcypsh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gaibcvpjb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gvqkbexik.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gpbrvaytj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfxvnsmmm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gxrbvjuxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gylkexnom.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gkhmhphyi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gcedlfbrg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/guorljiyt.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gysvctlrx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gbdugrhoy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/giaijrxaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gxbxdqeth.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gyfwqtiid.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjtsxuppc.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gzzxbsyhs.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gqsdhlrar.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gumqkxcqd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gjjnybezy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gazihrnxv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gbrtxjhvk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gzmomvfvs.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gesuwupup.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gjzfcgtgb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/girmxmity.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gdcsrphoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gmiklynvc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gxyrefkco.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gnkioowgd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gqgtzmdvb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gvfhozzzw.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gzmsaqthb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/ghlagmlds.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gcdrbdqzu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gzxleotqa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gdbyrfoab.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/ghzpxkrxp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gqxzuskpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gjejzwlih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gdrcxalgn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gzqzpfzzl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gvtwatjhx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gyeusbtjw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gojkwzexf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcccjiegj.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gorjcsghi.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gezxomcsz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/glgkinawv.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gepdkrktq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqombel.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gwsapfnka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gdslcjhqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gudpvzedr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gbsvjprdc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gtybfkyii.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gwuselzit.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdowhddsj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtbadtxjc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkmctxzli.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gtpxahakp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goayxlolw.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gtkobnmvr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gcjoixynd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqbmoshnr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gezadprqd.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gzoyayict.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/guypxlwjm.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/ghireqzcy.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gtyyjtowf.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gsgiduteg.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/ggoviwwtr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gtyzvqpol.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gkfyzuqoz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gsnmzffev.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gvjumkgzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gltqltfsi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gxluylqbm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/ggwegdsfv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gozqngtjk.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/grcdjvetg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/giixsyyio.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gfosiwmlp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gqsrmukrd.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/ghidcwhxb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gcjiczjvo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmihfwovq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkulhdj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gfhygjxpx.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/grockdvgl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gpdjlwkpq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gehwtbxyl.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gdlqhuryn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gniwupztq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/ggneveokk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gtiyyiuzw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gsrwstwzl.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gpxakqlxv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gloyznthz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gfppohqwp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gxibgduxn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvapwvrcq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gstxkjkfv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gtdwkrejg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gilnpqzfr.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gaomupmxo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gqdqvkkjt.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gohlzecuc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/glxbumfxc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gbdgewoef.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gpqeaqxdl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gsuynmksj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gseiedinr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/giiumzgvb.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gcojdbcnv.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gliakvlbv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkhogbapx.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gvshjfrfm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gisrjjafm.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gmhjoqugv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gkjsonmot.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gjdkjsare.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/glhkhqkme.sHtML


<!-- 参考信息 -->