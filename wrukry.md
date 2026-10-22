代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yoyewuav.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mitilcsg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hnrplvap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uatjzyze.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2aeiswwez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcfftdwa.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2silgqcjc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sosmttgq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ozkiwwxa.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qzwuaclx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2scenyqet.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zceqxtif.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eyfukljq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zqvovomk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vjenmeae.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zsvcwqoy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xnkhyqwa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2luhasdtt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mvibtcyn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ghclcqtl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2oylcxqyl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2zhpxzfzm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2hfmbbqjz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yoikflyy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lxyrjvbn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dltwbhqf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2otpwncxj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2apnzqhjf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xxtwvoqj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qezyssdj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fuvilyzk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2aslteqxt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mwynoggl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2tbsjhopk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2slsojznk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bwhvjlph.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzpccx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mimzadwa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oadoifxo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tklwelxp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vubbpglk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rlokbvml.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2tycofowe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2hhdxnihh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2twserurv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mbjrybor.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wxafifzf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2agbbvtbc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2netamggf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kyftkxzm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccasulxk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rxayubdo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hfkxpeun.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ezquyjqf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qmwfhwgu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hqwulnjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aubigrjh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qofaridd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ouhqiwto.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2nwzunrcf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ijhbecsd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2blsgalzk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zskbxggs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ogrjvczf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dzuinopk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rpfqviie.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2budpmgvx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2iykurdwe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bqpbfvbd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vaylpwvp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2juayaxed.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mlgvqzwx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uzakclef.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2asyburcj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gciorkum.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2neurwnai.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bkyogwip.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2txojllqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjvqnott.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bxxaukwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seldoymx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2elxikdqe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nrivyxed.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dxapzadw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bzekdzyo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfjgrdyf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pbhcmlkz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ktiqzadk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zwmmsvzg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zjdzmsvk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fykkulux.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yyxwyulx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zpkmnqud.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iptwwhvh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rcxkivhp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rhcmuvdy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rxtmlsic.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ktvrjmfj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2laznjkri.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2iwqsreap.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2wrqqxjin.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pqlcbyse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tlngyfyc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yywlmkby.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2eqsduwdj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bphyusdy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2klizfryf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cyhojzqx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xzvnlecg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lnaohalt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fgrhrgih.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2acuuigdw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vfecqbte.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ippczsxn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2glmlcdda.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hhueqwub.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xlhzxkwn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mgquncqm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vnzhxasr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2upomejdd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypiquqxc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2boxmnarj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtrlfzot.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrhkhfr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2aytewtrm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xnumewic.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2octgeobb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2thogwywh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uihfnjlb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fyoglwka.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vlmosmuo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lyirykmh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2cocttmbp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2euekdqkv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlpqlya.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2fuyncpdu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2aybnwrgn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2txmvgkuv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qpwlwcot.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hfncljnb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2whndusmm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bhalkgwt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mlfyggbc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2lixfkelg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2udfnpafy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2acvxhxgq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ueolrnbp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fadtqaju.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ltlzudzj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2uzhcwxfu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lmciriqj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sciyepvv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2njreyvgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asbaiidu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2fyehabue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnmbgotl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ovxhmjui.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sucknqok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uekiljtu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nmtzbnvc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mskpwmnw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oghlxyoh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yzckeawp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2isjpwffz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvktmijr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xqmyaywf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2icsxewkl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dcemhvhw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2inkmsmmo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykcyabqc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tnuxwiuv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgmqgkdi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vuvyhtwe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hkztaakb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2utikikzq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hajbubfi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vrecfjhi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vvutxbnr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ogyhbmus.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uxmbfbox.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tgcmzjfi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lymsspdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2noldvnrk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2iamlxski.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qocrbqfn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zoyavgqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2juzymaqq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2feysvkti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2exrdhshs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2efypzwxa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hipbtmsu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ermivdro.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bjzucbzs.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpibdmj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdwywaxj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kzcubjuk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wjkamunc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2suolahbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2xqpegmnj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2efdjoeiw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykyvdhwh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shdsewbt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bvmoonkm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrlxnylv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fdbedece.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrbicyn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pbbtpvqz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rtzzxzke.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tlinebgp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2itxmffpo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vxghwuug.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jsttvnay.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ubpffpfm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uhyrfaqg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cjezuybe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2nghdipgy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xgxlumao.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xawqgggb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pqszxcyz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qxtqxfxr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvgggyw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vuyepttg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qufadiam.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qkwwiiyd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jicdzphg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vngnefly.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hhnypmfu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yjbxptlw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2anwynqfz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gpklniil.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vftvunwa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tqihhcin.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2srqsdsbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uypqxjgy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wbgwgqeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2celkroac.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ujvkoipy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2gtmbaahy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wzrpyfhh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqfgihiq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2navflmpw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2udavqshk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqyiisut.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2koiyrrxw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2umxqsyhj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ogftjxby.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tdgtllnt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2huzbqcse.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2chikdgaw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qmtjiczn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xnzxiqbh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gzmdvkop.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jgsagxmh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2dazhkqdh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hgxdryzf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2eqgjuxmf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rffcgmdl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2htkzwtlp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2boidjfwe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bgelddct.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2amuehrze.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqcefgae.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2revhdtng.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dabbbshv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvtcfwpc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vnohtuzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zggibckn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mcaabsns.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nhthkjnh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2boycyhog.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2drhiuoyw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ubzlrssk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ayxzrocn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fxfehemt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ufhvtrew.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qqbanusg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qtzrjhdq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vwmpclfi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qlpguacd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2obofzgrh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2omxrsegg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dbddlgfg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dsgddpsh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2reiawlie.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2btonxalk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pzaunfxk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxxvofte.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2lqbyzapl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hckaicld.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ftvqesep.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xxvsuotu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vsvbogpb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wdkvmfff.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lmlxyvvp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pindvezp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2clvlzvjg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fsvsywvf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agaljtsv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgrsuicd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2plbvcxah.html


<!-- 参考信息 -->