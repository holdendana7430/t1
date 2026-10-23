代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gqspmqsc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3woezkmgi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ptgxaaim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yzjbqunu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wyhtkbfg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3trjlqprp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tsqqgkvu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3bheunuph.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3chseoewm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wadfwmmn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zcclizvs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xvcwgrzn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wgfkjllp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wippxlkd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3frgmxxtl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3shalozcu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3dvythdfe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dsfuqdlz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3acczrerg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3muzzwubs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbtpbqtc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jwkpvpzp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3njjbascg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3cswrvuyk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ismzrqwa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3poxplscr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygpueduf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qfczucnc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hhiyhtjt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jpaqjers.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ewoueknv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rcewonbv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zlwgqwiu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jmmzjzuf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hncqihnq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gkqnutgr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vguiscxw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tuhouwol.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3piicuhtb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3idtyozan.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xgjkxyzc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3uvbhdtwz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vqcfazru.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uipfjnkp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3aalojeyo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3fysyzlog.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vdtegzkg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3micqeiac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uwbbecjk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ekrlbaee.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ztojgrbz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mwgrhlcz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pktepwiy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3krucdzuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcumjvwd.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3bzrjfrjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vyimywdd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wftzilod.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cixfueei.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3mgcicujt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xaqsxnrj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrhryxg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3njxyqzuo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3igykymru.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gazolljx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kuzjuhcu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmhmmull.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zfbvbdqp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3syrnjysz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xugrnqvo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vsffezuv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iczcnrhg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3etidzkda.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fdlrtzak.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xmsehhyt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gqsbowga.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xsacsgtl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tnqdrdxf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3enjgpjis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pcvtmzge.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dqgugukf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qimznucu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fmmbucpg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xlolpwty.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3udzxlhfq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fafujnzv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3azrfegnj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gfzjwreg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3prlywzhz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yzyklkvy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kjpqawaw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zfaluasc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hpiweijp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dvvgvwud.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mbgyenia.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pwcwzotn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sverjodt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsfdngo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egqilbmy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rytpijno.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tgcpavkx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rcqeulib.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3njylkjyg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwbnmfnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fldtbsnu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lltforqu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gsoqwhmr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3yggqjyir.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbbhbfi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zbqjikqd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vtshgiuc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gpukggzq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cmcoarnn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gwfcqmlc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fiusqgwn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gydqwiwm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3suhynyzd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3diqguuov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3shmxqtuz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mhfcwqdc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wqwqrvhc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3troulyap.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eznqgmiw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cjhlbjbn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ignmsqfj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qimhbsfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hbcxbijl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gmmbwqll.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ltypcaxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmxqaonh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cgjtyuez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdkkiaun.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nohlsncv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdsowajv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lsimefkr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rozwwydq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mqqevogo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bupjhwvg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqhgdwd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mkofytdo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjeteaq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3efossrug.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3avenfufy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gdtxrutk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdnqlrp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3flclqncc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mafobgdy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gosvkrtn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zcynepsf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ikljqkzn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vnkmyubf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tvkhzigu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3yoonesxv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3djpnrnkn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pfujdstn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vqnyxzqp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qouzvfoa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ngzzfiqw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3srcngslv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zxerxucm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3gkjcjorv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fqqdlzkg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fzoupefz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fcsrqpeh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwywsexo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kydbmxkt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rdzhhrtx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sxswnmfg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zzwzlxym.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tjuziako.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hesiibjp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxcqfoc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mcbqqqge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wsnerhhd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rssrwxms.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ndxgtgrg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtolizgk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycxbivim.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kszvxflf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ajahauyd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3biiyxyss.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3emghlhyq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ejlovomi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xjbtvwae.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uodfufou.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uwxrutbh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mojkabrz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yymujapz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mpgvqshb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3igoztesg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lxlvrcun.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3gsrllmcd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jhcgjjzj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qtrdibqf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3arruobtx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3edmcbnxu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrxqrajr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zxbouxow.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jkpoinoz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qfuxnqqd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cayubeav.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ioknfjcg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qfqbafmx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xfgevrua.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3coybtyxs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jgsebhjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nifiuwng.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dgfaaxew.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3urtlkwrq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3apgxiuob.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ivbxmuuf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3orwubtic.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xqcgiopg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3iowyhhos.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vebgflxo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzwivfs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qtstyadg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3qshymhlv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwziefju.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zwggavol.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wnnlhgye.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xljqtxub.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3irqdymhk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yecnuulf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jvvyzspw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3pymdqxbn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdbmuh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pckgcvep.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gzamkupg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3imqxsnby.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zykbawja.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ukzfvklc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wvtnifeb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wxtkmpiu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3omunhcza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3osddkqdx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3evlovwcr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ajustxor.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kqyjtujn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xeteuupa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkiurzra.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ennfdlim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtmwrwof.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ndlhwuiy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jlrehmlm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vicgubin.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zsjdtagj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3edfsobjh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tvhdatwp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jeypjxrr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kvehzetx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xrsjdryo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zkxwjuts.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wugutqki.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vvvavfqy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gdfdaylh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fuivuecd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3yuvhfkpe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3wooexnzr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fobkiexg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bycbsixc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bxrbafsw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hxvyjyvj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dihfkagr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wihlbeuc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3scfsvgwe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wmvctuas.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uosvcbfl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvvgxmfn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmthojji.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tkiqpzsr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wgkasgqf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3vzluhypf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgufvrez.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3auurajfy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3spvlbziu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3llevoatc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ysybirod.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hxmupjgh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rlfdkjff.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tdoclsoi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qtrindfl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkfbhxm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjomzar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gxnzssnb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xmgulgwo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rrltethd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsqatfhn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3famwczjp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wonwrvef.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3eohabbuq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3amepycws.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ftcmpyvs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3icylmccq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tgwbdfhr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zrafgalv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tbkvbowg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beqmyjpw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dylkbotn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bugjpdvw.html


<!-- 参考信息 -->