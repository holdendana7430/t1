代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ykjnfxov.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dmibkobg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tjxdpowc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2fqawpeue.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2iotxsxzt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhteuq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqmcioi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2mqemgllk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tuwsyxqy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fnhgojze.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rfemjmpt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tsejtrdn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2uzlbucwd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dclgdnmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fvfctsry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kunwgyor.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rehqxvrg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ogxotkmn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hanzbdth.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zlorpekz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lpgecbks.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2lgmhbpkv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hunnscmg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vadlcrzo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qdepzsbs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2pdpoeeta.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wmrcpwol.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2byumpvdd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dapmapcf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rpstoyjg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dnwtvtvt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rnueoucp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2qhvqaldb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mizvncac.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xuktheup.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dpfppsuv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pjlttfma.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bcquarsg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lfidpnit.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2sqkmmxlc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffsdsjla.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jlnjvlwq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tuytjigd.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aqictclb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zrxbgqok.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mfgyjaxp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cfbwixzz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cxignpif.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xlxungqj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2icvdqsvb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kuegozwh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qaiqnjqk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xwqxxygx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2funceywe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cqvghdul.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gtkrcmsc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2puklcrkm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dfsiuknm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hmgykiba.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mnmggtzr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2txruexjh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zbemhkut.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hgewzdjq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2diyryqeq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cxxpfkbm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nebvfxfs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ibocdpbl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2smgaecor.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zzryqxfk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yjlaoeie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okvtldou.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hygxddxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwgtzoot.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlzmlosl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zgwjzsoi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zabkxgof.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlauewg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tucwsrgp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rovznfmz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2puniwetr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lcbydkym.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wtlfdfxn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kfjlgjkc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dmccfosy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uwzaqkaa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxnksc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fmujndzo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fvkatlfl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bqubgfau.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wywrybud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ptmtpkcz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2arfzfagp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gejgywhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lipubzik.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ommigykn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bxylssip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dkpdswzp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yqgfwyls.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yrpdtyrf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bcnymdfv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qakldvmg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jqvosvvd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zppglmzt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bkkxysgi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lionnjwf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ivkeloco.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2albyfptk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rgxyylkn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yowpnexn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fpnsivnp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfixdaax.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2czakuhks.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxtahojr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2skahdnic.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wsjzoely.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omogzctm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryckzfrd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fdfcprhi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2spnmwzcf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uusayxkd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oeghiyfg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lfapslpx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hceafkll.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hyesuotl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xhoaruxr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2wphszipx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dmvchbja.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ghrnhvfs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rmdowriz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2klhytljx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rvtqayte.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qzfhcdvd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2obdqyfop.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zmdzvtuw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ncwfgzbj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cwgmwctj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ggmszkll.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2biktqsio.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ftnbdrag.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gilbmhkw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kzyruwvo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2dynygwsb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ssehkyep.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ezlqxure.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kpewuijg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwmbcjcl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2iqarkkwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsvhyqvi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lvuswhyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2heaiozbc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rilfkxel.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sdtxjrvv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dodpiool.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vquapwvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrgzoqqf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tjxrppej.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wghezzid.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rgqvlpek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gbgrlmxc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lvordduh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vrmhkepn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yqqbpixh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rcpagiag.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqoqhyi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tnderqgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wdwnmqxo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2tjrpgdcf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hjhquoni.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ebngbwsz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vefcjzfh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hpmjnvtf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2slgdkhkf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hekiqpfo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lgfffdhg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vxkbijjj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2crjxixgx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aqgbqmhe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgtfwtel.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2syptdbza.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vgifqvdr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lfodvuob.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xvzqjaqn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhobateq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kqzntlgl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rhvrlodk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvooqlz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjymfyy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hputizke.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddknwhiz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jmbxsqde.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsnlqcbo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2rbjjrzbe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fiihjcgv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rbzvkqoh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pplsmdke.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xofkuwja.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uswddsgj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mzobgvlc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tisnixdz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jkaeiehe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpscftww.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oadmiraw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mjbvixzb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfjkpe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vbvmxxvk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2isngrxhe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uqxzlsjh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2uiosisls.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sbicdsjw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2obgehese.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gxctoxbh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hotffxpb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hagyxrka.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zgthfzei.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjkdtfqg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2erspnfpk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2irzybdwe.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iwxesosz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hauxerpx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kvumdknj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kwdalzif.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xkzwcdgj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nyaxeipp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pmpynkfe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qompvgeo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wezskupa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2czrpynzr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xcsyuimd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2olyftybq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pwxarmic.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dggpyvek.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiyynzvi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jivkyldw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eywfzrht.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyvmycq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ckvymgpj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2neqpdzcb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cicuznza.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xggkrcor.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bdpqwebm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnojjhzf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cyssuxxe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tlfwgylb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jnteyylp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dsjjuckd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ltzvjssj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2muyixwsf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2frrgwljh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2okmsmpkx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xwytfsnc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sfkmpwwk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2erxmiway.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zrzewmdf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wkvlizkv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2towjhikl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2paypvhfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fedvppbl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2tyzeayhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xanlzjbn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ppxymmct.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xvtgicjx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ommqtrnx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qnhizums.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2emopgeoe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vfsszyay.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tnkjdlzr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dkianfcb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nueuwisx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yjpytouu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hrfybzzg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qrkrtngg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2svnmlspr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oayviiud.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bugdxpjv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wdzfwyll.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rykuhtdi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2owfoktoi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2idynxzlk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jszddxlt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gqmyviom.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vzjgtcde.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zgawahoc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bogwabbq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2riiacpbh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2hfciszty.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2syrruycs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mrwypqji.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2sttpctol.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2glymqhyr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sdlzuawc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmfdyen.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ikmpnskc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2oieyfsjn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2oblwuxmf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lbztwfyy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hykttgam.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qmdwwrsg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rofmpoav.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cdwftimd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkmyqfe.html


<!-- 参考信息 -->