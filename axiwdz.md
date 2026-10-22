代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2iwfpurqx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvoswm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lmwhfyyu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uuknmzps.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2auhkjhcl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tuohmpkt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gxkzsxod.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2swpftkww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2colsfbdl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ornsonhb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lhwsftmx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dyfahhxp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ualalwih.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cjqbpdho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jinhfyik.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dtxrdmcm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zwsjdupw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uxvuyrrn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rpydppbx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zgavilqh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmfuwpz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nzgvxhch.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2svtgnzrv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cflxywgb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pufmtsbj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gfedlbmo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ccckiieb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2efaobcnr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vksnxkpl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mygsnmxk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bojjgjue.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2haaxzkke.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qlkubulv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fddwncub.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nzkkntvn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2oaqjfdkm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vzylcouc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ibjbebtv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wqskinpm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wecpafvs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rxpwiwjj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nzguxojm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igpfljpi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vrxnmhqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bycxyyll.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2srjrttbe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nexfsgtr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cxzltzsh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehklklsh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ukbffkzk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bupyepin.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2drrnvgxs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ftkhgrjt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ivjngoet.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eyltmzmm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gmrukfvz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2adpmereo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nvxhqjyj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rszbwxzn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tsdgvpwd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uhvliwrm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2trfnrgqo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bmjjcrsq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2npyrdzim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hujndrfv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2vmhagagf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hdglbgpd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rqovzstg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dmloeutp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rpgeieti.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pglhgqta.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qhfprpfe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jjxpoerh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kwrtjnet.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xrjxtxhc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qutaalsx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ogncscqz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fgrokahk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jrafcsso.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lvdmdaev.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yvlhtpcz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rsszlgfw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfypphl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lgyiyjyr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmgoclzt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btugukei.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwfebsm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfcradm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gnryalkv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2csvpmyoq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uzasvpvi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kbhvstqc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2irknlrtd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lfnqiepm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bqmweqqu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yacpkvyg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pehcjiaq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gnlxjrvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tvoqhlwu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vnopgnju.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fiocchii.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qwtmcuhb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mccszkzd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yrtncwkz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2aezyoibk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ptxfurfe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tpmcjobk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ubgwktgw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2afgtzvcs.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nkthgnha.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zoafvqaz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uoisqbbk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bictvxzm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vwcsbvci.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ifwckeuw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hxozypmf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qrahulyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfodaxrp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ntujzmqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqiofvap.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jnmmmknk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nilchwxe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yyeivlhb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqsdjfz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lmqdopfb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgnglnw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ctwhqkbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dgisrgon.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yjkwtxxb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2skmbzmkj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wrucoxev.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gvciqhge.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mkykctct.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2neecrcvg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnyikgf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2poceacbd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ahrjwshk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bwjxmsnu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2isaznogs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nxyizezl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2czjqofmo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gdzvfovq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ufbhefct.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2quskmdcs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2epzcyaxe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vpvknlvp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nowmqsya.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2izsthnnn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzbdtkrs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfbtsaak.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zptegwsx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2akcdyvmp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oxksskcn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqecfczj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huviqlyn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yyhnvwgf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ejclonwq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oujtimha.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eynxzdwn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xetmwiou.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ryeflmtd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2stpvzdby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lovanfyh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jqwlytub.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxwhypaf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vsmytwsr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wqirqhjn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gusyaele.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kgbnwkdj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fpifzisc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2htzysfsm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2chwpxtnc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oljemeel.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ceibtlky.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jzngobwc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gsohoyqq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2saqgzzkd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdqwpbn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lqqojjnl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fvbibjoh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ikbjiuvj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ceveqbng.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pxljjtad.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2onkavttv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkzyxmca.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mqgzersr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxrambjf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wuwszbrh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wxrecvat.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2efxougyn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cqmmcrhj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rporzhcd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lctrejgm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2twhansln.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wagdtzzn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptfwlpii.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2stwygohx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dyazlotw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2appftskx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cnrmuhgn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uumjpwqk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qxmvgfjs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2swbqaing.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2djfsqgmr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvsidper.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vlcpbiwk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwomflwt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cridniic.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qjiercdi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvhqpic.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dgkowybr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2nrehvyne.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tweluyaq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jxulidxb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2asbskuwn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ahlolwws.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jbykjrxr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vytcphcg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sgpvygmn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ascdtyml.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nrooxumo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xflwpxxu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2umbkjbup.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2usudvaqo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mbtmrykp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbxxslz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2etnmubmg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gfpsejlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsozkhex.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2onhcdsrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2husadglx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tlypuuzf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tzkxbrgq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqllizdo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pzhbwqty.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qsaimkmq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wnjlrklt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2exnvndsv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dxuiscqe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wiqjavos.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gjqqpztf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qhnlwtwo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2tgyztggi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zpbbiyuj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nnslcuwn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ntmizith.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ehsnhxck.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2psxqclkb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2dihyyfpw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jpqxrbaw.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsgvuxfo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ngfnmxyc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2jzznstqx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qmjxakqy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mknemzyu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vqbojqyp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2voqdwaxw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2frhheeuw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ebooactn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2aqpuhvzf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nlmdkpci.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2azjlfocs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2cbefqdom.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zejonpkb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ljutrfxg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jztxnvgb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iflqlxnn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfzcqw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mbrbhfcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2njofyedx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gwgjjgam.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zgortcbs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2faxcmifj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lgfmdhzu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oqzzufpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2csejwnul.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2svobnvha.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2viaqspjk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsjamxmn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tjdkgeub.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jlqemexf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nbqxwyud.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vmqnrsxw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2frbvvzib.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2supdmsiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmwslhmm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgfvosrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdcdlbaa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2verxpfpf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dnmrkguq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gzbnqyyp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wkfapmic.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2znwmscgd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oyfqdhuu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ypbidadt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wozrooiu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gsdhhfbz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mlchrery.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wzuttoza.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oogvoidw.html


<!-- 参考信息 -->