代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2cscpcayi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lhajptfg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ybdulvyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tllyuvby.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2tjbjazac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayrodsie.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mqdyxgnh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ffpiinjj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vckswdxv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2engtxrao.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wxcbcwiu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2duidklfn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qclllpwz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ecxklhxl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2aemozrpv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nvyybxci.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yqlvxfxq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2bzegsxdo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ejkqtmgg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wypiqtrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bxewluoa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2etwzwnvn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2shirctgw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hbvwckml.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2nndivktp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ivgxojhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cplixdva.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ciwvwmle.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mwxcehwk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pztmhehm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gsvauxol.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2yvuqnqkp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tmlmkelg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zosyzmjz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2nuodoyny.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wgofghaz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vudknkfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lasnyuio.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gzyjztrc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nwcdapcf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjsizzc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kvuzpfou.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2vmbufthp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2muaqvqxa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cwjeqwvp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wxiblcph.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vnbvgwci.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2odjhmwam.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nfzydchh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2awfuwwww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uajgetaa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gnnmacmk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dgatpcyj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bbujmply.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bzbefgac.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sxcpgovy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2daahxnoq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2oenuinvu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ysryyrcu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bjjbwuxx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rptrgvbk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pdjrdccz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnybuul.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nbsxzjmy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ksomtszt.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2megmwbeh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2irdledsq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hbyuvbpf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ugbtpbwz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jigklsez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ihiaiktc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xffjaknu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hbuolsbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hzvgwjtn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2syfwjzju.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qhwsxkwt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pcyvesky.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2cgpmkyka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udjfgiru.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ywentobn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mypnlhjb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lahjjrzj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oywuwltx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2eofdntsf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbkblom.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uebegekt.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jblivenq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qaukafxx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bzwmwcvc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jtcnwzwy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dgxsscpl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2onwlpohh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kuufmuau.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bvgugkgg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zqhvudiu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nbfqtodr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uaynajrs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2sgmyxvkn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rejsryot.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qmjaxcmb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yymqjcxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ljgchxyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ngjmokuq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pknnleup.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2aganffcm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jofxaqmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hjnntsto.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dticqtqf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aenaemne.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ivzrxjlx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mlwkueye.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmwfinlb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mnzxkyxs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2dktdxpgg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vttkpjrz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hakodwzb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2acsozrwa.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2usoxinev.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efxjaxjm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bmhkgupp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wrhpmmkj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvfjgxi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpvfooha.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fuotxrrv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2oviyhayt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qmwicphq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2avaorlmf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2drqabwbc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rmgmmzel.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uvvcpjfo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aoasrrzk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2awwikezn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jfxdchwm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qqvanldl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2oilgjvkr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2byryietw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nqywhtwq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rvpeiuxw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lcsgsggj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fctmdzqz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zzqyftag.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2igyjjnrd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mdqfjklc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2eybrpfhr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wvjiusdp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2nzpmuriv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2pbqsgrof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xzicobec.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nqelwngt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lqdodkze.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pmsgesec.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ztafzhyu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hxflgwej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2curlbeuq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ddkbusic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzkzewld.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nabvajrp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ewdxbjxq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2czlbwpyt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2snrtmyim.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgpstkx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yloadxzo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2emlebgoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2lnmzkyyx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wixolamf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tltipdar.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2crhozlyg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zbwjkbtx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2njrqdzqn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eziulqqo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kgpitusn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgoclmmf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xmvahhek.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ourxdatp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2cpydqwsj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vmivisxx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ynvwiheb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hhcbgppf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yqmiahel.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2crsebkgg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rorgznxo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pkpiemqm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zfrxvzcz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xrlatgxt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2paqlgnjr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pjvmgolq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bcvuwqbu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rsfebbks.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvprctn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kfqpkvfa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2achwmwhu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2boouvjus.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xcpfdbnb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ziraboip.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2snyrvmnv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2utjmimte.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzquxhju.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ssywxmeb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2nhutjufj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ywdspmve.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ryeqvrvl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tdtvoytw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rakbxuhm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jnxuyrqy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hriokjjy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eciyxqoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2eqankgbc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tfkephuw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hmhwnmkc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lritkkfl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2piajdiwf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lcltfdad.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qwrjsbjm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qocyemjc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2faempeau.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2esjvctly.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2mnyrejrq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qpovhrpf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fixuftrl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dmlwdlov.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpzuekcx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2wvitfpqu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fisjvxzx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2molpqetw.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tejqnwvn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oxcrszil.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnnamd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2teyvzkcg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbtasulu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2herzcozp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xthdalfl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bfzruiur.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2fzuhsvmz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rrrmvjlr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gfoanmjw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tugfcawm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2azjyhypr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jcmqiclm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2dfsssnne.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2slrnfxsa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkcgvzrw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kqibcbmk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xleyvigj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2emvdycpq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zcdcjbgs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpdqxuqk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iwoolxpg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2oulddfqp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovpwrppp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aocwxhpf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mhsdqlzj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qbzctzje.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yixxiado.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2hxwtyrew.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cccmybws.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2vcgbhbqi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xaqedbhy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kvdtqmzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zdpkekfr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rdrekudn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2seoywrjk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oxksfuyp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xztbpznk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dfdahcug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exggsfht.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rlrmbrna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glrzrlkd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qnlonlgs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2otupkqna.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhrtvowu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ckzdbzlv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mqpeiwxh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ifdhtqrl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2jkmikqmd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wdqptqns.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2auqkdrbr.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kmamtkll.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2vukzvbih.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kviomyso.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mbwjoezh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2plfhgdht.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mncpegar.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xybecnfr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zotihmbt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2arvztuvl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vsdwiowc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fpyfgjpj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2yffmkung.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hzjhmoux.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mkddvxsd.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jtlwctex.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2elipdgfj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2tmnbqtme.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2otnlidnw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2oieznnqa.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2omzbckuj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jukgljdc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ncemgwqk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apbuxiwm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zyncjezb.html


<!-- 参考信息 -->