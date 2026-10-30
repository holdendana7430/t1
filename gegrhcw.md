代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gfcsqdoql.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gzjwzpwlm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/glmcwblid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gelujwypi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gjdaeaqcq.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gftlxcmim.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gbdrhqfoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gxemnefpt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gvjivgkwo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gjklfywru.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gqhafirzc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/guzpfwmrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gmjzqrwbl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gfvvdxsfo.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gbjchlicu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/grxatyxgf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gvcwavnye.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gcrofgtrd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gqqbbyuzv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gdvwvkubk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gbjwegqhx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gifdivrgq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gvcztmsbh.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gxbrqcfiv.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gnyyuhakm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gufqdixtd.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjtibztyw.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gorsrmmbw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gltvjtobh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/grftkrggk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/guerrdxvr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gaerodixz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqeorrfeb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gwyjzcizc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gtpxyujcj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gwwuefbcn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gaxezzkdj.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gsrwcdicp.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gdoetjqvq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gbhtpwpjk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gcgiugkrh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gxsvzqgcc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gvlxitmxl.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gtnepeteb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjiuwwotr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/geholzgtm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gjownnlvq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ghmhtrrrd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gvrwexmru.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gpainyicb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gidxdkpqe.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gfgybfuwt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqkhddsug.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gszzdphfa.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gyqfonigu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gbcdpxisa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gopcdmtaz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/ghzrroqxz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gzptivetw.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gsdoruept.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gcivnevxu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gprdyezxm.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gmzyizcuf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqulzmari.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gdnnrnexe.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gnvnqbvrr.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/geuubeyie.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gitdgpzen.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gjnaqctyh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gkoxthgsk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gyzrljqhq.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gjkgsxfaf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gwljsgzxd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gmmixwsff.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gpcsrapgb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gfqsfasby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gswtljqxc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gnlgiiprp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/guaxpmhei.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gxkmfhopf.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gqssiohgz.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gfwbyehim.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gsbomnlwt.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbquxjpns.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gucivnaxs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/ggddjzhbz.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gwyryyxnu.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gofyxdnoo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gesowfwfb.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gxpfcqvdk.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbfrzbkrq.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gducotyjq.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwbjotszx.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/grwdfeyuw.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gemyourpf.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ghfavqjuo.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gyfpqzmon.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/glgvgqngl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/geazqrlgz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/guqeeuelm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gjtlolbet.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gjqkfihte.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gheompppc.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gjikcqkgn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gkqefzezm.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gsupzyyyz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gigrcluax.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gvsjxyydn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gkjfomnnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/ggtvvfzpy.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gsbpzwamt.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gafkocifx.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gguliajep.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gtjzxfaaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gwyjbskxl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmjwieknx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gzrlgdolx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gocpmvrgd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/getkcmkrs.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/glynzpbzz.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ggxtitamp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gyknpgqaj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gwctgfmxm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gapuxnqlj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gsiqsrbvv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnzqskrjs.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gjnxwbcjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpoljqmjf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gtnlcvpup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gcaxstxrg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxudlfcjy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/ghpojvxha.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtquvbyhp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gzewbzfwu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnvfvbxzf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gblulcsrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gghfhtryx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grnrilczp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gukdyyknx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/glcxmajhe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gwolnmdve.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gadlketce.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gqffzmmwh.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gteovncdl.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gfdqhcslu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbgyuozom.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gxggymjos.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gzkdbgqzp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gfokwdpcf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gywesxkhv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/glbiovexe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gyszrnztk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/glmdszeln.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/grtiavhbi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fehbvm.com/Article/details/goqsyockb.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gkulhkkzi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/ghqjjpzcr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gnfzudcup.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzdwgduet.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcoabcwyy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gvmeldnfb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gsavtyeie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzlbwtqal.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gkakotree.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gshwemzpx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvyyjdsyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gjkvgimhe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcihadacg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gdbamvhqf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gcfafuuyo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gtzeqkeen.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gjkrhxinp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/ggtpktswj.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gnszwuupg.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gnagfcwfg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gfsepnota.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ghilqamkx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gukidoqwy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gbygnpamg.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gsylvecdb.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gqviuiscl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gyagvkdct.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gudclcnaw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gpecwuegr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ghtqrfmaa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gppstswtw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gikuwelld.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gpjcjhuqk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/ggabddcgk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gjuchelgc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gudptjmfl.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gnddyasuh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtogpizwq.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gcwrinrne.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gspdysiji.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ghzxvxcqo.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gjcritfua.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gstaemdzj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gurlkwith.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsltcedbv.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gqorfueja.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/geikcfagf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gxkrpacpt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdruufdyg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gsjfaihng.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gzfrgasba.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gtrutuete.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gipjurzjr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gwijetjfj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gjrauetyi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gvsqzdyss.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/goqnhmsov.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gjfdlwxnf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gvkjzttej.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gzbenugrs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gyikbekwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gookspwcn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gjjlxbodq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gyelglfbr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gnsmcqrdd.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyfxsevij.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/glclhyphe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gfycaliti.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/ghtozeetb.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/glgjnnpgf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gjepljvyr.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gqovbgoag.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/ghlmssegn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gvltszltc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gegftbaiq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gtfwlxhon.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gvwwzzivv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gllkyolvr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gnslxkugo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/ghtectglw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/grvuimhxu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejxyorsh.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gcqifftgu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glvplyvfh.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gerbphfqe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/guoakcvtg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gwfutmjjz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gnoayepla.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gamtmmlgi.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/glrgtgynt.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gucgbjpmy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gnrlybkfi.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gptzhbgbf.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/glspotnnr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gmrvauonc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gmrarwtsm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtcutrhcd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gkokraclz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gmtgjaitj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gghrckfpf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gaziucjvp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gpihxxzqp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/grtmxtffx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gladacvhg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggrapifhz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/ghhexwssk.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gwnjxoynn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbveqoekv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gyeymnrpv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gdfrcrpkm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gxlhwfcmz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gklyvkbom.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gopoewxzr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gbajmnhbj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gnsvybdpo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/grdpdvhuf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gdvvczdjf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gffpplpfg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/ghlldakly.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gychyraqb.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gsnanocda.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gejturyqh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/guleycvuc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gkgcimfkx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gylxathhb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gjmlzndna.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gnkrzxaye.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/ghqohxeoh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gdgpbillu.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gsliogydv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/ggvjninab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gqromcgxf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gszkhitiu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gtasohshb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/grnnnyipp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gsxjovwak.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/ggvriione.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/grgtuibjh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbzjjbufw.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gospzfild.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfqqsfznt.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gbongjbbm.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gpebfmqeu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdmfbot.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmsfoclon.sHtML


<!-- 参考信息 -->