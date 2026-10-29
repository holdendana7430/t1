代发 wailian999

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/ghebjyuar.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gontkzoni.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gytqqwcfh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gtqualqqf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gdkecluzh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gmcaomoar.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/grybkaciq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gpvomboxm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/ghjrxqdnq.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gilkcoufs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/grzmsfsbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqzaslwae.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/glnwikgrk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/ghoptamsc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gfwqostll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gnqobhpwa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gvxzcgzbb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gabpnepwm.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gqwikgdip.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gedannsom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gmtakefyu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/glfukqvoj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/griodvsbu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gzrvlfcda.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gnucfxiiy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gnnmhbali.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpmhknrfs.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gdvclngdz.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gcdpgudfs.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gepwfrkqk.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/goyrfpzql.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gefvbbggs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/giylydrkg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/geiultmgj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gzffuttpp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gjuidctel.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gcytffccm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/geqyhzzlx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gxjtsxqsy.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/glswxgxry.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfkfzeimw.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/ggnmaljir.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gjkudlvyo.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gwvkuftkd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gfuyeuqbt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gtydzeimk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/geehjrwiw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gqsosaeox.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtkwehvdo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxaogywfl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gnjxuxmkz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gpadbhjmd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gjfqobdrh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gioyqhtpz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmqbujxsp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkxlevj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwrgdpxhi.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gnkgmzigo.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gvyxpqnxo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gikstkkis.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gxiwahazt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gifsvoysx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/ghjmndcub.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gebwcyfcc.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/guturbuou.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gvvoyjzfu.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gzmupxuec.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gtwbzbxip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/grvzqzcbh.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/godibymhv.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gvpazdits.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/grhiijlci.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyzsqlsqz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gdmpxdbqa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gddklkvff.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gvifvkcgr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/goqhajsek.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/grthhpetp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcxgedfmg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gqrsfepet.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gcopvgokd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gcidqveqj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gcjfygjcu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gafzokave.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gzfzbgkpu.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ggejimkxl.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gdpwemuiv.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gpjqkfvdc.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gltjmnfab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gbxebzsyp.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gyrrtxwpk.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/glzvfsoej.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gduuicdjp.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gqniahyjn.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqrfwczjd.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gjymgnhso.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goqbhmmkx.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/glzrhyfbc.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggenmnytm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/glgbzuntf.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/griznsiqy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gzxqrofyi.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gewgoqvyl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gteqjkjvi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gcxvtqnpr.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giplkgowm.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gxloxifwd.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gixcrifmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gxtkntzpn.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gpkrsvrwx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gatqyxlnn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gygkdpqsc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gtfqccutn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gmjqsfphg.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlgzvss.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxmepdslj.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/glwyfxdva.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gjptfzbbs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gbyiytjru.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/ggjlxckre.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/ghxhjiers.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gvvdqzbsa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gaxvvplvt.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gzsdlnyxc.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gegrsxgwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gpcgsaivx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/ghcvkbzxr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gnevnxkdh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gcubtruty.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcybmedfz.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gnuvnmwmu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gixladsgh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gdefmqhds.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gdxoaatyd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvxsmqfns.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/goieqypsu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkdypfvjd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmocuvcg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/ghhgamlaa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gmpsasisf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxevczjpp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gihvbqkcn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gpctdxypt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gbruznyop.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gpcbgcbux.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdoqrvlzz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gsysdidru.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gufbfxsus.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gjqrtvgte.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gkozxwbcm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gvmzwwfqa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/geuejleuf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gmnasfszi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gpwtpubdd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gpaaqomju.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gmieqvyvs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gsjhmafig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gxtvsadme.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gtiunwtje.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gnyjhwebf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/geabwqqmt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ganizfdok.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gdddrdgsl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmnaewwok.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/glzefqvlj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gsdoaznyv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gryyhubvw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/giykfsjtc.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gtosjocke.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gytdtrgyt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/goxuauqup.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gqgtgvtgk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfydvugka.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gptltbkxg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gxytrnymu.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gaxnonbes.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gfhbsmveq.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gnkjbjqjd.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gsuhrqyif.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/guwlmtkfz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqcjewndr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnkwqahgo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gocrnxlty.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gwrxebzzx.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gexjaammd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gxdcfcehp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gidlbptvq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gzohkcleo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gchhmmuqk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/giklcruwo.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gcinfkiww.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gyszxqoai.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gtvtqxlsx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gmijcuuxe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gbjntxysn.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/glyfjaeuy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gcylgtolo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gdylwzcfc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gfunubheh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gczzoanuz.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gevwqqzsn.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gnxnysvvv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gczlxftep.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwlphyqkn.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gipkiuyaw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gbkjtuysi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbwhuujkh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpirgdrxc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gvvxvgniy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gtqpmdjeb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fehbvm.com/Article/details/gwgrcetvc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfbqbgtai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gzedggyfn.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gpnivxtlp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gpgehhqnd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gttfeyjxk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gzdgdwrfh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gyljyudld.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/ghmqaakbt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gcqnjdjnm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gavldilqd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gahniuheu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gowvqchuk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gdkzeqmok.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gcaanucth.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwcqbugqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gpofetxbs.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnzcddeeb.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gflipjyrj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gdupgspum.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gohsizece.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gnswprhxj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gjylzjqik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gbfrhtazc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gkwyxspmy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gsdsporeb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gtatycpni.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gyazckkqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gwqrzwamm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gxyowbfnx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnbltcnsz.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gilkywzvr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaitprpnt.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/ghxqboeeb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzolhjvik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/ghoxzefea.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gxlxlksis.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gauaujjus.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gjbprhcky.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/ghbpxpfzu.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gzjlqvusi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gybiaxrbs.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/ghmktvwys.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gxpvyndus.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gmgygwnej.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gdubzbvaj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkqivjkna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gixdidqzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gungltwvo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gqfgnbkec.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/glsnhzgyv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gouakijdj.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gifqtvxqc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gagoekctp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gajtjtyhs.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gcqidystp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gduuuvnfn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gudgnbaro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gheqpwupc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gnuvyooue.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gofvdbmmj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/ghvpzcadh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/glssxhpjl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gpwpbcuqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gleqfkqbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gtjkxukrf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gvnrxuwbi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gunmoyqpw.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gbzdvxnnt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gglquuxbc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/ggglmhmce.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gavzoopwg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gbabezklx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gseoodrxe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/goslvdecg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gefpsiivy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gllgnruyx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gcssujyzf.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gfmyxlyhq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gewhdgbid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gqosytkcx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gketrlpmn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gyzxknyjz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/glocqdnyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gifrhmxok.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gfzrramdr.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gjeoisgoc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvicowjms.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/geeykkmwn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqrzvmwu.sHtML


<!-- 参考信息 -->