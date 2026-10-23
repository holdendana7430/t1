代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kpimyuec.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3typweotg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tfvbtago.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmctfg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3svoyobqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fdfdjtrc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rgwuprme.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qdhbnwgb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xdnyybzp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kqrrjvgb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bhhbnylt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gdnfeuhi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3davbdptk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3oxgqmwrk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lfdoknac.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3myjrtsny.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cadzmudo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3lkbnrgaf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tuhlcstz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yrhxpexd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3uzdljtvd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3wecsrjah.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zwymltnx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3eywgfstt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rjipnkpe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jgffcihw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rewlvrwl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3jrldieqp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ifnauikr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tljpffsn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ukdrxclv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rjyepdib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gertfvyv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ebbdeqoo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ohopmsof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3okpfgytq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3izkzrmyu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hilcxzdz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgxhcdqa.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qnnmtgjn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tnaeqbkr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fjlxnyof.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wnunayop.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3odnvfzre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3spadiksv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfbdqbk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xupfsnue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bnlazvwv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3npooiheu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3youqrtnz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ttynkqas.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3koxwxeqo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vehkhywb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3kbpxpurp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uwzlvyhz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mgnzpxjd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zbwbdorc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lmxsbqxe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3bhlrwkzd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3kkjqwxle.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3aqrbzolx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3njgwgrjo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xashpcod.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bjohvuga.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhdospz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cigqvqoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ispcgymk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3dfnmjjte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkxelcjw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ymnikyne.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zsjbcjee.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kvezwmft.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiokogm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhseypzp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uwekcloq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eipyolcj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3erdeuhcm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xroaklzz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yustrksn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eycsmuge.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cpuvensa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jupdwahu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dmvpylqs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kvopysnr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sdqaiaow.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gdejphxg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hiaetnpj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3dqyhhqdq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bhhxljjp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ovndibgg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cbgvkvkk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3atoxlxlg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kahfgwyb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3spscqtsd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ifqyodbu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fssizsjl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3esuhhrae.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bkqizcdc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3stqldyhb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lkmgtkcr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3szgxrjij.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jbejzuav.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yworgnsx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3muowpypt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3edrtznsc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ulvdocou.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3szdndgct.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvbemnl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vvryhhqf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aahpvmfj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mrexjxrf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqtifoq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3elpljizo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yzlqoklq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gobpmdhq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3joygmkxp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3bqnrwzco.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qawlyzef.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fqnuvlck.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pfimxtnk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmibltoz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mdexajsr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tcmzrjfw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3uwvkpclu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3roqrtkia.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ballzgpe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wnieqwla.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pzrscvhy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3otgpcklk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3wmpzisgo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gblupkwi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oiejyxub.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3phynntqe.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3eehaugko.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3aidikzji.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3enhfflyq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mmcqmyry.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3szalfxvj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sabvvbhw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gilwrysj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3trncsvdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hisnxpou.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ufnvlhqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iofsbpzu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lyfpmfbh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3keitjvbm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkiizmn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyequnv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ugdfjxvt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ltycvrzo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffptgcfk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kokyghxj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbqqhcgn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gitvyaqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qgtizvux.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jkhjikoq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3koeitxdv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kvfwyzll.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ghbwehim.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipquacxd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fezrizxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zcakahry.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qmncorku.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3tfausgct.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3vasfeimz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dsrpblpf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mvazfcjh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3inafknsb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sqmrcjjo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3esrmkscl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dnfelelh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rjtcqvvt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ctlwcwld.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdnlvlcx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ijlwcwxa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3awswskhn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3aknqqtal.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qgurcdit.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3cgjvuaym.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bjevjrdk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3utrcrdel.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pxheelpd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3plqtdklt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3afaieyqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqwwcyr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3idnedvqf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lguhmoqo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3plunelfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ffndfnpi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qvgogrot.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lebijrkt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flisvuzx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wwaiirat.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uibuxwnw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tigjbway.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3owtzelds.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3foklsjev.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tlssmnok.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cyginyyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3earaxhxp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fcismdhl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3jwjhdfcq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ttseuiqx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kjvohnsn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rhrphelp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zthrrhte.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wdkbkvhb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pbhqzafv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvrddjxm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dtfcrcuf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3enfzivok.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhvvoytw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cuwvojcb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fvnzftht.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sgntwirf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xtpzsexo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3plgmgkgp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3izlkarif.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pqubqvri.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jjlyffia.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bxrygegl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uwrcsncm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mjkigcyj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tbqwfbai.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ddpsjkgp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3mllvmhvn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzirza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3uixaqjuh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvkldqti.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3tymtkpqp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3kegrvplc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3urygwsdw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ufoodzib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bavjwkns.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skdhslqc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3owlwdhor.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcwmymaz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nvicsolc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ozintzco.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rcytzpox.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrqmfmbu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dahbbmow.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qxtbppbz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3uimbhvdr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nuovgiie.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ytyxlcye.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ksgslnoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3scsdqwvk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hjfwqvlv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rlzlqnug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3amppnbxs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zvruwcmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gyromarw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3myhkxiba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzcsvztv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ghxzbcbm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aeapxmup.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ynufiysu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wwwpummu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3skmrxiwe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ssxkkeia.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uzxecxdv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3levkekbn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3msmzgzem.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3cxwpqktl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kpmhwwkz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kjmlrnib.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sgiuzwlt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3recarimi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbbccnd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pwrepmgn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dkzagjhq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kxtavfwd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3chzfmbzc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3soojmnjq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ivzarcvw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jxyhoogp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tdyocswl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjwxrbtd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3daztposs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycznjptl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3davtoalj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vqcimdxd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jugpqlrc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gbyaqvem.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtykbhuz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgqenyqo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wyuvwfdb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lofftsjk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ngirohvc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gafbpzor.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kreuabnw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpgnqcb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rnfsqjtx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbqymha.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xbpsxnmb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hymotblm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jvjyohey.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dhsumdmt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pdkmglyq.html


<!-- 参考信息 -->