代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zrqqpccx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nnaueuvi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uockxtdn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wxffqlnl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ekgugnhz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qnonosqg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pfnekapt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hbuaebep.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2memerafs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hafwaanz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fisnohcs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hbdrytja.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gmejrumj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pwfyhyst.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rtkeyzeb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ylqtlmdo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfitutug.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2yvkgjdqs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2llwoatil.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2frhmyjvc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fvjhmcyl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fxyypbuk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zmxyqsjx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2afaxtpny.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rgggkdsl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yxevuyca.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hepufvli.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wbsylpkd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ywtubasx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfhacsn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2dethnvfy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jfswscoq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xomcvbml.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2raoufwhx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sjyvsmcj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ympwkhyp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rxjllcpv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wupfcosf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ayembjhz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2skmnuzlr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lfludaox.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eexivdjs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2egnzwyfl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2ntovdwco.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dygqkeii.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hdcvkuof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ctifrcai.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2brzgwyvt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zcmuujco.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ssgzqrjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jredavug.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ihqdupbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mefxlbbv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oldxikwv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kliweguv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ukyektub.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2giadzzzj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgmpdbu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqefjl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rsxhfyfk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kozrauxy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gutjbcrh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dcvfsanl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cmubrhqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bobvzxva.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qfeobwrg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bjwoonjt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2warrbyno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xlbjlywq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qjcalies.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yezbkeer.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2mtlqmkno.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2idyixdvq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xraigfrv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sgoztrwb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2prmhfkga.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kqjlukoq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ervojpge.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kxadxovc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogweadpo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hhhelvox.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bhokxfjb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2sihikosz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nnxymifs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2frbqszqc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2trwmdypr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dfjaqfrh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2crmwjjzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lzjqjodq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xzpklepn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuciylqx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2atkhgyta.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvrkjxa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2djfutiyj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpiutjf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oikrdxcz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntzvcaia.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2owhudmwu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jbuwidqm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgwtmtfx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xaiiqkhv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iprnkfui.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zfctpwgi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mayxzidx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrqmiy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cijelbmv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qgbbjxoz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kgeckkjv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jjmdjvqb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ibylqvyk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2neufxdcq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kupncfcs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xudozjco.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nushavpi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ctuqijjp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jxnbhypa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lvxdwxbg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kimvqqmc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ehzkblow.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ozfbbtuk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rawjpqvj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ekmxqsse.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dyodgtgk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xqxissrb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2bdutdbrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iovqpbyn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rjetkpzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcgjsspo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fkxfvjmz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2esftiexu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xitgqnxw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2utzunqfz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2slyoqzdd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwochdmw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjsrtra.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cezpvfzh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2crmalaur.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bfeeehlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rkdqoywz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rfcdutip.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kaabiild.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ayzfhfzs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ffkdcyhk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrhrsrly.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2msnzqakm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jaduzyge.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2indlbokz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zaowqcyt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2uykzldzm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ktynpzhj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2djsobjux.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zddoztnx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2swxgpnmk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eeciaokg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2hgjfkwoa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2altmdehq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hudmglic.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2chszopgr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqakcwjd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xaevxpxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2immhwagc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2cxobjoch.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sejgdynj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhiwgpxj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2simxvbhc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vrpiuits.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oastkwoc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2karzmwyg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwzysrzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oazsbymq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2seicgxyf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2byojghvk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zpsgylpf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wgcccxyd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lpyszgmz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2flsxffut.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vcyvashm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uroqkblx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rwhmwsyk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iiolaahu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqrjig.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hlanxeyg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ortfsofy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xcchhwtx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iepocfjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2aebvurrw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2stoteqdx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bmyxmsnf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2dufhafxq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gyvrgbkw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2bhnjjazs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pbzexioc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tyudgbuv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uicgfunw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zerigslf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hxtmaike.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lgbppjsn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bjbnytla.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mibemsnb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xmavrfjs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2webignrm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jdgxggol.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fwoxkxgv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rnqxltog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gttxctgx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2thebbild.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hkwxibbi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptgzkxbm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dufcnapu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qieprgpz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bnroecfu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovsxcxxv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ivptvkaw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2prnozzci.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2umkdmbmq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2plfinrks.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tqvfgoht.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ymodeloq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2joifvdll.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2poohlafi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qluuktia.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gpnuievl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wtubfhyl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lpsnkgpf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kvhqrbwg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ouiqawwj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pcsgujvc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2caggzjkp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oqhbwhoi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yhpugqob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2azrvpbal.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lzhevghq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgmemk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qhrtbnvs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fktdfkwl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ahtqdnrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfqxgrqe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hqwqnhsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yffbthkz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ofwckmyp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gkrnssyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2eqioqkzk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2krhugxim.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hzofvhlk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cdotnbzp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2eljszwmo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dmuggikb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rqoxgskr.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zxtcwvaa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2exjbkyap.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ffqiikac.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wltarvdt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2frwzkugl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrtjiek.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rmnyvupt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2sythzyis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bdxciutv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uqrtwahe.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lsbllzyc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2tjbsajer.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vbmghyyk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nxxzsxze.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nsucuobc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tksllyxb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2iaxpelij.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kjplfqdo.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2nsicwcvv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2iatpnupl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2errkfvde.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2disjdwsx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkkkgbil.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2evsfcxpw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2krohxqlk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zywjbhzu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nedpukoz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2tgbuwphr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zegzwxyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cwhgprly.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzdbsd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2utogpwvr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2eqlschfk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2paffeepw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cuitango.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2wgmclzgv.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dszqkttg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2jumgqxre.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rkmffrfa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qzivhxet.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsmedj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2pwcchnbj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2xyzmobzo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bpzrplol.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vqccrbly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyfdqtgy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxrcllzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chpvmuje.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vdrottnb.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2mnhdfasn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2roypluho.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wafurgti.html


<!-- 参考信息 -->