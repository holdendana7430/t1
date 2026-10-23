代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3uojzasij.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dayvynzr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3htabfdia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3njktnjqe.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hqhfmpyt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tvmcvwkp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3diqeykeo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sakwryan.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ubwzetsa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qlxlvdnv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3owxplddp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3oxvutvhk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3icfgujwu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ihjbmlye.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hlhpxtbb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmjmpx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qpxclbos.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tjyyqlrz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tmmwsycv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tprmfgat.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cqsptzmc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3subjbayo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3spboddus.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3paaabjfp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcbthqf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3eljgigcd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3pwemkaoe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jviimotx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3whbiaave.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3asssrdxp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rolqhswx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mvhkkjbg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lyelkmpj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cwchugmv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3krvtoiid.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ontlczbl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqjpslw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tgtvdaqy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ouepxpck.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3znuiycya.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gfsarhzh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hlzcqnzr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyspcsv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vgrbmepb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rpzsmbdh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mtbacwyn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kmeplmqy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmkbnv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lmdsnebf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ilzqajlu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vcxthxpt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bhkqbmbx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vababwzf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qinrzvks.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3woahwrqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pvyoaivy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dvsyfmvk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jqrjmhbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkcidqkt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yfwcbwgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufvyxqbw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lxqdvkbt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ebzrowax.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gjikuftd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pimocafi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3souiosoo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3odhrivjs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3esnzzlja.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ciifxsng.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fpjbjlcm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vzarqhzw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ukzkbxzp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mkwplcdh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3muoepfzd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hirzclws.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bxwwaluo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uuojvect.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nbetfpxg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eygtuywc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3swgrwiqa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3irtcmksw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lpefzpii.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bkhkqche.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xyfyplll.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3eikurtlv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rkawzidm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3farduihe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3tcbdjjwd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nreaggbf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iosxjusm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3magnlcdq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3abwkkyuu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vckoehmg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yibvvzag.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mqxtxkkx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eoovqvgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zgtmlrta.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kkjacqev.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3syywrzva.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rbblexjr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ycreghwa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3caxcglrn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cosppsfz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kgllwqqj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rlpczzip.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3czbepgmt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rjorgatf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ppegfnpl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zcrnitsh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tmjmkfud.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hvqzeden.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kvzlinag.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vonbhhpb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yviqkmrj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ipcpoqap.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dqmvumxr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yhweqnfc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hsgrkwdj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gngnkvoz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qqtowbid.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3prgfdfbc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3sqbluzbi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3onlvoflj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vdaswcfo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xqkrxszw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rpbzufjb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3exjrqhny.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bdogrrfw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ydiitlpq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vfnnzvfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vxptezlv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kkkjhydv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdzbem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abwyckxh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3feuijkls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efadearu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ssyavaht.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rfxpoflv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3esvdlfnn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gkxmqdpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3izimeipi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qvixdqvm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nkjnookd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3yohsuitp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3avjeligm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3puicfuot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uwchqngh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dakbkeyy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rcfaciqm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zjhdgslt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdgimek.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uxkobwob.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zfzrinda.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3abclbcdz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3piebfdpt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3bvjqbmfb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hapumymc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rqvrnhpm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eteizkbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3voykktxc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3csyonpnr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gldonuhb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3nzgfcqsn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rvnykomk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ankcrvkt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hburziie.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ppnthwjg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mijnxidg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eftyxitx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3frqbnwjq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpdnocn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3udkowlhm.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jzowtmmo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ycbwqcfm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hsjipszn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkkhqbum.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiqkzirw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3oifwttgh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3epxxeybr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lruvcqbb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fdwzkdpl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rzdqtccc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cnyryuov.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ggfpeowx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xbdymvdu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rftxadoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ytptwkuc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3musvxnkv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vgrhuoqy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gdbztcax.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yqkbvpcz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hmhwjhug.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cnnttvbs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqijfibg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iexewfru.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3txglxspi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nvgfbvdo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3urrszlhm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3etsmnilr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3anouxhur.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pdrcqgbs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gtlkhzwj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fscokwhq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cofwtxsr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bkwwpwmf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3duayfjur.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3koeiniai.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pzwszvys.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hiporrob.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hemhmhle.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wafkxpjg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3roidybez.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rkxtqame.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhsexdix.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3alkevncw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fbnfxsjy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3amtzbrql.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3tbcmwazn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pjwitfya.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkjacsyg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3oifhvwlo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvuiofg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iveebgwg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsrmpyn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwfvmwj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3junvzbcx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3lwoqaafa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lqjahngf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpkralqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lzeerqrm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bsgyjdxn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tkzngsey.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3djhzpldx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qcnrazus.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ounfbful.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ftwehcpv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gkamhlif.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hxhibkqw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dkyzdert.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nilnilxd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ujboaduo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbcuxnw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3yqpvoerc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jxshkwhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpvscrmh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dwigypfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prdgrilo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cgavbnqb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ydyetcss.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3eemruouk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3montkkuk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ymgszuiv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3adipyxoq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3exqeidla.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lnofvlly.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ipyvpcue.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eoyctjnf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3nywjbbnk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ibcpjfll.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bckjubct.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zdelcwjp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3otkoghla.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3bkfwfwxc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3huapeadt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfkwos.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kqfzoxrb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsdonexl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3nufnarfz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ehwxarbe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3upxlapgr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghikyerv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dnjgokmb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jbsykfmd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkknjhzr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lwxslzpt.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jrhdvyio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3epofgiqi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kasksefm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdhzdef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ahwdgcml.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pqfnxpvc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3okhtqcjg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeuiehzb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gtuwptfd.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3elzzqwct.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3dxbgtnwn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kamdabwy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qcscfapr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3yikmmtxs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cxttwuyq.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpgukhx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3addbkotq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pxhdcbax.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3hdaagdgq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3xdsvxtln.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qwmwffdp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3plbcxxns.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3wgftzupv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wdgrnvjc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nddkvkyx.html


<!-- 参考信息 -->