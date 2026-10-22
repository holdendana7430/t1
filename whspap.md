代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qwbthcjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dnwahmus.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jzpnuubl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2diizfdrb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zmczzwxu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mpwqpfeb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbbugzu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bjoexzus.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rihtwkvm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kaapfkbu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2moilpjju.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uliypvhx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jlsbrigj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gkwdybal.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mahfshis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2xoafuqna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qasrjcdo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ehycmoia.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nbyztaxu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2btlpjzmh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rhclgako.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2aefnpqad.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jxllzffn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ognhwxwe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2awkyaxjq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjfovav.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ttbciszq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eymkgylf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2keeaseny.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qcepmcuq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ynsxchec.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fnnmrkvh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gdayoftc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mpfohvbn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2svbqoswt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2scdjknwj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fubvajmw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hwppwmxh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pbqxgxjo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2svplaiya.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2siavxviq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ejbbivkv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xrtbfsnw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ymsygzbm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nubldckd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhweznad.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rptjurgb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bprtrwuf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zparmedc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mskvsxsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxgvmhuh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ldttzfwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkjzrxou.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sdtbbvlc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2swnqctut.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yqlnfrqc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfledddg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmbvzm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ptjxkhpj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sdchipwp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zevijgpj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jxaeubgb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qawjcknj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zcmgkodc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2udfriedk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jhjvwpuu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zafiplsk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hhzewzkf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dtehcyww.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2lwphsmqr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2avuukoiv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2otkpxymt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrnycek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rwzcuhaa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kxocemti.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrftvtj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pstyutdb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kurfbqoi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wfpjkygk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lcbtovlk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2etoaaics.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2gnvnibzd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2otgccayc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gdkmoqmw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wwuirtzs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2sxydndtt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uykihwsn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fbzfhtcc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2brgjefce.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2arrwympv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmtexyn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nwiuunuq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yuwykmmm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnkqgwgv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rmcwcdut.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjzjwnd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2plfvisfk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mbtbmcyl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pzkwsrpy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjryvojc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2iaztpdfg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vavmmwsg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wozvndnb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2waihcnpn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yojwyaft.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2txdaxifx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rdfdqadp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xhnxgwbi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fliodivs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pgyeufih.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2edojvqor.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ulzqwrdy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zbeecxvm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hwsqgxcm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2macwccyb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfkaivx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rhoplhwi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lazrtqea.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ftwrdczz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fcosrrum.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xfjsellu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lbdfkgdk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ddbiacfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dfnnicpf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vkarexkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjajhuhf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fxgiaevv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2demktxrn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ghrfhsta.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fgoonaqt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2muvxoxsq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zjsedzwe.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ebswjgcg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dnfgudtv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcftasr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jzxqxblp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cisfsbso.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2oefgiecw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2usjfmarb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lbrhhllw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzsxdax.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bakpkril.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2aorzcjkb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqmtgriz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dyktevga.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bguzfxiq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mzzqcapk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2guwhdccg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ctsdoucj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sukkxyje.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xkamxzvu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hclvosoo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2nmukvtno.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2rdqcaeaa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2daffwzqn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2nztonbty.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ytgwload.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjokoghx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2khoovyhv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xxxkqxyg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2surgcyoi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wnaadwaj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2krzlrjwe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qtzkglqs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wmxyrcgh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aptazwda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jswddfip.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lcywrdwl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ctgmcdmz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uytxommt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbuzsgle.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dptbmlpt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xpvmnfkl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2paijbhau.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fiwvsrxt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ycjhfeqf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xmqlkohq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xnwtxhfh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hperfsxh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ctoccokl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mmsddtdo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uqiyetqx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ajfytcfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vagyvpib.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2clcvezvs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2elkfgdny.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qdfoijis.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jjzfxhnd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hiisvibu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ylvjpbyv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bvzcnmde.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2plnjewql.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yuzkdwlc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bvnkzosw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xnaeqncl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vqoeoycg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgkqreqp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlypabeh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2qrsjemxe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kjfzjkdf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gkmlllda.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yiattkgk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vodjynon.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xfiyoqof.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ejaxxofh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rcidmyhj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hipwtyna.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2plwkyvfw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qpcbfcpm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bxsbwnbf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mmkiumrh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvjbqno.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2afnhwggk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2odilsmss.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kevvqezr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wjbycsrm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2anqdyfyb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ipatbxjv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ytrvemxe.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2edipfbzk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2gqhljaxx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxyprn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bbxpydai.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gzsefocw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ikxsmnbj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lcwwmeiy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2weusmpoo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2irgvhecv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lmwzpmuh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sgmzsmoy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ygazjzcv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2buiheyai.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2agvwkcnx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qkamdict.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pbigezob.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2twjjrzob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aacxfzjz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pcwquoof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzbtlgtp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uslvituh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qvaavhzr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxskfbvr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mypxdbkn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2igbygpud.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sfrrjulp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tqovbbhs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2bwfugwif.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qcrhpsdh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mfmzwgsg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jrckxeql.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nubyyzwn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hpszhezu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gntjicgx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2olufqzak.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2vzjpvvlr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2biihnjls.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xdnsfhep.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zpjhkfmo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kvenipha.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2keyedves.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2svhhhgxb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qfqylkfd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hnvfhipr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vrvuifzu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2msnhnejt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xrrndlov.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vzckhdzp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kohneapl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2thdbhzgv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2skciziaq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ruqggmhf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rcdkodsu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nhnypkrx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zosiftgm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hpqrlxdq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kajecvrs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfgwtsq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2itbcwdsx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jxnwffsk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzfyxrb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2spjbvdfr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2nyrxvlmu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rknwmwwl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wugfokme.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2akfuygal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2omdkmwvo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2oplrbspl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nrqpwcdb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rcdcsumq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2idgvqsbu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2avaffshq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2cbgvsruv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yxgjpdlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xdijgoap.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2stqjrxhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuogfqwn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2aswsdnbz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2blmvhteo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2topglubu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lzcusica.html


<!-- 参考信息 -->