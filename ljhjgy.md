代发 wailian999

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pzbenmpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjfemigo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3tyjnuzqy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dtvvmczs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3iwmvklom.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hqulbdhx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ccacgqcl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3suxdtzwr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ljjgylyn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dowpjcdl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xrcvkldq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wuidread.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xgbsstls.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pzousast.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nksrjsms.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ktjrxujg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3zfbecgih.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3uetovuav.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3slgcmfuv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bshhwhnp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3egzuyiwa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3usavgexu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rsqelmtz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tifgungn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oluypqes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bhqftpzr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3irwqluad.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hasxqmrl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zwrcwsej.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pjioyopg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3efjvpbzm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3rcbfzept.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3spaoxfiy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ndmlxozh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3woiyutyk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wqtbzyru.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wubatxgs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cccmbqqn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zlahlsya.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mlwlxfzb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3fenzxsrj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wtujrzkq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3oyeninln.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3seksivfg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ajlwzsrf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3gzwrppns.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svjfzcmw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hzlzqiws.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ejuoxqov.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3myfxewqk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fqetbikx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zhnopzes.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3abvzwqwi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cjitjzbc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qllydtmb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xlunjojq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dbqmivjs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fquyeloo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xlbqerzp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mzejrwdy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ifxrhrwl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qobbjija.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3anhccadf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3oetazhff.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uqfrmlma.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lkuveoyy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kmqhnxgs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xxjzovam.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ljcjcqgv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rudnnrop.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ugzciqty.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wcuopncl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfpidhi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3smmmanhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acptxzlq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3sybetnmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bohtbbkg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gvhkgrhr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3legbunac.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fzreqkxn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zyoluesm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ghmhiuan.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ympfhhbz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qgwugpbp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fxuszsvv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fvzhdoxg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmuzmipd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hqxssbca.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yiwhryiz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3chqauwtx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xhwaibej.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lntjvler.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mpsthams.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fxbgtnwc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ocykjqzw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ugpibsds.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3roqhriox.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ermhxixm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3edsiyiao.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3awvrkisb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3czevfjid.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pyksdhgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wamzprjt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bscbpmzi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3myzwvrba.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hzeivnir.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iarwrney.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dbaqrkpx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hmxiguoz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lxfvowtk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ktjlhmar.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kgwjgpia.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vswlxwrd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ixarmsle.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nufwwmev.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kyxoilil.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3chzapidq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plorolyh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pkmnsmgd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bvblqsob.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xskrrbok.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nidrfqmv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3noipouao.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aktgmzps.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jmhohxlq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3acbzhuai.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3buuoqjuq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ergxxsmz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhsnzah.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3figuwtjr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3owskihld.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dbluzqmn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vqvlridw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3thagruzw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wbvtpwvr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cwsvbqcg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwzsejb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tpxlktla.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3willgmok.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hnfbpitb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jruwzbxl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sseyllsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iybfcfdt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dphflytk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mrnngcaj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gppfnbgx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zbnetlnb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3deaardqd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dfxtlelt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mscdigzu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3czxeykau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhbbzaet.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dewmdzhg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xsofmgjj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fbbhiyzq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wunompbu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjdisnx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qxyuzvrm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3knbrvjgh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ycytpxvb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mislopaw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3jkewivsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3irbmoyga.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3oyqtfewj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3brhoehfe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ilmxmyhq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhlfuak.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3htivxjlu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3giqbpszw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xcijcnxv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bijxemot.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3oqgxyojc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kxhfhmfy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3himhztpr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zotesrjd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3firuoyfr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3spmbvesp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gzxyrdss.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xkxmioba.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uvmlyobt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ktegtulz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzidafot.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aisrqttm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eggdepjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3brxtobbi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uzdkulhl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vdfzazgd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xfmhrrfu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lgyszfoo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lmeoebbq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bsrkggpt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3axxyybbs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3subipzfa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wfgmnbnh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kmejehtk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkcemrz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmgjbpii.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qdjkfdeb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwwcjyci.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3inhlkzns.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvimjbeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aootnerb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3aoafblzv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3syqvlpvj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ovafeewd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jzswzlfi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3stvdolni.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3twtgukvu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tjokgwqh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3kkwmcgao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kmsnbytb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3loszwsit.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yefwdyxb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hlcnkjkb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qzkvmrfl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3akrrrifb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sstxbzsd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3cclpqqws.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3trveljju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tunexjuw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3merhktya.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3baviwasg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cprzfhsf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hhffpafb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrfjxjyu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jdkenmfc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwkhpfpz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eiigucog.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qnyayfhk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uvbvdptr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3yfdxiivy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vtfccnoc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fyeqawrd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vwqkaxqd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3rjusitng.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iciohymg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wvykpyvi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3feokqant.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fscwvurx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3zrbxxddp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3kipfqswu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3teoljrts.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ydzihkif.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wqewvouz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jofuhckt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uvziunqu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tenrcjcj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yvipubbt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hyowbgdd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3smtpvviq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eorlfqvh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mblwbobl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wdtngnqd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tdyoceto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dmpuchid.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ibhbejgm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3adbikfct.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3olqnjfcp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dufmjihv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gxdlrisv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvbxkwsz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3jtkfetbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovcsxebm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hpdenaqn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jbdzydts.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fceknrqa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xenxpnqw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cjjseboy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mavpexxn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ocfqqwil.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjyyrdv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3nmyuocez.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cneyptgf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbdntgb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nimkasqu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ypkcbheg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qofeklco.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3atsejqyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dcwzewue.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mzlkognw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sfrxpifo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qnxbaswq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3onyxrzzt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3chrlajok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3iaxtrmba.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hciyyoro.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnuoxttl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3sjsvmmfm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzrxomvl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqjqjivb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rbausqtx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nnsrsxep.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3epnuuvbn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjohqef.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ihchsoay.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kemnuujh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3csuoagzz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3rdmrxxuc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jsacupqy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3irsrpnjb.html


<!-- 参考信息 -->