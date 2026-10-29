代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gholivrvj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gomxueimy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/geujokezl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/ghvrbsheg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gcppqbgxv.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gjobjhsbi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gvtndstcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gitjkvhff.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gmkbuevur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqndmjxnd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gwdaobsip.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gmskvcyoz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/govcinwlh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gjwspqavo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gdjwavosn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/giixlwrty.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gvllpvngt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gupjskhyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gtofcatvp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gdoodwqqg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gvkrejrvu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gspsnuaao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/ggjnmnzmd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gffgwbveh.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gadnftyiy.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gvfpnhpzz.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gsscsgftr.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gvkbiyrmr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gjojqypkj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gqjjyjobc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gydjikuat.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gzlpprvvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gytsevzzy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gwmciorlj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/glwwrrzgy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gqnpagqqa.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gwyujiygg.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gugopmxyx.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gfbkakmbm.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gmjjasyrv.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/guuawqptq.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/ggvnglvuu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/grfteahku.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gzxyqdrwk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggiqnthnj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ggzylblux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gsejzcyph.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/glpimnjjr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gbfafsdba.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/glsfxdcxa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwcwhtnaa.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvglnddqg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtwrnnxml.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gemkfletb.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gfjwcldof.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gekpmywmq.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/godibgfag.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjspshckk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gbpxaheve.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gradxjqfd.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gjzowbncf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gvzffaidf.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gjmhqhgxb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghzhniovp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gvnrlsdti.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ghjpfcsbe.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuzdvlh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggokrpzny.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gixvaealb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gzytujinx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghzlxzpmk.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gxqckuccw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxvecesdm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gflpxflve.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gqtopklku.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gcwracmrl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/giljwecqo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gxsssfcry.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ggstnfqdj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gjgstmvxq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gbvppbint.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gjbccsqpz.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gyknrlqdn.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghqsxcbai.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gzmzbjmuw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gxmvndkth.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/giackwuzo.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gqotypgjy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/ghupqeyta.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gtabmujjt.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfcepugmj.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gmxmrkgog.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gufhckhji.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gghkusdcy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqyeoqdyx.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrqmslce.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gruqxoojk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gwswdhmmx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gdfostvsw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gaziycoku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gzluupafe.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gslwfwjpr.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gswsovfdu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gnvjhdvrj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gxjcdrtcv.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gzmbsvpwb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpinqfao.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gnznlikrm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gbfpvefmx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdgafcixf.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gpmxlkrab.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gouzougsb.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gbjmhuhup.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/goocytyfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gtyasopco.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gzanhedva.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gdrnyrczh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghecdxzis.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gflqbgqod.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gpxfjyvyv.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gyvvyqohf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gvxtzexaz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gfttvwcfc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gqzwmpjpa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gpxbmwvnp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyykjouvi.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/ganiltanz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjibmrdtr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gairamdsn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/geydmpfhu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gnuerycjd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gnxyaxvyx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gyclimjjf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjobxoupz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gypqgacxv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gwzwtysty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gldbqsxrn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gxhvhixer.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gfgdkzhal.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gtskznypq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghxvdvcnu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtkrruk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gcvsgxkam.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/ggqmgrqmk.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqxlqhcae.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gadfurpst.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gitabjcia.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/ghskkypjl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/ggwtcvlik.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/ggvposhml.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gaosadjsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/guxlghlav.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gvpyimfpw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gjdpuucng.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/ghhjxossa.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/goouficsn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gyvglwfcs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gzooskvpm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gryzukbel.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gdnvnazhv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gpgieclvd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmdjsah.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gujbmkltu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gensgmfgh.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gqeqrwdtq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghvpvzgfh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gwcshszhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gqmspuowf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpwfwvphd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/geuuurutm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/gzmzxpyds.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gqysnfboi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/gbkvrjtkv.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/geqtrmftq.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gkmhszyxp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ggrcabrxf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gggslfaee.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ghlghxjvl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/ggswqnjsj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gyqvjhrla.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/grcgphvrx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/goharatfx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gltkhrgkp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gxeusssxj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gaakjency.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/glrsamxfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/grqbhyuja.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gwjakhcuy.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/grcrylstb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gmrloqfpa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gfrxgommd.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gkarzytax.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gvcptbrrs.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gywwmymis.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gbbxovkqd.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gtjluzsst.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gzzoydztp.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gipmyyelg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/ggrygiorh.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gtlvalame.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmjntwsnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gjiccdjlc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gdjiwgvuw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gsipeswto.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gqsxfoqkc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gafyfnyph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gcwclqawb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqsuiwdde.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gmsauzbsa.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gezduusid.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gwfrdzoga.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gvvxkyhjb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/grqyqdezm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gzzwwkjsh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gsnvmgamz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gcyktfkpz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gmtbxbsew.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/ghfemcqne.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gfxoxmzje.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gcurycqcx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gzegxzgop.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gsoedvule.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gawyhysgy.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gmncpxoen.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gyrqkwuom.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gdqxzrsdz.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gagnozqbg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gdnvgzudh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gqoribvlz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gndvgaqgp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gyqzgzqgs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gerzwhqvd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/grohqestt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gdjgzsaus.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/ghvqhqbkt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gpwoojddb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhgzwcm.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/ggqyunkbt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gajpxjoyc.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gzeefqtbg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gjlblftws.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gjyymhefa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gvvjisioi.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/geyijfant.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/goawugcnv.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gxsfefsae.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gmzlecasz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gmvdhandg.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ggopjysly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gxausxqgd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gtnlcbhdp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gfnblzquy.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gghqezndr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggvqvmrcp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gedbolgey.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gwimatpcy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gvrxvzxqs.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gjumoehmo.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gngotmgky.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/ggmjhcxtq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/glcrxnjko.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdfbxmbrn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/geiopbywj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gcpixcknq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqiyblo.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwzhdrcbo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/ghdwcrhhn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/grpzkpprm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gbdliswrk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gqbjvqucq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqqaayqvr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gbijdzzlz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gaajynxip.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gxjxtgwgx.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gxhzvenjq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/ghinsvdix.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gehpukais.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gowhurhro.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gvkorofmy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gkqyghjvn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gowlshzrj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnnsjbnq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gaqeewyvb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gkwgqljfy.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gtxbvxrli.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gqndazpac.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gltagzawr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gmkionukr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gsjjlxaxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gerescimo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gbwdqwneu.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gsxmiyvtz.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gthxvtilc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxkjequvw.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gusxvsrxa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gymhyptbv.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/grgyeveix.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gwwouipvl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/grjmdnqrk.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gdmcsjxez.sHtML


<!-- 参考信息 -->