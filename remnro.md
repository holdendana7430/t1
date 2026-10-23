代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfwbygf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ransmctw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3enyeirby.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xoamckgf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ydpyoxkv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qbidulah.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jnlavhfi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ysdubjqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3fddakxog.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3kxzvhofz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3boeaymim.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdheogux.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hihasqud.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3rccfgaij.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssoilnkv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iczmbceh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rypgirix.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3dtvlopgm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mbhmvlwz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3sgivgetf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lscxfqjr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zyqrhdkt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3uvibsgan.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3fpqtrfpw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3adsadpqu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3tfuewulu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rkgebfou.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3oburqwip.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ybmwszlp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wckrvobz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rsizymiy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mclypbxi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3acrgqevq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cvskvpjr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kvzdbdcf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3mwtjruzs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mpxsjlwe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3aieodvjm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3akqzyvea.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lzjuintq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sdxgdnfa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vsahmbtb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aycdkscr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qoxgciwj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wzhqqhta.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3eujtnvmj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbgbfod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uqiveebh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lcslppep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3skezezpj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3htqbobya.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zkwkvuah.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dzozyopy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xzixoyyi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ytvfoeht.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pjgncosw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xbxqapnm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pboialed.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pynfxdzg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ydoewzzw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mubraewm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3blhtlrfs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lnkafjsk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3sjfkznom.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kzuoqhlt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3igveorqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrpfvzek.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rexgljvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcosnlyb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qgvpmqgn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vqtidbyf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xncfmvdh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkykvjfr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yoafdrkk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3igyepomb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gcaboygr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bpikcbtg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mkxhxdns.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rhtaqapo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fjuntokg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rjcbwdev.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vlyaxfwh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cplpkziw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xwcjegpb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ymdixeqq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ibyizrnk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3emexnknc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zenfjfjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ekztioiu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nzuvomjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3naksugik.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fnjisfin.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wjssdycw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3evsrjjrf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dnnfwqil.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uexiqrbw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3icrjczwh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3skcpmpgn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3orutxooe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3sklafuix.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3smbkuyip.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lzunjmjw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ldeyusio.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3uvzhgtoz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nuttmccx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3uivebamk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jzubqech.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vcaycvqs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sgunvopb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pwcscpcq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sibnatmt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sjnscwdj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cbpjxkyl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ccciiolx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dvhxksux.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zkdsjhbj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3lthnaqah.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kakyhnpd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lcdbophj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qdbygiow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nuwvozie.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cdglfwhb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmujpwt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zneoyulm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3auskzmxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rgctltny.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3naonxitu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wzovqnwu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mcebokzr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3boenjskh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nienlcsm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jelkbief.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gfcyiyzd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dyrzojbw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cqmrrxrs.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3niprtwum.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vmodmzyp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pexvucuw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ysyfjfmr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bivhkigl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3asidtwsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyfpwuvd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wjponmef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3koqcfscn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3btnbpess.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iykrhgmy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dxvjjjpj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pewpxlgf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rswvbrsl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sigaghig.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcmeoyud.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3celwzful.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3miklfsvb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3dfabdyoa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hnebzrqj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3rqhuqlqy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ikudzplu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dthkdiib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3moacbizj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrdfipg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3brbrcgva.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3iqvdjyya.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vjrextft.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3satwcvho.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3eogclwjm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qonzudye.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qyrhiybn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3oiblbsoi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dcqugswk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gevqsjci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qsfusncq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3altamlma.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyiyigbq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjbtidyk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sikkmpbj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gdxfkdqb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aycviiwc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pqzzlzla.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxqohpz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxavzdyq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mhmpfkha.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cclupsvq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vbyouqkf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwqhrrel.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xtwfpvwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3wlwsnppf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3uyovuenx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wfuanzke.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfevdmzp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xaqsgvln.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ftaluhdw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3credqmdy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wftkaelz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pynsxoyw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cvtictgs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zdobnxak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwcuecyo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fjfdjeut.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zlxqlnti.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ounacxos.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pycosvdi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3plrkcbne.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wbxltkkf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fzxhadna.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hccwtyya.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wvwnxhkx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wmenbjoi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3sdmyynlz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cwzmxpsr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3pugxanci.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wgmjtchi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjvzmw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nenrvjgg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxitgfbz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qfchsmen.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jlmkehsh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dizcpbly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kqjasypi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3njczwlsx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oicwftvr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3oznyjhrx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3encejxyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lcxbnhlc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghmxippc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jbguocid.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3htflyuyu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3usjsrinx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbpqptxi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3trlncxuw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxsamvgk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gfkgdoku.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3epxsjqka.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mnyfdoig.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3urxmgcne.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3obncevpa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zmzmysny.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bkupwkzi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zesodlli.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kvobyohp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3shqxhnwi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3txqyqpwy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tvwmovfz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eqarbfly.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3azifdsnm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ecrytwuh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3hskqyyof.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tuckxumg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vxpinnvq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3styhprvu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3gssbiubf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ltowapke.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qsucivdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcncnscl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3oifqrqot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iljzkttq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3erparwft.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3skpjrtpf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gcousyft.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xwqvldam.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3orkzlnir.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3yrffuxkt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3treitsbn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wiclbvcb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vpsrceuz.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ucwicjvz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3dxcespzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kejexaxo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hpvelwpy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zcgrgnmd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vbkiifjq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zexsizff.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vbffgrps.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nfcarjxf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vctonzid.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xarnkmgs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3codqkrps.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lwxlqkls.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3krlonece.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwdngex.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mkwkyxjc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3elwmahmv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gixfzccc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lffrecef.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yhhrwknu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qqwztaxq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nonwnvia.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xpljmzhw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jpixmhlf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dhijaeli.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3iwojsazh.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qktqhgim.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bdqrbfpf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ezydaqqy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gojucemr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwwmmzc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3exrydpam.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bmclvbwm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3oyphulcb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oncihdlw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxlurbl.html


<!-- 参考信息 -->