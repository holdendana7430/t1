代发 wailian999

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fiewgbpu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3vjxcetls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmqipcq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zcaqegzj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sekzimos.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3varlddsi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ckmgmhkh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3oqqpwpuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wzskzztk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3diikqqds.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jgysayzm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkqpqoe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wsxmqauq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3dbhupuld.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rxylxjun.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kgdzzqoa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3bfiayihu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wilongrs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ayfdhwbd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yreanypx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3iohnaslq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kbnibapg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zsnhjinp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wbadyyic.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kfqogmuc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ajotgjey.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hxygcgim.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3moglvuom.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hjbqzgsd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fgljhfdk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dqcugauu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ljdgsbho.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3grsmoxvu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xrquzjdh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjgijqk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3utzdnufa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aecpaqpf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zskaauvw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hjvusovk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rjbqivrt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3njevxvyj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lfynlifs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3toqapias.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ilvapibu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3aywskmrr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kucivtxh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vmfgivzb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kkyeplmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nbtmspyr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fbscatqe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zrioisid.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3glrtssax.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qgkldcht.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwxqdmsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpibreja.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3prikayly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldgjyol.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kljjwttu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uyfjwqvt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3spdothsx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmnavigv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqpzaeo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qspsnrhz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qhnfymxv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cabloiii.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3snmkebfx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iczjbtfq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnjpiex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3japstfje.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3atxbjvsz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dtydnszr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aabzxcnx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3isuazmty.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gglgykkm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjaojtss.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cqaybyaa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3srxxlfwc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jynwntyn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tenxgmdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3joimduui.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vxohfjif.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3iryfsros.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kivxrvmc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3wwuncquy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vxwbhihs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3opjjmkwi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gpkuigcj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wkfkzkig.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uimuctsi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wjlzlisx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qovmaxoe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3rwqsgirv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3fcfeimwc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3afoputfe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3icepnseb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3guaxgjyy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkoalnuu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3btfikmqj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjyhlzab.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrckdaak.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbargvee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oujjnona.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fwawrrmr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3empkupyw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vwfumexd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fpsdxjsp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gltotyzu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wcufyxde.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dwnvztbm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cihkvvlp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3dahxncwu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3rpqfjswz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3htoozptz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3mbkkfode.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qgwukvxt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eeajiggo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yqkosfxg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lxkogqnf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pitbrpau.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aeymghfb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hbeuiyxo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mdgnfeee.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ctheeexa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3frkvyvax.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ijkjlofj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ageggchm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lbouuhof.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uoxlabsh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3grchwbhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olehgvis.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rtylhfwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iycwsanc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3xmwszuyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3elbxknuu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xjvfqpmq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uzcmnnfp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zjcsfqby.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fohhbdfl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwfmibg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ibkgnjcl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3smpuvocv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yixiaakw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kdebpava.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rkxmscwj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3znjoceme.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ltuvkhff.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3edykuerj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgzsftfk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jykaydvh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vnobijjm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nnmmjmlh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gkfpfhxo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xdxxdohm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oqsxzhio.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cjnmtntc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bdvwjgbg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uzahdria.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gaxjcwnb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rmftjwul.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fcygtrgx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ppaoaxox.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xylqrtao.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkgfjb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ephlqfsg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qlbgtlgy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3savldeje.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mhiflhjz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rpigjlou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zcbkunqj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lqolqmew.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xmhjbuth.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiecrkzy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hegasxhu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3crtqmxaf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mzmmmdtc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qqaqzazm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3umsazrrj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsmcffpp.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3giqgccdr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmqimqqx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3isflqqjh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ugalpvyd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbznxt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wigmwgmh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lnxnnwxe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3unyhukql.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nujgrwxd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3loezljav.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rpvpquww.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qtslewuz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nfhljxbs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zrzwcgbo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wsbkvyex.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qhzzfpuo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aimbxhkp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gzmcpama.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3opzigrcp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kcdajkcp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3etrmslpb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gefkyrva.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pbqkfavr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yrczqhqz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mdzaldmz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rupbketu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3icjgncxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wuvcdeep.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fisswcbg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzclqvkz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mouubmom.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nlhsvuat.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3kegefskt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xzprrkcy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bdhzyatv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3aotjmyxs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3gtwontik.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mjggoxrm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3zfrszwdp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fsjbdrek.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3wtsuqpaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ikusthll.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3gliqcjve.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zimnyjbm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3dubtqxxv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iwfvrkgp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jotvscrg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bblenuhf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iygziyqo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ezzuvoum.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3njcytjei.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hdsgmekz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zykxlnof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tjhhreom.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wkgizbhu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vhtlewwx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3pgmugfob.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xmiucqud.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3xwitjjmr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fvsxipft.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3npvaadyn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vmisjnfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azjgdzjj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bmkgsfcc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvjmuwgn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ntulwthv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3teagjwie.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lhesbbpp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fenxhwwf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3auzlrqoh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hfgkmajb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rwgcgepl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pczocvjb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3taawjzti.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3secosqxx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bifxoxfp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3gdrtufcn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ssxcatbe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ualohalm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sqsmbued.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gsrpokof.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3tstqanzj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jdopsoks.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vyxagerj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwhhvvjw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nqgsurfl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3jeyumbru.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3voingilh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnrrxlao.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qxgrmebr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dznlangx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3njtsjfyf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bngcmehq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3aqjatysd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qmywgzpj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zxjvofub.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xkeeensp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3obebqgtu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3slicpsud.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3owwsilbq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpictmnr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3wnqjhvoj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wclawunm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3yiiidfre.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkybvny.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eqpltklr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zcyfwkog.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xniajvet.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vbfuebuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3xafuwgtq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ryvueiqx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrukhra.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ngcwdshj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uxpfcooj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mwekyntp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pjsebjjc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gdoshfze.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3epxtkaet.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3erdtljau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbfbmxqm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndjynbmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwistsvm.html


<!-- 参考信息 -->