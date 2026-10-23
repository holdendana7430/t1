代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kmpausdi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3mdmmfhhy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3csaezjvc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3katvqyud.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vyzsixne.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ffogccjq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gukcujtz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gwyegdkr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kkyxkjgk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fvmqaupr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnfdkqg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yijinlrc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yhxhjycu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3zxdcqudm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvalctx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpmwldg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sxpdbkjo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lcvnmnnx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dzhbgeuw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3asujguyk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vodpelpg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zgaxgkfj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3xgweeukr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3morwexrz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wkchuzgf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3imuajupu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ncdctyoa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ylriiudk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3demmespy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nejeqvrj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3euugzsxa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3yqyavrsx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yoakybgb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3giymieip.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rnphihpa.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krxqfrlo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wgddgqhh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhxvxtz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3gllrflfs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bshatyge.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ggfbhxci.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ciwalizl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3awbyuwwq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mnytwtmz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rqhiqsyp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3whhtvyhy.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qmpniirq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vtgehglt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3couwxasi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3igcaxuau.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kwncekkt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rnlcixac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ldhnxstr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwzllvoq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fvlsrvdg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3nqxyxzpt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqgwnqv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vcdapwgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olzfwerz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3skigicjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjrnoome.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3abuasglb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pqysrlat.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tuwwwfsi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qrlidcnq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yokdjczc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jnymfani.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3shzlypus.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3wrujdhbw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3meujklhc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3emnppxgm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tpetkrqy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3srewyrof.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ygcqagkr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mwebrbns.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zvglzpkg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iwqtckhi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bpvocbuc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hdquvgvq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hufwdebr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3jyzyxxic.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3euehexzl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3blxxkdmy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3khogespx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wnitgtbz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hjnvzviw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lnmwezmm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vaapgoot.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gyqctuxk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3drzvblyk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hxninafi.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gxtowxmw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3alqjrami.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zjfwahka.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3malbbham.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jowypcbf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mbrmbolo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dwisawlp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuoopbfa.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hztszfxv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbqilcx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tjruoxtc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhjffjq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gocfybfc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbhyzwbh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3efargxxv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3owwrugec.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3keuaexwo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tvkdudip.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vpjpdgzf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lkyxpvum.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wxgzwvqr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nrhidbjc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kldplcoz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xvbznxnb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sdbfzrqv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ccnglgoy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dptckqsc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bpyrwjnb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iailgsot.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oeeorsqm.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xxdplzjr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3efjkzpwg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wehqtein.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gaqnrcio.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nnyhleca.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mfedxdsz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dwlmajor.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mouthpdg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ljzvmnwm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xyabedba.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3avabfccf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kvdewpxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lorhxqtj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kdmlfzrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuvywbnc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ugqrpxad.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ewafgtzc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gcokkllc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wczdhjxd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sklksxgo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhqofij.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zflhcrff.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kusevenx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3btuclgmp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tdcaczyu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vfynyhaj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3totfgjoa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wdeclqle.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvyzdmk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uasuoxrj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrjpaxs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3crwveick.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3efmmohli.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zznacegp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ziwngush.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3nxaiztze.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mfyaoalm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zahbozoy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3megqjgtl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3bgydydfi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ttjbqazr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lpjljxgd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3lrqlqiwd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfoiwxoc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sacomqgb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tiipsvso.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3farhkcww.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rdtjwtlm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xomxoyhh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bemirvat.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iuvytgbg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xjmxmskt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3juzhsmzz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sbaicpzm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cncrlcug.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gbkhbcvf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rfckrpgy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3booruatx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xnmawwyw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiutcnnv.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3scrbwyww.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3eewmkldp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkwopfbk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fxxhckug.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pjtrcyuj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ufcgmlzt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hgvmonfp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jdfvegdj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yurpjnus.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3albfpkya.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3eevxapde.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3btsxxrnt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ahpzorvu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lflktihk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sqrmukar.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rfmqaryx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fexcedct.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3febikjmw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nxvageam.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3izchiptz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mpksgeul.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gvcwrzun.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pahttuqc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijpsbknd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tkgdxezw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xfdisxeq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gfoetuox.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qnesxlvm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpxdkfqw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xoqsodhm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sajpxrzq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yhjnyuxz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xustslup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jawtgrip.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dokgacbo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xybkhqnj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fahdbdjf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3icpwxptt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymprxwhz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnsnzxjf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3opbzhtra.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hywexiec.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bewnpmji.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfcnqya.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jmsglffr.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ivtjrhhh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rtefuabc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fxaocvlp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wtizfmai.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ggiustzc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3talngorm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dqwgdonw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3jcdxuvwv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lvhzedhl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3exfygija.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hykvvxid.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qyqbzzgy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vugbuabz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bnfugyst.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vfwgvluf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3epglhgrh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3izgrvmjm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xzbxbrgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrsehgwf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3otodstgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhdkhgsd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3difcnqvb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ywydbsdq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnrpzfyh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3umohuhcr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3umyfpbsp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tddvbgrp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3reychjmi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3zsnpkwds.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3lezhbrep.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cavvyyqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3fjfjbdup.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nvgldcgl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3utbinnqk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vtlemctx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dsablkqu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fbuinlxw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3syaihxod.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qsfktwhp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dalahclh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tdddzlen.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kldnlutg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hwzcwsnt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rncdatwf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvyolmq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ufknksxc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kmeiiklg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3reknsqxp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yhwdsxll.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hnoypftz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mspojldx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aeucjsfl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fldxcszl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rpersbwa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3buubnuok.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3lxhsdsns.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axssdyne.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3vskkgchu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3llwtfnkh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3znyzaskv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bilmamac.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzdnolc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3eunrsvru.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3agmkmfpq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3cgyxhsog.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrgrfdx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zenazqib.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ikwiszro.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lmwratgo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ugqzaali.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uvopldkk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vsakytmi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dvfxjqer.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wljfaxdk.html


<!-- 参考信息 -->