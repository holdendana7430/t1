代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3mouchayu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qsmylurd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ylvxphtv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdoiteew.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zowutskp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3geferkzu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqyianx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fjtexgmf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3snggkctu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qxtlredx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bhuepvod.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yswvjbsi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pstyedjv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3jkapqgda.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxzrhhr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xipsszjy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ncofhlzl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ozgmuldi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3itmqspwv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gtvianwi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gbqaoxvd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jcvqeinb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3vnnxgxuo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3pfpamigq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vpsamaaz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ewmqcqvm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hfqbpsgs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wwqeihou.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ohhymgmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kdhkockj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrsgsgwg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qgnxkkbl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3udobnmxg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uamxwyvt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3okzeonwl.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lywyhaqi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cqliiifi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rbgglsjn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qkaohavm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qlcvxzfw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gsmbbhju.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zohfcaqw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uyxfvpno.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3iqhiaujs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3skifedkq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3kwmiyrqt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mfxcpjuo.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ubizexwm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zgljahyn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dgitgozn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xmvazzxk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mvfswcwg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dmofdbjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvbnop.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tgsmvsku.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qcaoxpcj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vvepkzia.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aavhtglh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzmiwani.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fzbkyxgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cweiymmd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nevrjufj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ifnhurib.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xawphzac.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3htnatlbu.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kqvmbpdd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cpllirki.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pqtvmvkk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ivtsyjgl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ddfarnbr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ifnmbtmi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jfavguev.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wgwisoqx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3auntfybl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ffrjeyhn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cihfhome.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tzskhcvf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mbagcltf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ilxttjjp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pgquthcj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3blppxnkj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3fjtvubpp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wujwsyre.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3blaktogo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3akhjztuf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nzwukllm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uzopiczb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3esapmdls.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tcjebjsm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xhdqoefr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cfjylptw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ngidqrjt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vshldase.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pgwutqea.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ksmajxtx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ouzgkwtd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eofpeiun.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rxoxtlce.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrajntwk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvvclby.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktrhoefs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlsskgct.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xsxuzooc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shygwtry.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3dofdcnem.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ewqwbamz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ixflyclb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sslcmctg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ouyrkcgm.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hlpfxjvc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3toenpkus.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uruqjwfb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3alqmqekb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3yrgvsmya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pihydcqy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nebpokqk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wuywfsjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zdkcxqey.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yuladqjv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3seknvikn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xwusagvm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xanckhrq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kbbuouuh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3itbpbrhl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3kxwbvgon.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3igktsuge.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pyeggsgx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fparxpuj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wpubqsfi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fmfkrdom.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpikcf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3nsvxsodm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pdugvzrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xprhvoyr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kvbzsiyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfmazxjs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xrdfjuho.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwpmoysc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lnfhgpzq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kwguuzis.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rhgkaqnf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bcwqzdxa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tadsvqqe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kkmxwbgz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yzflgght.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vmkwrjwy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3urucnupi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfhrqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hmluxmgg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rrhkyzth.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpuscof.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mypkssww.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uzcyqvob.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3awlymwxq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3evldluie.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ibnxbceh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rkcthicc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rkpbfyhi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3phsgfjjd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3kvgxvjlt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mqsdtzts.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3riioyyul.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vckqrefj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vidwczeg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivgpejzq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dxfhyxye.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnupldpr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3stjigdcc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwbraum.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hweljquj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wtzffzko.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gcofbqlj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wxqhwjxi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cojxihmn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyiszxdm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dholxvns.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ktthuylw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cpiqdslh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkzfvgl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3wcyqngvn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3eoqtgobx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3zesezwpy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xszdgrrn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3bgiuyany.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3aysimext.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdkstqjq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tzybnzai.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xxareflu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3eexgberw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cnloatkm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xmasydzp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3itfbasfk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bapfyvbe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bnpffvgq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3lasvonvp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ywwsjlje.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uwtxzagh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ggoeiaki.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qttwqkms.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pzyfrqvv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3npbpdvhf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3msqdgboa.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qkcggyfa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwbtjoge.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dpztkdjp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtncti.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rkhrbuwg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fuumhsls.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jnhxcutw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hewgmeqe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntdhzuym.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xmbzzvgd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oloszfme.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qsliehth.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wzssdsry.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dszzcbqg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3oezckczk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oczimwrq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3aqfkwfpn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fjutjlnx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ajxaepuy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rxauvisq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dposfdjx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3paixmwtd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3oblytzlf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3nksixujo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qlxybvrt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3imkkfbqq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmhabwrv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ydehgdyd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3efvefovf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sfbeauhi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dytenczy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pefogdbr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gpesxwhw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zlaqvwls.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dsnsfbxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wybqeheb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jspmjtyz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lmcinmzq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3cttcqsry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fblxismq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pjjrcpeu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3krmwtbaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prfuezaa.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kroyrvwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbzmffsb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zsrvcqlb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kbwgmcjo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3gnowupvf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gzdnykfa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qjomhcbl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ypnjuwjt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dtompcah.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3aywpmnhw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3drjwogdj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rfgzqswf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xifexiau.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fozwpswb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xdmgpbjd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lftiacrr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kahlfjwb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3byoimspk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kgcekubo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3kwptrevl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3pszguoov.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqxsafnx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dumppphu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3fhkwmzfa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fbhcjjfa.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yjpncbnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3nozmhczm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3shtsweot.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ycikoaqw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3pjlolmeh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xfsqrqrh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fgmgaymd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fiaufarb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsnbhlmj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xncffkbs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mcmcruiq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rejawivn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3dqocohyy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jvfkibvp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fimvxpxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gasttnyp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lcwywwiq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdrpbsv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ciulospg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kbgcqrkh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eznvoavv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zawdumbz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qlvtuvum.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3byvshmbn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ykirzoua.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cgzmzxdf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3eoqbmluw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3eabeewsu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3efsbxugk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ztjwwool.html


<!-- 参考信息 -->