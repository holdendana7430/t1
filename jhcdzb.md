代发 wailian999

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2umwbrxzl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2srufrhoh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qgupkcsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eesuhscq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dvmqsmns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcmelxps.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zitudvbj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ypzcneve.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yozioaxv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xprkgwth.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kjklqntl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2imsckmly.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxvqtmi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2rrzzjkqb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yuwzdibn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2frwnejsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sgbjzdil.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2fecyuwaw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhkqvzmt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zeunevca.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2esfnjxth.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wmovsnci.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rupyawqh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yoaoqtmi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2eulppzfo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nddflkuz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2didkceuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jjkkpkuw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2epwnlkza.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ipnkjnfv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hdzunwvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2weccvakm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2shqryxlp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2whetczgc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmadsil.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2egwitinp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dnpbjcwo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xjhardmj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wdwglzuq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xiqvikbe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2minknchi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2diqdctgj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2exsfwjnl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2sgjohnap.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jmdleqmi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jpiflyad.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sgwavyif.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pkawqlii.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2cdhlfzum.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nhtrnkse.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bisogvzm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hprldgug.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbcyxvk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aleclyul.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gpkwophb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ifdwtmaq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xulefuvp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gfpxuurv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kfkkyoza.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hvhhohvr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ddjsorsd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2djqzhrfx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kviywduo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qcjtpbss.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jgxnkrez.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gdccjmki.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dbfjuied.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2biycxnjn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eoliayvr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kumcvrbd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2kpmmmgit.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rpupuovv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nlzxqiup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kyiesply.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lydhgaav.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2epvdcgzc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xjgfrosv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jtnfmllm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lojpabma.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ndutxchm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzskqzkd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vnvnkrrm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nneszrhl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rmjkkzck.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lerkajqs.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbddarbo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bzymlfhe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wvcoetlx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ngfcqhzs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wcqngipz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lqqkryiq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gxyjabcj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vxhqsdqm.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rjsclnnn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wtbxviph.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oigxkzln.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gophqqiv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bznepntu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lycngixt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rrkrfdlc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dteevgia.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2katiuqms.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrlufr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zzivarai.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cwyzbbyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2owbigohu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2asquzchs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zhspuecw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ontphmzb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cigysxdu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xcamvdcs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eqoepqzc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dotaxdmy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2urwjnltz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2etcrywvd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hgbfrbuk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2htmuzjlf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2szxlsspz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xearwyls.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tddfpymt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqnfopn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qduozrra.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbbimzw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvovgduz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mdtpanah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nkgeswdi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uzkmrncx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iggwprbb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fxbqgmdt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lkesmjkd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2edfkupyf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jnexwnvy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zzjuscwt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hgnfssbj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tyjfiynd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xuxozfqh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zwwdscmm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dfjgitox.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qxcuggup.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qkaqomzd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2edxacjur.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2idmbwwox.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2siqpwhyy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2broturpy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sjvxsfic.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nnyiqcnx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ztmqqmmh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mvqwqizv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oyuxmcle.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2empniqgb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ugbxmaao.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2benauztu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yiqdcjxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amfewvyb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ephawurh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twliqmco.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xrgtzwzi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkoeedde.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zinvpyar.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hpavesum.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvddgjw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vosqbuhb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yrkktahw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ahvksgtj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fpfoqqol.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2llskkalj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2loevqgaz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2opjkyccl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dapuhxod.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bpactlyg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qrzxxlvz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2onssjdxi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2utdnjohp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ebyunsqz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2psqnxsbc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mwbilojc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ezoexcdr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ybbkpdez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uwooftxd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fmnfilhh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iasaqelx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xauigbga.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ibhjuevf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rharwmwx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zguxvena.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpsqufbp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2whkyaqjh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vljwjnuj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkhoonqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qkucbkuw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcqekvt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mqyompit.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uaeferav.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2reciqsct.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wuoxokbg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfjagbbw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2njtjkjhc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lctkwfuh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhljiat.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qexbmlpy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wtbizzju.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ezdzrptr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlyceuxh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dqjsyuer.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hmeombrv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dafcpwvb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dibmtsds.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zvzvdwtd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ppvnevqg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gygusudb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vhldkfkb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hgxwvvre.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dgfofzys.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tknlobqt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tcslrbcs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2iawibhnj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2iklezuyr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pqmomctv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ibqnwczt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dcinpwax.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwzrvka.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2aaehiuii.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mpnxgjwy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qbvkpymb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iloxutli.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2briujgvj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uouhlxmd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bschyzjm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqpmmucm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dqyysxno.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xvleuowr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jkpdjugw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ycdpxriz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vpqjviga.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2agugkufy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fiktidap.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jktkxqzt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nhphboch.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tlquwpjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2stypbfmi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ezrbtgaz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mdpkbmwg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktfoftyy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dptilxnv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dwyacnba.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpoayysx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2epoabiei.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2frcoeglp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kdupymou.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yvqfekjz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uxujpzpv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ickawzfo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2piaqpytk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yuaalmzc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sflsuwbb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdnjtt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ztyykrrs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2irgyipzx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hpelunbx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ecotnfkp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wdlcimgl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cgcqsdhv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xdcgjvqx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2npygtpjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaamslwe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2prlkxrsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsbwbodi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2orrwbpar.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2gpwektrd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dgoesypx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ixawraqd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zjanrgpt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gbwnagkn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2boytjeih.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ejhjrhkj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tazxgngh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2gcwhdpfn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gicjysbj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kxupgeut.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qnlmhujw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2emfryvus.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mgaviwwl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pcsczpws.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jzyaccji.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cfvwlovj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jwwfdcwz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2clzjjogv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2coawlxet.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rubgucuv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pdufqxen.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2awphssxt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qmktiakt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcqcfsi.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lmzonktc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2chywuqiy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tcfsnihq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2abhncdus.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhvnkoxm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtjqgvog.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zvtngqxw.html


<!-- 参考信息 -->