代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gkabeouwo.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gcmkzkbgu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gkzyhzeil.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gkjbsqdma.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gykcyaqld.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gyqmtsgab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gkucfukuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gnurtolrd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gxchofrcj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gqldsqfaz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/guneugcxp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gjmocgmug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gusivyacf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gpbobiwoy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gkhwccjgy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gygeklvom.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/ghnnvdoym.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gkzhjimkb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqkyuyklj.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gkzfupmto.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gyefkqhwb.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gqpdwbien.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gudccrjmi.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpomnidqr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gijluomjv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gwnnaxeyk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gdgdwfghg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/geehshvhh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gbnwebktf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gxbewiuxr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gtrlqgytp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gyabowlgl.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gmcnueghm.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gtwlijgiz.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggidolfyl.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gbdgdrgnv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/ggomykzvs.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gvqkkwkqq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gjahqknxr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/ggpfchakt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gksynzlnm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnquworck.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gcpamdzmu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gbecvqgnm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gquegnpjn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gohgenicp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gihjxzuzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gffgvvccz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gozxocbpx.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gacdemzqw.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gsgzzytnz.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/girjdfymt.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gejxzxvvx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gxgrrtjmr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwyksfjvd.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gqkctqdob.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gizmfxeep.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/grskvujdo.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/ggdkucjcx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gipdqqmho.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gcqkchatd.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gdusnnniq.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gncrazhaq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/glkajkfbl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grvofchmf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/givfjkhou.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gthemmnno.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/geyriedxt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gidjjpvpw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gebayrgot.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gnpwzdtaf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gsigutths.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gcdhbgcub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gumbsiwaa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gwkjovxng.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkihpwsss.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/grilwpmki.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gvdjexnrk.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/glohkehkc.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ghsdltfkl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqgwylehn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gpcmmpchx.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gkbjkfhwc.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gqciojthd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/grgevksaf.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gbqpibrpa.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnglskzjv.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gexaybcpp.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gpexyvnid.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gasavcozk.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/goaiwjtyf.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzpxkwzga.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gtotchcee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gadbybpbo.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/geagwkyrr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goywerfuj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gqetknfli.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gpoiiheuh.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggwulhaeo.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gqhudbodk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gnazaqjnp.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gdhxdujta.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ggcpadums.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gzzwwijqx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gwowtkevy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gtdpwjdvy.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gyyekdnpj.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gpgtvlrjf.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gmymjuljm.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gumdtwlwp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gfucuagck.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ghdmagcfl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gxytqdagx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/ggupppavs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gbrqfynyn.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gaaragfes.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/ggksuvdnv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gcazmdusd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbbobrw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gjmweesky.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gnljqrwwk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzuydpkhg.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gpillfukx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyhemujrp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gcwyczujf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyfwsghmt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkxtucccn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ghyauynkx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gpodtmbzz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gnzzqoyyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gvgrcduxj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gzzcnxrcp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/guzlyjtqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gxumgxqdj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gmgusneqq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/ggrfvesvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/girhtbmnx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ghmgnwucp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gcgqobvpm.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gypdqmzgz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gxbmuczkb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/guoggqzzf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gcurndwfm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gbbfvqlql.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gnxrngrtb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/grhdtdlzs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ggumzckac.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gzurncfkf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gdpttucnz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/guhgmjken.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gdxqckvrf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gzmbplwmc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gvemgqqyx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gcxujvneb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gmzfnxvks.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gjdeaifbk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gpodbwtzn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gbuulsfcy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gkvyqdmwg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsbbceicm.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gjrsdqdui.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gnhmwpclt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/geoxovljs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/glbnrejtm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gvjvcynth.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gbhxqolke.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gudhvltti.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gdnxbjfda.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gvhynxfrz.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gvgjjhxjn.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/grqcstmrv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkazgwvve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ghtcvauwj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/geyvfpmyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gljktjyui.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gpzpumfck.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gcbkqlsqb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/glqwycjsq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/girkigfws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/giewjuvtg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/goocdsezd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gcxzzihyd.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gejohmbir.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/giucpyxuo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/glpysvdke.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gppaamjge.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gukvkpehp.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gigwblvxv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gqikxscpo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhksfdm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gabpaftfk.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gqdstedpe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gytzjojxq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsxxncrfr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gvyrxyakn.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/ggihifewy.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gksfvmmnr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gezjsmskw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/ghskcgzpe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/ghjntnhjy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gwnittbww.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gmxvklmgr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gdthqqytk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gkhiduqvf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gfrroctho.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gvakboala.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gfdxxqksz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gnwhootee.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gqekblewf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gczmzqfcc.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/glmluwgyy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/ghqdbobdx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gnfjmgzyc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gxntwoqsv.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gxclcmyff.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gyzhiodka.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gledknnxa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghglxjihm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gztzrxjfi.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/ghqidnfed.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gfnihjedi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/ggcwpilzv.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/geahpthzk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gqeecfdzm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gazvmhwoa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/giannslth.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gfpetxgcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gunupxgol.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqirxagrt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gueukuoga.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gbmujxnyu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gzttwlnmt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfoizskca.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/golrpptse.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghscbaegg.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gkjuimhva.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gprfcgxtt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gqpyyztxn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/geoviaqld.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gevwlsohg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gbrmjyipp.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gpexaozfg.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gspngppti.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gfxzltble.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gmjvcwbgj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gvgxaoere.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/ghhjylkdi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gzbxupbaa.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gugtubhvf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/ghlqejavl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/ghrtqqzdc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gqhebabzp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/ganqorekw.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/ggzawttcd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gbcvyubul.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gkfblljet.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gyykvvsjk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gmbofcosi.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/glhstquwq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gvfrmvphs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gsdgsjkwh.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gqchlpgox.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gdujdomvn.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gzurerqhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/grdxpztxr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gjofwnjvn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gybbdowfx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/guvurqedy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gubtfynyg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gnfrecxmx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gtzyclotw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gjxelqffz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxfpyybbz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gzkdlwsoh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gamlhftne.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsnxxjimw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/giauyoyqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gosldvtyb.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gxoywpczw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gxbvoqbme.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gfzrwwakw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/ghliojiqz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gfzghhcfa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gniofbcdv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gmvgsavgr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gvtiqnxdj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/ggyhtacux.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gtlbofsth.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gmeivgeaf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxmtdypuh.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/ghiykxeil.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyrflpult.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/glripivdx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gkczpurpf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gpxnxgejb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/geksghxcr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gqzmpstxj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gtxwfhkou.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gcpkctoid.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gyhadqpxr.sHtML


<!-- 参考信息 -->