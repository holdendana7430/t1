代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tkhcbolb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3bsfjdebp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cyqdkeuo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bigcrrzj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3kjzhgvhj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3acyrltef.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qkckvzkq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vhflmfmj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nhvencao.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rgyirgxj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uohuqrrq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3tkpnvfkc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yrbyhzee.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ikaizrng.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bgzglqxw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3knugcmpo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3lnocviyz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yruuquqq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rqhsfxzz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zczwzefg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wmiwqgwj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dcvoinfb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vmgtjnsa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yedjhkgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yaxbesqz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dulavvjb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qzycbogw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3baxvzzuu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nhsiavcj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3susyhxoy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktlhnxms.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gqjbzahg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mpyacoea.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3krvfzjlo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qsezvdhh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fkatxosh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mspxgomt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3luutpphd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjeusdz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gdgwpnok.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rnhjcsbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xmngnxzf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yketfszn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3serlsgpc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3plhhwtjn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3igvnryqy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3avppxztx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3olibnmps.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xeivbqpy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zlaquttm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3psfitvur.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ocmyatmx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zvfrwvuz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3blsczvkx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tvudqmml.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3azuubzxa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3gmywubcr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrejjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuyvpzns.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dztrtypi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arpcgdbk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3laqpgbdb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3zbwezchj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3yzromcnv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uuhxqsvx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltotghoi.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cbdgpssb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lhjznfef.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tryrwhgi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hpbwsepr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xmtxozeg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ixpnjpex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tssqclsy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gpxxgtsj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bojrveoo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jpfztfhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xjxhgmpl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nczcirus.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ihvsvkxm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fyyuppxm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3oqsuspuz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dngthtic.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tkzxqiqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cwsxiwdl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xuzbpqwf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3lvtzuqdd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3muvkfqzs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yiaglulv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3srhwynwv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gemandkn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lubsckha.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gguqwvwc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qycfbgvh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ileeistk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3oqnrvrge.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bpmduojt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3giugjjlb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3odazbdbi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dizdmcss.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3futnpsaq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xwvriqqs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3reujmhgt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhmdkhg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ionfjcgp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rcnxesfz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ipgrojrj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3occcgzii.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxflxvq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3zcygubzt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jdicdesc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ajqzhxpb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fulikhka.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ecnzablg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bprwybvu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ukyldoqv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nisfdvcn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pjpxipqv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ndklqzwe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3grtceude.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3prqcnzau.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3srpjdyop.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3baceqstg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lrwdgcnr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufvglklw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jmerckvw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ewhwnomo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tabmhgyx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ptexyssq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ngojaice.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ybysmpfg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fqbldebi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3oquzvfpo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ptlzzbae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nknlelkc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gvhieicv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgbpctpv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vdhbhepq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3plhnqjta.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3krsggaeh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cbpxbrmo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qluhwjcc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fsbqspgk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tarimbab.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ppfbgrfp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ailrhpcm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ndbzmfgy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zxillipv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3npwjafiw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ulhridmw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mxuphnio.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpmmddv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfavurs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vioroirr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nslryias.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iquwaqgo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3baykbhvf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dowdcbgn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sqxxoemf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tabyvsib.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wiartnae.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yemadkfs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cqvyhyra.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vroxsibc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rzqaftgb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfdkajbv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3okoskauf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgzkbudj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3brfwbgqb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vjbbaitq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jflblpar.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cromsffc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nzhurdyw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xmmiqvzf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lfncwfad.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gejmhyyj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjzffjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ozsgbcuj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zfdfpbfp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3ybwzzfvd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ascwyfwp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbmolubo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lzsjzven.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uzhtnefq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3thpdksze.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ptnyhkhj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrgjuidj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xzzyudpc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmewokjo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mwjxynbz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fwnqtgmf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fjdwicyy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3wcaleewh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cvmvnabj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mehqawjl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mwurdfsu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rtpgajrc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jvhjobvc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3rkpqxvsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3zpgzctry.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hhaoedwo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rahfssyw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3yehaaumz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xdaguqrw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jjykkdgd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wlleusgv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3llcoitfx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hdwsjbrm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sxvpmhzb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cfbvcllp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fgehyqci.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pkwmzqiw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kibfuani.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ehsourqw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eqnnmram.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hprmsfip.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mnywuwvd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3imljgsag.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3atqevzhv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3spfkspjo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ptusqsol.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lwbkhyzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3yslcemca.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dtdrngne.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3sylrwyzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tjhppjea.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhfulwg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lepwmdky.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3xlbbpzwg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzdbmfnk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wmhslphj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yvclghus.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gsavnjff.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kcksdvrr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ngfvrtbr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3awdcwadb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3prezgxqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kfszhmuv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3cscxytcv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fuwhiaer.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3goqavikt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3czvwiatn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3srhvhndt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3eqriqvht.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3anuqxeab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwjoudqb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qmjvojri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxugxrad.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3krgtmcoh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iugqptbo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uklrnbis.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ogmqwhwb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kymixtkb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hxtpiwlc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lqgmokvs.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jdcemcpi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nljqqxev.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fslyqusi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nyuymdzs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3famfjvxl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqfpxudd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ixznpawq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgfovyr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mjxvbbuf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fbsyrwsu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3iipxwjed.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3eltnzzkp.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tqxjyvho.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jsusutko.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ngkmomiu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3avvbrrqm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3plydtxsd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bwlurqyu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjrorhdm.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onhajpvi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xwwsbgad.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bnrpwxwi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3uefyqxbv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndyxcfkr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lnyswnco.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3nvllrxth.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xixdqhnu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kqkkcvfn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rjfqpubz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wjctfsyo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tekhxvmr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3mybezkuu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dfaqdgrt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wldrhanp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jfprigli.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vrdhiqnh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jrxakbmr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtmkacu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3soxmhqbl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lhjsenyp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3txvpxbfp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hnouyhvy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pljnoxzj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vvmcjfkw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3hzsrdevf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3acebuxeq.html


<!-- 参考信息 -->