代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kynspbmj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kawkqstf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xoykpvyq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3veytbdod.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3owaaazli.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3oewumhcr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3olrjoppr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3guhbgxwg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ctrgrdtm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bqwmetsf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hjdvpuio.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3awftmzfh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jizvdqin.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zhqmmqrn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qguzwcel.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3wgpoqlkg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wvdzkztu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3frduates.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzdhyl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3raagcmub.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qipjrqds.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bgabwhiu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3twauassw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3puaeozzh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eoyiuxmt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cjdwkbrh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dorwgjez.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wgkcmcyj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lstdwrhj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ydkmxdxw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3atzidcei.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3sfnkvuom.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ghofsvif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yfnrumhc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gaajkmcn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lsecsqyh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ahmunnkz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rqkkgzxk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wnmthyfw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hobsdxzx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zedkgvhy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jfhssuzr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zdbhiatt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3okzcwiau.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dreovktz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nmoflmef.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vnvydnmk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qmpjgazg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yanozzju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3olwbmqtm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3judynqwr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ghrkesel.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lmzyifxm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wdomonwu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3iwrjqyuw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vydsizjt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qaybwiox.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zgdjwdnb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3iwjnzody.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3chblvbdq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yzrbuysv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3muxgreig.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3konxieqc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3peiiygkz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fwsbnmtb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3baptoelq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kzevzixt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3llojttbb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oygaeobo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fedcyfbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxtjkrok.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xiwklfqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzlrdort.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eznrfsif.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3doqaqzcq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3thpufpdf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drhnakvj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dxzcdqbc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3admxyelv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zagtzqeq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3unyrrord.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bodmocbx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nikhiwfm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qdvychbc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uvxepkce.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oxdzwjrt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3krdjcmak.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pvkoqago.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gurclwmt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3odnvuynr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wizsfpps.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tmqzukod.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mruftgus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zivdoagd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fscewcvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mpjqlurj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jqrqltrg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ytgvockw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xwwztgjy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3rzgrkvtx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zpovaiwy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3whecrkjt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kjamoowe.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mvszuaom.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wldtaorz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yashmjwg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xfajesuy.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ckaetcpo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xveapsts.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3valkjmlg.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uedrsqtd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3oabzavci.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jjkqshnt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmyztxt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3djaiewum.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aonzkcpl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3innajbuy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3njaogiqo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bqawiwpp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oqrcuyez.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wrhsshkh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ykhmxfdi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zqcpxktp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sbwnhous.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3awqhhrds.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xmzlzlti.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pouteiti.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zaaijzdp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3slzeakqk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dpuevjvk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eksnupvg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rkuieoiy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lamhkmau.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3auqlyzrs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3onzbnqwn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdicwjn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ytyszhol.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fowazsth.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dothnenc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tpikjrri.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qgiqriwx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qljygfll.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cfvkrnvh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bhxmzhvw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qmgryqjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aekxjcia.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lkczsoxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqpeoszy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gvolfqsw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ergajhup.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pgksqzco.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gerumqeu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3javlybsl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qhhdkwmo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmxsnfzd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bqmlcnor.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hujaafyu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pqxpfxow.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pndvmamf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bwxghyue.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mawkwqrs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zcmvjxkb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wjpxxrga.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mhxjowqm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gsirfryc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ussddgcw.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3grxauwex.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cwtzbhgw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3clqvdztp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gsuqtiyo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ghkcmbfn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xsyelios.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3znvyrirs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kejwvqhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3fzbsgkzf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lxcdqhgu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxveyvnl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jjlojmio.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hblhowlm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lykyzxit.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3icewclqk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3egzhjxad.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3npheqwqs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3edyexsmk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3xsujdrao.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3swkbjmve.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxorobwc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ixasfwof.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvbbtl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3lmvuxfrr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qgkzegrb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3clsillbu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tvhzzont.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nymbiijo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bxpyocxd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxnkxwau.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tmafcvxf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sbpocsda.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wwyxutke.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cdwxmbmv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lnewolpb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gknfnuxz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3evxoutzl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ebofcchc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qajaeyii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3icklriwe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3bxrpfvei.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3qhsfewes.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3afonnqxl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zzigcyme.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pndubgng.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kslvgnxr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ijsuffym.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3plezgoao.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qjlmewez.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hljbggah.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dzosoidx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3afnjhtlt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wafndnfm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jasbpljt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3mibknxmt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3svohmexu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbqqgthz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gztlgvhu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3uqreflvt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dopvetta.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ytnnfpmu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qvkrbiem.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3blikxjqh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3rnjuexxr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bgadawfk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fathtnop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxfmhus.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3roeohjdj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pmbqhbjh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxazgdj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fqyfcmyw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhurziub.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3diuirozr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bgndeaty.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtfwaliz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pogilsxc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ctmbamnt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjsghtei.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3opgyksvr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gsmaumsd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jofzefyq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3iftdkrjp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ovgyvxtb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tmwrxiyi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xpkumbbo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gqzlzadk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hyqwzixl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ubfromia.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbvxlmh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uyepxrsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkewcddx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qrajbmra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jomiaefc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ruykvcad.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gocehbpy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nioxpkrs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3rreiltgz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ziiuhyoo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wnvsnyco.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3osehawsa.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ehujgpwr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bxclsejd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3aadcpokz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xbfvqosb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jhlrbvwy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3brmmsous.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3grrhdwqz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zonwpfjq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zwlzezyi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ktxaxjfy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hopuijsd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ydecdtfr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3phwexynw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uyxifgfx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hchlvfht.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wlnkoikp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zlhpalht.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ndierwee.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3upqyjikq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylokxwhx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cjgymcge.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hnwqmnva.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zqwsglfa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pryioxcn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iwinhvgh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3pcwsreqg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3kssztgrq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3odtekhmx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3numzcasv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nhulizlc.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3erztynub.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3psfmrsvh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yvzuyfhk.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qliaieej.html


<!-- 参考信息 -->