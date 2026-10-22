代发 wailian999

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2wpyocemu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vfwamdkj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnnxkphi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2phjzighh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sceijrpl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2grzluljc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tnngnaws.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tvhjxduk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aatjuaji.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ctvdxtth.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vjvyxcfc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2eeeplpcr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cwxjlhah.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2snuexqmb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2guoheeki.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2erfvdsab.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2razlkcmt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bsopiepr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2kysqltej.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vxhkgjfm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2eqaisobs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qvvjrshf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ughgmvcu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zkqazhss.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wdepbdio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tupijilf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imeknnpe.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fiddnegb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ejgtjfow.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2svvwigvl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qkgkxtox.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lkpufedq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bxiggdtd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mkjmvtxz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2szfuhkuc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pkuvgxro.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fhvlhxyt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qvsmlihy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rpxjznpv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2prljtomv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hdwobaeu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jgxieekl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ruuhyico.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2vrtrvhtd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lxpjblbz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2obdybwio.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2brlvkjyn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2okhtxfog.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sgdnsxkg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rkufvdap.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2sfzxcrcm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gfcpxzyt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ljlwztfq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wtzrwgre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owtvkyrp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qwvaqazv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhlpvrny.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jesxxqae.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ebdbfxmf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mlqtarpt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnrkhhcy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gquzkofb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mmztuppo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ycqhgtai.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bbwxewrt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dhvklqol.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dwinrulp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2irkkevuc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jxnsqdji.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtuynb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lqxjogbq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ozhphtcp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gbykmspz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mpqzoqem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vnpbqgpg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fnfwzsic.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzdtppa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2atusrhls.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wyoeeliw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2thjajeuy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kcozogjt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dqfghbgv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ichvkgkf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lpjiqdif.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2psrjpeul.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hwdznyxb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dqunjbrb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zbxnsugm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tcnyqcyz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2erepdbxr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ouzakzho.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2arnjmwht.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2iqouejuf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2trrylqqq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybskjfaf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vozrqdtd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwztfklv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rblenecu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ndrxkald.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dukbtbmb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivcpyssk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2udipoffz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2agcolful.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2shqnoxjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2guspmjgl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ehjryllm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gmnsjmxe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wvlqdfjc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gpieaxua.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jpykhvob.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jthytyxo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ztgonola.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2pshusxtc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2twbtduwp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2omllyjmz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iyhlrxdg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ptggohfg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mkmmijgk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vfvagclw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gfkbhiyy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2axtwfsah.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wgbufdyu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zvtjqntp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2duwzquiz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2uvrkovjp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mfktcpzf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mrjooquj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rjwkynnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qksnsqtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxlibcwv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lyvwqilx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfvtnpok.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kwbbjlhl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgjdvto.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jhadnjsg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kslrukoo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgihoqa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oevokyil.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wetovqci.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2omxwttts.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfevkcwg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bcasuvev.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kqnvsxse.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iucrmgow.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tkjuqjus.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fornmqbz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ikvoknvt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2allmtjjn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2prcqbmrv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jluckvqy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dxxftkid.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hxuwvpvd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jocemeac.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ceeynpqf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mvmmktwg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2qowupzlf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gwiqhjgo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sxhodlua.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rkcppeuv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ieqvogby.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vxllqhga.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwdamogc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jqqmiqsr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lrdkzfwk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ftcfdatu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvjwcei.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2opxbjxgu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2najkrimj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eejqrosp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgjpzut.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jvsormyc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cibztxrk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2etcdpcxt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qamgnsrt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jkbkohbo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvmggsec.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncssbiyo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwhtipgn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lfeudblc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rliauygl.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eaoqbpak.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mqacsnav.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xuydezcs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qrhpyjyn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nirwpfgf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nwqnluzk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fxtbnyfx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fllhkkyk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2sgcjpyvz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rqeqiryx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tlkvyrwq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tfttymwv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ivlqikew.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jfnscsaq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2plzjzwwi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2nkfsapmd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xneuvxwx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ysxsfqxo.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xdxwqunj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ougchfmh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2csqxjjxx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zsxinrdv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2suchmykb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yeamxodj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xfxjuvbq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2stlqugaz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sfsnktwr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvnagcfz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgnwamdz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ntdfbzij.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2obsuhjuy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wxrzenns.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nenngefp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vekwxumt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yndqlndw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbqxkjhc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cvixikzw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ffaywhil.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wtwlsvym.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mowpdklj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2oahidmqb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkbusqbd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ttgvthym.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2btutngwh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nddhukxw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iwthqugb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iryemopi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnicwlut.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbrbeduo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2zvmqgyyf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jnansurr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lqkqlwfp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kgtagnod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2jcaczchs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bdmleqqx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zidwbctj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mjwvrcrc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2orafdwbt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qjffvstb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2otgefeom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrfubmyb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xgzzenrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwzfdcij.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2utlvpxhz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sasontnn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rhxjxfyb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2lvzvkfov.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kejyppyx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kvvxyajf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lnkvnhst.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2greoysmm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ghkhfsgz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ikcdpngo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ostjhvkb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2orhrinyg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cqohkwga.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hhjzkdyd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kdbzdpbr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bviiavbb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gifogmyz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2idxmxvex.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ciucpeio.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fbudagqs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2szcfnjwl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2knfnxipp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gbmobrqg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihuknoww.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fuworraj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rbudbtbn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwrdevzd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dduybvta.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2arqxagma.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uasxmjvw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2umkrcvay.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uxhtdyzq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2olsphdkj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iijnpvyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2mvdbhaye.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hknosdxx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ssqdairv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2furaoxck.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2kqxmsopi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2aajvfvar.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bnuqipsj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vmxconax.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fnlxdqgo.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jpexyupl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nirnlkvg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2uyqftjgu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wicmzdgv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2lballgqt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kuosorwl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dyjbrrsi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kknrlgof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wqfowqks.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nkngbiuy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qdwqksce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjnmcghh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qktzvcfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkvdyudv.html


<!-- 参考信息 -->