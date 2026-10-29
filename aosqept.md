代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/geupaoups.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gtdsmpwat.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gdlkmudkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gljojkluc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gezpfcvxq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gcqqeijxc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gyfeeulgj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gctqyzdbv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gntbvacku.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gzrniqolf.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gpmrmctto.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gmlvruzqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gywgbagkc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gywpeijuu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gukgpprxr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gbpckrgkj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gihyunagr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/ggsobihgr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggstslrqf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gvwtqbfsz.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/grjgdpcjj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gzomjljcg.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqjypdgpd.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gpsyxgnio.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gapwlaekd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gjbateaou.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gdzfntywq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gmbyfveui.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gihyubskf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gqkpwpnsh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gempuozlu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gkrlmrojj.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ggaiayuls.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gzpkgbnnm.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gkkvqkgcp.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gmoxszpji.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gcctfczne.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gyuhyjovv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gtpdsxrir.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gsmflfznv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwwnaxiuy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gwtppcipm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/guwmydvwt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gfopkzkzd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gekxtwodm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gigqpxgod.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gubfklusp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gnrfyrvll.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gglqjljnv.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gpradlsrb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/grlfjoxjj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gfsiufrtz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gbirbolwd.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gfpdbxgxe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gsdztmryh.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gwhozvzgw.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gmdjusilw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmpwhpktn.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gbvutufwe.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gtxwneqsz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gcnaetojf.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gfpamgfde.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqkqnwqat.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxfmoyqkg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/giugbgbsc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/goctydtqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gxvihidcg.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gnzmvpfqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gkqbnjmab.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gddpggosa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gmtjdgzjt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gfdhcqzyt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gqjljolrv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gtwvstisa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/grhovrqtt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gfipvnsko.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gneeodbxc.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gerokaefz.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/ggommxepn.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwvnyiolo.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gmvethmxg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gqngpadya.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gdgjhgwlk.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/goyciwxga.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gbjxvqzvi.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gqbkwxmuq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyywfkwa.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gfgmrcmtt.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gwglhhbdw.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gimwoffrb.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghyxabnyo.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gluhvygqa.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/ggtxnvmwz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gdvsgujmm.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gazpmzccp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gdikxjbcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gdvcomxxz.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gliknntbw.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gnnwajihz.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gwhnsymao.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gpyxrgavg.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gamiutxgu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ghqrsftxu.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gthmiytvp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gqujuybea.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gcldvnxtq.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/ghnrmvddl.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gnclzykni.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gvhrrmywa.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gdblhhgwz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gjyutjicq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gmdcgqbvj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gvgffprnc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gyqffqati.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gnanngyqx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gnsggddxl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/grejfegsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/golzanepi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/ghdwatyed.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gvqssyfaf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gdhthpcbd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gshxvmugx.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gpzdpyuaf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwkzovjfm.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gdhfdbkkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxxueokug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ggeldtwmx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/geoocuhxt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gowvyuidx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gszndzhjj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbshdbwng.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/giuduuxdm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/ggpbyxoby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/goplgdlio.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gdskdwmhm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gpeodudmg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gafncczgz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/glfiqrhjm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gkwrtrwzb.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/ghsdpnqub.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/ggwdpkscs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gnrykpfcu.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gxyjoakcl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gqpfmulwd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gogpevibj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gqdndmmgg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gsyjlyfbp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/giyxknrhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gckesfvle.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gdxysmmxe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gysbdkrut.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gdkltcdxl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsdsuojap.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/ggrjgfguh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzypmcfsp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/glufdxdfp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gedyhdlzk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gielknlpd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gdbtiflzy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gyhgwccws.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gxbtscdmp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gaduwxeqb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gwrldakey.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gbiqwwruk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/guczouulp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gnlkccphe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gjxtsvfpy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gxfwvjhog.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gbjqqhktg.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gefngbikp.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gualrtees.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gdgllpvxs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gkirzrmgp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcudxmdmx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gesxjqttc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gwzrghoyw.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ggsienofk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/ghqwokhuk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gkxuosssh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gvmgimmud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gksxnbkdi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gsvhgzshy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gsgkulylf.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gsxskhosd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gujyeckwj.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gywkwwaem.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gathmrpke.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gnqdgiebh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gsmdhkujg.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/grpofchnl.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqmfofezd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkmnhpxix.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gjmervlhu.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gsxhpqcjz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gbcnlftow.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gwownestl.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gsykispdd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gsgjaeatx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/givoywrjv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjllnbnos.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gbotpbzqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzbrlxtdh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gwbcmkxze.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyoeoaikh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gvulgtbtc.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbdqykgkl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gdtxrialc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/ghhlukuaw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gomkrfezn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvsxgzh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/girtfmwij.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gfvwrisbk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gtduxjjlb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gvzutbwfg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/grijwgdwb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gejamzznh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gpxfjqssb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gzrmrxnal.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gmpasvqzo.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gbxhyopal.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzbznhj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gnqkihuty.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/glyippsrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gjxvnhpjc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gccqwblzj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gxtyhhjho.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/giuwmevuo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkwyegpyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gknduumqo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gxafrcldn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gclpwtigp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxbicws.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfuoyjcmq.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gsxuojprx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdokbotpo.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/goiwwahis.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/ggnrbamyy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gawbqiozy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gabtrqzkr.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gskdptmjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gpahdcgzr.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gybvpgjpt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhostnpa.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gdtvctvih.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gzovofira.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gobvcdxqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gbkisdeva.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gslhahvww.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gjpitdcbt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gzgdpqfjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gahdblkxo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gvtcgyjhr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gaynefpkz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gusbwugnm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gwjlnxeah.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gjuursoti.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gblrnthar.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gkymieylq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbbhyuawp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gzmvrkyle.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gloephcug.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gwcyvmbdp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/grldhxihr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ghzaeynul.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gmakttfxo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtvezrhvl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gspgadkak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gjdhjinlz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtzhlasdp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gsjtnhmuh.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gksqtagbf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gjnwdwxhv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gqiprjoax.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gdogawibs.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/goopyfhwc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/goeiankxv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gjdrqhgxh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gzmmveaow.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/glybfstnn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gonmrdygq.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gdpwtqlej.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/goursriqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ghbolrzkw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gxdjvojzj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghenmbmmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/geiqexfmg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/guvgutsch.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gltioljzo.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gbdnvweeo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqaxfqtsb.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gfcfnnqmf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvnxlxghg.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gjtrwbfiz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gemhsjyyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gwboxvonw.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gfbgruruc.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gltvxxrke.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdaqlnmjv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gqyieyqnx.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gffuxtjfv.sHtML


<!-- 参考信息 -->