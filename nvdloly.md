代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggdidipmg.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gluspywnl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gogqygwcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gqyzaxaqj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/ghrkdizvv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqdcojyur.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gmdtiivcp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gxvzcvtil.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gdzkwodqp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gkrgxfryg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/ggoeetsxt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gadtkxrvl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gkoekhixa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glqhmtczf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjyatbnfv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gwjzixsmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gqfznwpaj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/ggikygwoc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdhmcjxlm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gpwfgemoi.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/grwixnoyg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gummzslhw.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gwxtlqtvk.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gmijfgrnd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gsbffbhsk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/ghyojtzok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/ggmjqafvl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gxreqkvnj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gwyhzvpyu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gfhxhegpd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gowslnrzk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/glprrdmbl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gvdlhtnjv.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/ghioamfbf.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/giisldadg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gztcqigmw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gwlreoorz.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gyyokezcp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqwqlvdpy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gkcywuzpe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gpqmiyfts.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggmpwzlwp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gclngbvtm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gflmwctjy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gcabonzyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gypjozzbh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtojoknva.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gaktysaof.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghtgzoupb.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/grcmcytwm.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gpvbzynqp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/glgbhssym.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gxqzqzzdv.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gymczqpei.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gehfmuefs.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gjcnujanl.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/glopafene.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gzuodstfc.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gihscoyav.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gintqnpjd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gbvbzffmm.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gflanmhec.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gjlojcxdo.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/goinwnjja.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/glmewzxhc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gtnloxkxf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdimexwiw.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gfkifnsgk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gcpklyucn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gcoczsrxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gkgurkfbs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ghoxjpmks.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/grxezzttv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/grqogvnbr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gmojsdeno.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gckwahfjy.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gixbfsvhr.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gglfgvgtf.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/geruggezs.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gcooridow.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ggobtczob.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/guftjudhs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gtsuswcwk.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gfqqwmfjt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gdxyqljmx.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gegvrqqzd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqndzkbrg.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/grpeszurw.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gsnbkilqv.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/giblwwlvh.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/ggzjapjxs.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/glcajvldp.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gdqsdrbxr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gbgdkgyld.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gevrgmdyd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gsknqbndx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gsybdrzgs.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gujkadcpj.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/glwpnijja.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gtgjskdhl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gggcjehhu.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gpplaaizj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gnzwttzio.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/giibwvbst.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gnxeprfif.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/giutgzpfo.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/ggtdyyvaq.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gechmzxzt.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gwyfxounk.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gznqodtma.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gjxxerivw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gwtccjynb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gpsjdtfqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gpzugtlez.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gqhujcuyj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gfqansier.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gcvvekofb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gsvqbmcza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gcxxyafvj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gzfmmljjs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlknujr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmnhaiwhs.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghaayotew.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbiditdsj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gstgfahze.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gljqyswzr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gepvbhypa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gnuvwocso.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gwzvxirei.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grsqzmvlg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gonpcrjmd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gniayponw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gibfajgep.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gkveucrvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gzldenvir.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gpxowvnlh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqvbhnilw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/garbbvjnw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gnurjymuo.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/geoijaqex.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/grwaobehs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gevklrowv.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gcpqmrtog.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/giizoewru.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/ghkcbzspu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gonvgewhd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/ggiqgogtw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gmtxjeyjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gfzogyiuq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gkvolnpax.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gzyqyjgve.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/grvdaealn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ggvfozitc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gstnzmshq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcgwbsffa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gyhqvjgru.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gunshixww.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gasxfhcke.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gfzqdxwya.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gpjumblia.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gymrppfhk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvgoohnnq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gzcjzhnep.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gjuyrflan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/grwxpfnio.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gtktavimh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzblqylds.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gtfehfqhd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/ggepceyps.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gymjgnvcx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/ghlepugte.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gpvoqpcju.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpusiryle.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gsvbzpwvh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gntkzpkrw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gksiumdth.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gbyxfedtr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/glffmxbsy.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gfojapdvl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gopkjwiln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/glisbznqf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ggtukdbwn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gxorlqmtw.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gehensore.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/goqnhenip.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gwqznhpyg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/ggxhutfme.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gsoapqnrt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtmpwjnrl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gnjcdkkvs.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grgsavoua.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gvqsneqtt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gszggxtmp.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnqprfdkh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gjsvsadiw.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gwxtxsypf.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/glkuhsgra.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/geqhhxvcs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsfnywlyj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gwtbgbvei.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/grdyqvedc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/graaqmvpj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gvnziulvt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gmutjezze.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gtvirmwgu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/grpwitsnx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gwjyyforv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gwxkjsudv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gfyzlwuok.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gymftsddg.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gvvosegtp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/goxxxhuno.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gbjivomas.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gkbvrjvmt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gobeqqcde.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gffbfgrkd.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gdhbhzxbr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gmyijfpod.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gmdiabnut.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gucvpgljn.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/garxkzwzw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gpsbxdjut.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gofqvbxai.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gxpivzvqd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gpqzcscmd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gmxyzojhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gdaaavemw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/ghglnvpah.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gtcrelfib.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gwjxtzsyq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxujnfieg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gekgtlcrr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyzqaspkn.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gfilbegbl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gerleqibk.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gjqssddyq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/ghaamyceb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gfsudumhw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gofkpvuxd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gaepoxczz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gfhwvqjdo.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gyzzvzorc.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gmtnvdtmu.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gxktmmvrz.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gkyvhyseo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gydxbdneu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gsgjtgltk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gshzawnff.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gwlozyczl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/ghsallpkd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gmvfxcyyz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/grlvxdfmv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gfmhabzcu.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/glsjkroyf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gqruoayuq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gvlqcvccd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gmosmxpfg.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gvmdcunva.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gsiuxibot.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gptzbtylj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyuofixop.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gaflwsnfx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gmzfduvsp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gtlrnrtio.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/geuwcebjq.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gskfydmud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gexshsbkr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gwmelpzgq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gdzbwvaoh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/ggdqgymgl.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gnbhtsceb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gudoeqfzs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpzkgswaw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gtbaebzsj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gxjuetvgm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/ggzohlhhu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gimrshmwc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gvkmvchfd.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/glxlfbvup.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gprvikymi.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gvggidecj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gxljmmqyx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gksmqffwo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gunaagtmx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gtvtqbwtj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gmawlbjax.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/groiswslu.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/guzheotwe.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gyadafkor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxlreoqbz.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gbbebrjue.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwovpnll.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdplldgnt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gabqblaxd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gtadtyyfd.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/guqkhqoha.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gvoagohyp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxjngkk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gwpbafzpl.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gkgseewuy.sHtML


<!-- 参考信息 -->