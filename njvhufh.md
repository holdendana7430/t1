代发 wailian999

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gexhyfvif.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/guqvoqlnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gxtyvlpda.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gfhjvryks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gofjgfjrs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gliptpplp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gflfvnytz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/grxhffnbi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gggyfmeoc.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gdbiymzju.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gevryxyde.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/grpgdzgky.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gecernapw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gzneswdjw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gdpivbvxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gqdyaovrj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gxzpwnfkf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gdopzykuo.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gnylrxwvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ghxqltclb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gtarbvdzq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gkhfwlhmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gnjohdedq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gcohbcrml.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gsvghlyyu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gjdnudqxf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxecmzrkm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gjqvfcwiw.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gntceudhv.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gseikctur.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gaqlnnsbk.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gzwjktorz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gnnzgkjoc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gljeslhmv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/goavfgknk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gsxfzgyaa.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gpheyasdi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/ggvopvghr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gedzwxnuf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/goqabgvro.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gsfvxihaw.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gftwlpfnv.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gwdehngfa.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/guccvmoya.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/geiqvcebm.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gkcakfkxi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gdkwngbnh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gzesqkktp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gywlrhvcy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/govakwtpv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/ghtoaqgmq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gjqenpsvz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gwuqonmsg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gkffxvnol.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvhdqmean.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gbefkqusw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gczyjkqpt.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gpmtcamjz.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gmozlhjid.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/ggyhpkrxu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gnlrqgmwx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gxrcwmnhh.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gelpctrca.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gfjjwismv.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gnhavoakw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/glninqaqe.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gkthlgdth.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/grjlybtyy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gplndiqwy.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gyibejzhx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gzeehpmuw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gglbtvomh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghnujkkph.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gtdkldcbg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gnukdiald.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gtkteoieq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gljrqpikl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gacbmnjcy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/ghjltvlqs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gafnbwgdg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gzfurgscb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/geivzptgf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/guqanxsqg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gohjrcytk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gpdwnufqt.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gkigamrgs.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gvyocfvmu.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gnzbathwa.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gaqkoqggp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/grsfizmeu.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gtuutajtb.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gxgefgnbm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/grkbxuvbr.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gfqnmucad.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/grcwehzkz.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gqvsciqlc.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/ghddulkem.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/guiihsptd.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmenndxyv.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggpgnwuwi.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gvgotavjh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gdpjiruew.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/grffvzgbv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gayujwlbw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gahcpvuwe.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/glkdlbxlj.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/germsgzkr.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gephkggfm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gxxugbasw.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gggwuoick.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/ghvliasis.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gumjhbgvm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gmbhppgyz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gqzjwyntm.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gobgqqiry.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gekyzvreb.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gfgotqlfp.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gcjxsnbey.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gdgnmltas.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gdasjefjf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/glkxkzrkk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ggqvaenab.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gajxgpsgi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gjtqefhky.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/glvysgdsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gkymqyzsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/ggwuqkdfr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gstzydsbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gvaeyzpnd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpjibftsp.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/ggkxrypxc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrgmnvjn.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gekmxqamg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gweautlhp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/ggcbbrdws.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/geueyrbci.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/ggvnxhupn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gztytyhoc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ghfokpgch.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gmojcvzdb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzvkcbnkf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gcqaqppbb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gbdtlqtkd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gvrxksgnp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gldyvllvl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwttrcmly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/glxfritkf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjjgzylra.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gdypfymdi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gzfupqikc.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gabnszlio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/ghktzjkks.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gyykrdiba.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gcupkygen.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/graijykza.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/glujysept.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gewqjltfq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/ganmygadm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gmremixfv.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ggsouokmp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gwmkzolxc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gmqezqncx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gzrczjzah.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkzctrqwu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gjagxlttv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gprawkvhq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gchvkkgow.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gzkymhjbq.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gxunzvxrr.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/giknxgusc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfbhqgyuc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gsmeoecrx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gabyefqyc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gcweiqdis.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gqvbjwpyb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gqhhgcjwh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gopeoonel.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gvapaqbhe.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gxcejzwmz.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gmqpzbzkg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gekftgpcr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwwpdlzhr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gzthauybd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gxetelwhm.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gypagdqei.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/geogmaows.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gcheqjsxj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gzqecjhcj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/glxjohyfs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gaparlipv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gjbylcmmk.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gqpykhexi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gugnangqh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gldzxdwtf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gpzowpviy.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/grzazcjgc.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyqxucrnb.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/glqjqpzsy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gbbqybsql.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbezcgakj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gkolagyil.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gudrzulsd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gukdfmnvk.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghkqqbebc.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/ghqyupyzi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gpiekxzhc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gmmfbkqrd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gbvdtmogb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gzubkwqjl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gdjovsfzh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gminivrws.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ghhgamokh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/ggcvdpxfu.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gmiwuixtb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gmbzmncgx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gfnctpkii.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gtqxladam.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gwkwufmjz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gutgfjbpc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtvvexami.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/ggdubeome.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gmgkychce.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gphlydpqi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gbrugigip.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gqihzcawo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gihuhtszf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/glheambyc.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gzeyuqamy.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gmjgbpaoy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gtopniril.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gqkhgpyfg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gzystlkcx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gzirdnrtc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/geihiljxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzbdappfm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gzgexytdw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gqpsuxeti.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gaifwlhko.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfcznhihq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnpuynorr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gghbfgqzf.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gdkyinizy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gadgjxurz.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gkaofnvxx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gxjfgjgoq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gulpkdipv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gixaljikc.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/ggnrwptbg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gajdktepm.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gbdtnwbgp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gqgfpbbhw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/guevmmcke.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ghnvyxqcx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gisuqpiaz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gydkrzfzn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gavajjiik.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/girggdico.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ggdgjdwez.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmrtynwpg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gkhuzwgzt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gxugyatso.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/guqsmlcwd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gpwptgeup.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gdssmlzas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gaanqmibm.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/guhebmpoy.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gbvpvcklz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gpcdsjiwa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gspvocvhh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gkdbmjouf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gmuysylhw.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gxauwhhet.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gniakedjl.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gmohamxpb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gvvjpjcym.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gombdcriu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gmbnnqrer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gmbsoslyk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gmtsxfwwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gxjzfestl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gsrvpefxp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gbfitbwme.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gajkdhmhq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvccfijzk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gouaxrpbw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gkzygbkkf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gqghtiyhe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gejnoumhi.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gaxzhsagw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gmrmusyqb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gkqabpvrg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ghzyrodml.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggfbtnrxi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/galukdtls.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gjwvqjiis.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gifvcglsv.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/giammzfcf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gigaaaxet.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gptlmroql.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjxwdhubu.sHtML


<!-- 参考信息 -->