代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dtdoyfaa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3unxlkiru.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qflguetn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gdwgxzcv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3jegrellx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bhguqgrb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3canibhqb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hejnskde.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zknwlulx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hppnnfnm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3imdansvz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zviojmnw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nsklpayg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lxxmiydz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qcpzcpgi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nnckzhmb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3znxjxios.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mluiafan.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oxioqkmj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mqdmqfbd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zcmgyjdf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3neyaesrs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yahmsptn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xososezp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qumkucmb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqurui.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yktalewh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlhhyut.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iqtjehsu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3psoxeizh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3aolnvhbx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lfmutyah.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xsfchmbm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cltgjfch.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kowgnslc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nyrogsgc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3snnuvdpd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qhatavfa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cqcigcqm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3yllytktz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3saldpqri.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3chqefcfa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3leqwmbln.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zkqcgyxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3egosfboo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nqyihgfp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3nwjksljo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ibjcxtpg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xcsberuz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3smaqgbaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fatjcvby.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oxqixbwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtwuhtop.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3slfgvpjh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mkrcmbuw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3awrdsqqz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3utgammwj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ssuwubgx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dgpzzpei.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3duxsphxo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vwoejlvt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wxirjmxc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3cedfejuh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tqxoxrdj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zfgtxqmr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nzrwfozf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3medqxlpu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rezskiib.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qugucmtg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vwrajzem.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ejjloomx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3efwuwlhz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3yughbuoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3epdqinhq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vihbzzfb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mtphkqsg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rgroycze.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ygkcevwg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eavjojgu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ulpcgeyt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dcmhhypf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3noktdkrf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3uwxkdwte.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kpxapoiq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xqmdccys.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ocvptlcw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ofbhbvtd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ckprshsd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wkvcuepc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3toxnazqs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tmppgyjo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3demfwvyw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dgzsgscv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yuoavqkq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uqdhepwz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dahoxzlw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dxuaxitm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ehtybjqr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jbvweble.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tiyeizyf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mdnllule.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sehovinp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gaydrofi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkrlrbn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzgiwn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pvsmzgdp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lgqtabfg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hyvbtcuh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3uatcemen.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3czxhsdpj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bmtdrixt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ecnytkxd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rvyutmzy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uiaofvxt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pqjicvlk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bgmtzzyj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mbcpozfo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bwlnrsak.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ojgtnvqz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tmxxpakb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mlbwlrrh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dghlkzgd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uemckrff.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nhmuejqu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3snslqemb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3carlenuk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3eestsmuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmcsygzj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fgrlnjmo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsrojdho.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rjupfyez.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rmjqtwai.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yujfnmyj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrwsooee.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3anqtgviq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eetumscq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbsaeip.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3aytatmzd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3phyykmkf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3akjnforb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cvvuuhtr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sotgydzl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hqbluwoj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdkhgblj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gceknawe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jdbxqlww.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zlyhwahm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bzdwrfbh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3bfchewsn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3thbjklfu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rjgrenqj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rwpcgbhv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ynkrwqkn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bqcpwdgm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vmiuszjs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ojjbcnhm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qjynluep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsqyzuff.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bggkfxgi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tvlcaxxl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3enjmhafh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3dcechheu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3miozdbcj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3przqicfn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xtmhnumf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzicmtvx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ggzyxcfu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wovpetng.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rbpjwsnv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3acdrzgtk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnihvew.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3njylamsi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xshtcyej.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vfdraudw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wklhgaig.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxtomfqc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjgbxtd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xmjcapnm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3clmuomwf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vjlntvtw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwjhgtaf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kfgrroih.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ibczjoso.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zjagqrtx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dzlmhzbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jeguduph.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zdslkqix.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mwlsnevi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3lbvaaaee.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ycxcwsdd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ltqzyemf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sqiduuhi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dahfurvo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wjvgwriv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3efhvqgtk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dmapvtza.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3knafgmwf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iejaeqfx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3aabyzewd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dnojyysj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dndipjeq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ayhcdrqh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lkzidrnx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3msedegcp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lvpapesa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqnwccsl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ncnfcrzu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3txkqqixm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gfxvhjqx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3denmmsyk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kjyeduam.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjrfiad.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3txifufku.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3aybjpusc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zchwbhhg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3plnqbhjw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3fhrwqjxe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ahsdpcow.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3inlxretc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3jrbvpwmg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xalgbehn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3iomgjhht.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ivonpasv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3arjjwkuq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gzvvmahx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dzzszazl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qixwpuuk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kkocajsv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3krwqwqwk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mrlzdmqi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jurwdbgs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hpcrkoxi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cixdxwzx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfmhmfb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3joachovz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jpyretcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpdwuppl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pxfthdwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyegfczg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vwgsnmaw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ppgncmkd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ivazibyl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kortbnum.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sdpcynzh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rvzxsyqz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kuvgdkff.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vvkysyzd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ddyfnqdi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ldwtghqq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjlgzuj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3amvmiwpi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3nmvohrac.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kytnhxwl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3izcnjzfi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gzcfflta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cirblwul.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sjjsuxgk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gsmjconp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wdfbpsrk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ewskuhtl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3czttkprm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3emocmgrj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdqzoteu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvkficp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nnoplhcl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bqqbykiu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rqpmhjqi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jnxnvcjs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3sumqmjrx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vzhoydmh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vjfuemdf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ytvyulwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ozxlrigq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3trnwahzr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tzwxthwx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3fanxkmcc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xobfkvbv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qjdzuxke.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kapstetx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xtollgpn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3axdrrfff.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3newlpxza.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3sgbgmvwo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cijsobdy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yxzmfjfb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zbdkowix.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kthdjqal.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pvixqjdf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tbnuyias.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cuenocnq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ycjetupb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ikbdhwmy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzfpqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbyaavnc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3lhgwskzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twfxjvab.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vzyxysog.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jkornaoh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrdbij.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fzqfzbuk.html


<!-- 参考信息 -->