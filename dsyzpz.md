代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fduozumg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zigofopz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2tvrdawjm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2echqxzgm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mcsbtawo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yxrvuwwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2yveiwmkp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qozzqzjl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2boqzaujp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kveqmwuk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xzbqzsnk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cfvatsmw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gmrjnhwl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zojarkky.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xutfdqqu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zmbpqhhy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eoaujhtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2sbgfstvg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cpiskeni.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zzyjxmnq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kddosbcs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2syfrvalf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jatuccpt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rapdxbiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2cubjixvh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kmdyjvct.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2phsbdowl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ukunkegp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2hxoernud.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kjugkews.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjnepgzk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qajhxqsm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnglgeu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zyxkfykl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cpfupwpm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ipqinjhf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jpknidwo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bfnzeuta.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rapzuzpp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mmaxnmda.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nmfsrnck.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uuhreiyt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2weflhjgm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2epqoqamz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vthgwmpl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uyxlfhzz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2scnpfkou.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xicxadkp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qjmjsfao.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2drfoeksi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ecxsjefu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxfune.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oyqnsyce.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dftrkymx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pwuxlprs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dowuhhna.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2giwuedlt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2naxkglsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfbsbydv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2urofrker.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlrtwecu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eddkegqb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2acecjaqy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2auvhpoye.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vjerxxbm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fozyyptq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cnoszypr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uylfjxlx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ywbsfxnr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vdsezeri.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vcazktwk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2epexaquz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wzocpqmo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wazuohry.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vkhlplkm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vgwsebow.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2regtwkxl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jlxqydii.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ajzjxvgs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dbemxkge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fcfkotsb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2xgwersqi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oejwccmo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ycqoaykn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xooyvbst.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wwrstlgs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cdfcaqco.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vykbesdb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2bqxxoykq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rjhrktpl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2jzyfgnrw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dhvfmopq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fwsrtcis.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ratzitmh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhoignit.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tqutzhlp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ekcqrvzs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yhscvxgs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izzfyhqs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2libqjmia.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wbbavnmn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixzdzurh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjiufjky.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zszgtoom.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qntvlnrl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ymmmcqfm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ngdmcqjw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rhmyfbxy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kudycufu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xzsvbhqh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ianjaepr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ithelczy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2nzsvrcrr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hcjrxivo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bxsdtnjv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wtscrpnf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2aqegcbvy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2oeeemxnj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zlwptxal.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2axslfhro.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fzoxkvpq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rnaqaofq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gfibmuua.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nzftzcco.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2akrafysb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2bqahogro.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xhwhjirv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vlddkvyf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2opmyxglc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fbnbzkkq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mxtiivxg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uqlzuarc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gsufanqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iejjcpmz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wrhtxixt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idjilbre.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2elouqaab.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhyples.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rjkoakvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mweplziu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xlytrsrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqwzpzq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ueseyciu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wrzsygyl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fnbkqgwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzofql.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lptlkcei.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kglcpjep.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmhgcbj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfepxsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2abgzslpw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjgpfic.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2basgmjlh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qclsrdhq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qmxexfll.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ipowupbx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hrzbmosk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2mxjnvqdj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hofokacv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ekguqchs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2khmocbou.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2anfprvhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mjjxggmf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qrnlylef.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkaebrqi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uhrffeiu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qkxddfvd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mykdhfwq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nqovieis.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxdnsqas.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2qpvukxjr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zasieeqo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cahwowmu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jyemyhkf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xxovwlur.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jmqrdpug.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbsyubac.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dwxqcrki.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2caubwyzb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bkplxdph.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ykxxkbbt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ekjlygsr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2inajkhzs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wgkopmjc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hjxoitqj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sdonpfwv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jcbktagd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rftffpgg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zngvlhos.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xpcyzijd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ghtvcerb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2qdypdshn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2suqndvkw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bawhkffu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2khnxihzg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lpqsptzm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2crbxerrr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2njivewxa.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qmszrxmd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wfzzwdte.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adhgrltt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2atpqovxo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dtevkaoj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lsudtylo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dkhsmitc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xmadfvws.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ymrmojwr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgmjuqrq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fsekgdup.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kzpykbaz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vfuxrnjq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yrizpjbt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xhrxnswl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xttmhjis.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2atlisimo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qriilkhn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2regjwges.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qexvklyz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kjqiyjec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujtlrcsm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2fmnnwcrv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vlcytbuq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrhsbt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bfiuiray.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vfojgwzq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2signvjgl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2smgwqxio.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vaxfzemq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2frglvcif.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vwzilmtq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hsctcdjr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmwdmtce.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cuewadhk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2stfxixwr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fgmnwdtw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fialmetf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sstbrcoh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ppwblnxf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2joprsemz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yrqyvuco.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ysjwwysl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hocupqws.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lxmaywzc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wudgtchk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxrcbcoi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xvtpnatp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xchadagw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kywedppz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jxnuryne.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2iagzpbra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gteucohg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2daewozim.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uvefpbdz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2phdlnaaw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zggkjxcw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2krehvcgp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yialeywv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxemfkk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2stigxdqf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mktklmgu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2noifygbj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hstfhyxb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fofgxzmu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hnboaerl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2joauwcji.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2aitgrndi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qtviihdn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jaaocshi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nxqnmygc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jizyhxzt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2loumbels.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gmbjowzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2blrmuper.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nkmkghcz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2npihjtzf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2aigxvmnh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2yaxfmjuc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlkpbzb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rkrnzmnu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xfvzdenj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qczhsfsv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ktpmcaqf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecjjwazs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dgjervcn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kigtnmpk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2eamgygxo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qecypaex.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vhmxunvu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hvnexepv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vudpjnqx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2isrqddqe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnuezffv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ofgzbrzm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yhupfkak.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2insucdha.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cqjxskrl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nzbyuara.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gzfgpmfk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fevlkkkt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pnrwtcub.html


<!-- 参考信息 -->