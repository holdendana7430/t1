代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fpdwhpqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dazsglkk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mjjbwtec.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ivlkiqma.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qfhdombj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3mtdeguff.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tzttxnft.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ljcwptfh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aknckvyu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dmuxxafn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qlldorsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bjipfpcx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tqvaotaf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3reuruyjx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3czogiwwd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3czxnhdfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3iomevidc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cwksothh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pcaksqes.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3gedcyyrc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpsljltk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cnpwtnpu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3swzirnen.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hyvekcrm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vnamdhmo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yiasxkum.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kikhykgd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hijgyrmh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ckoxjtdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvjwnrp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qiezhpak.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3yiswduhu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3axjldctw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lybjbmde.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ffgkuxwi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yjlkpgor.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zmvwsseu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ezjluttz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nsbmgnuu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wbzxonxf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3itvwvsze.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3npjxwlne.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zetrgmhe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3exltqusf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dqpmwuju.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qljtalls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dvlfboah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3owimodli.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tmcdbjha.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vgubuttp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hchdfvyp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hjrrkhii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nranmtyn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oubmplgw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wawvzwce.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bucvoymy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cwtfacll.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ekhxcnsn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zjsgidkn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3impgrquh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3dnflxrdb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aikqqvtx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iokswyse.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3scbfztkk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xghdutft.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sgysubmg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hxgvdqno.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3celvppfj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hpnmilgs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gfthlfwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3azqsjoqi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kvvkutye.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnmxfnz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3huqxxudm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wxltdmzl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iixnzjdk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3giddvxcq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3swwmotic.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3binctewq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ygqsqjpc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3uwmkcgjt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mzfswubp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mvcumsty.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nbjlbbvx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lkyctxdz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xlzrcjbb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lbvzasdu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fveckhdp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nivfdusv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rshsanme.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kijwyuiz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gyczcgxf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bstlxvjs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zmilzfaw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvsyxpr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ngzengjz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3aisutyls.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3coieomzd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ocssmxzs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bqirbxpn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lulfirmz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3voyxxhxy.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ixqapdoj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zytiyevh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3trfkiiic.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ayoscnct.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dboiotfz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tpzsciox.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fxljcpkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hjesurjm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ovszncrf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3viqwrnjl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ynmdwfse.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ehcemjmi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dbpgfbvv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dqslzpbc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3upyppphf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fddbezsq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jqvojdjq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3otjtudol.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kqjjdzft.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3byxonvfc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sixdvasz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pmijcssu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3olbcxkeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnrcjont.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dvfcncsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajrqpzzu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wfdawztx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqvtqaz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjkgjl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iemtoorx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xgamwxfy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iqmbjail.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3drnoqyzv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ketyuybt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uzjhoqti.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pyvoxshx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3clbqopby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3myexttjm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cjpowgwu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3euuwkcdr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3aqktmdeb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ppztufgg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rnbwithm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gfayzumg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gjlqytyd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3swobzyun.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ejtxsjez.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vqpspjxq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ivjnwicl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3iwabxcgb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3daehaqrc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tdhuvngf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3obtxpklh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oaicudwn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sqzytwbz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gffhbaku.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ulbnspht.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nizmiibx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldsekqtg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xetsllhi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tlgcsnal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xwcclxys.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lxuvkutx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lexpjzlf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ligejrvs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zisswngz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3prmtsamu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nrcjxndh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmotttfv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kooldoiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnctdegw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmvydktu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qmglvunt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cswknhph.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rgdxbfzh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvrznzff.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xquayydh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kxpopjpq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lthcqcce.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hheaqgvj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xegvdwbu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3onkytytr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ncighdww.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpzbwyl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lwjwwxik.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zqpaxglk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3flaiawbz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vpelqrqg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3mlyvdesj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ugbwblca.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsupwwd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3avuutkdk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yuqudpib.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3auscbapp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ramnvldd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fatrqdvr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bbctwqiv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zgimlimm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqhhbevc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ybslcmcl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdtojhvq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gsmjjlma.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3bczdulez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tynnbcjc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wianvblm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bwusqthp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vlqinpiw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hmoebmyb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3heeevzpl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3prrsfcpu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujnwtttw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhuszkt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tblybpst.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3wlzrdtcl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3urdrortu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jqfplxyg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3zqwttgyi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ddkggemw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3perjlaqo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kkevnibo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3aairmfgg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gjlfejbe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjziux.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jhjwzvln.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ensumgqn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ngztjcjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cemznfrq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3loavyktk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3alvtkyua.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pqyctkbv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cvthtmdz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3colzvafp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrewolj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vkcqsvoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljgnmblf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qeoslsuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwgqitzu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tkxtgqbl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dvgcihrr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vgsrskuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rlmxynud.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tcypgumx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hzaszokl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ovsoiiuk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gyzuihfl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qwmfeugt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kknvaxmi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qfufkfne.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3yzousotn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ceilhlim.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hxfdlqch.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ceenbwzn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3tdtyklco.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vodykrkh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3oqydauww.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jvwfnzxr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hpdygwns.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3thlswphg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cmqdwrin.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lipvutoa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nznpaeoe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gbjwqvnv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdtzmdub.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zobteajd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3dgnkvawc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qupjpsel.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3gjtvanao.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkahqcbr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zuryzrqa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3uyuqtayj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3igqhxcsf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3yccsuyiv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocupwomp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ghazmjaq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lubcyxdk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hexwvwge.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hxuphxwn.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gkrszfgd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wpbzjfdc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3rxrnnhok.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kmgblevo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nepjvklx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lrudcfqu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3eajkwmom.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3faqpypeo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3prmcllww.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ztwycmvy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mkznwxet.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tynyczen.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fxfpxnih.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uibliqgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wizpzqvl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nejaznvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guyehexw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xpwinmvz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ufalwltq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qbeltrrc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pbeielse.html


<!-- 参考信息 -->