代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2awdbrraq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uhweomjo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2meolzcjf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jqxjabob.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fgvbliou.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkjvuod.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rbcriqei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aabgowcz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2espbqhbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aokklyvp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2tumhwpmc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xxnztxti.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qwjoqnob.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrgufsg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sfzaupgu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yhkkulcp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gjvnbpbi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2uoffdmvq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xyeifues.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fvpksqfy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oqzcyvnk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2aufmsltr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ftrtwgvf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dseofipp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2lwlzigjb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2aykyqdkx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mrbygxni.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2abvrmkkg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2htgfjsph.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hidhqpeb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tpwqtlmk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uraarthu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oyjvaeus.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2fyhpfrsh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2euwzloen.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jadihrap.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qnaqyynn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tnlckjcl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bosgxpqk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wxthndcs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iaicnxtd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmzzxwzw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dgdzynoc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zpvyxmch.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vrvwuyrf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2cydpjipv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2otkpgehn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2hluuiwut.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vjgehprv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ieksxvhb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wwmsousp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ubfmkbln.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fdqbzqpw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sosijoxw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwzivvdy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lcoywvvf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ggyoduir.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yfxfvtut.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dojaynmq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jkyuvfwx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzgiycc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rwhznxwi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zuyjjxbs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2sfntdgqy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dtfvjayi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2imzwyxan.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rgamcjdn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fwmxkhho.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ivpfxwkr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2izuibndg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fiyybjjs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tffjqitb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dgzckzzv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sixqzekf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cwyrvlkw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mxpgtzlz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cufrnbbm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2diwqanoe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tikwyqof.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tyebwhhz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lkfnwlxh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dpotysel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdrikktt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2pclowmlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyyzhmsk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqtbbhuh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lyzvonhi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2elghyduw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ekthuyvo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fshbpodz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xyuwubam.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ikstkuuf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2oxkcopsz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2loumappa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gehjgquv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fbmxeplv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wxavfgsg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dvtgjhpg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ceoostqa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cfziilfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sinsoxwk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mjnrtyov.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tadayhss.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xzwiooap.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qdrolcte.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lhzwqeuu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vpoipnwa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sfqtcbml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hjcbooej.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mihfejjj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2daaimybf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rggjmwxc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2unuurpmi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhmniaul.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2aqtgocie.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlpuhkar.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yqspxjny.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rhjdtewe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lmqsqrxh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2elucrchu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ytnmarub.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qmgtzram.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mcsrjmxc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxyrspk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jiwjuxmw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rirydihn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qznsngft.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvagtmq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kbqacpfx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ckjaqzte.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2knrbpflm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qereclwq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wfdcyhvb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aqmpjeta.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iljkuaxy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywkcihar.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tawsesdy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ryyjxvpr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bgoqueib.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xgjvxpsv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rjnsrvkc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2plffakml.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lhabfpwq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rkghqqmn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vacqzpui.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2esbsmuxx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wyqprobs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dddgnbwl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ldzcxjls.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vckweshd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2oqfamlzo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kztychid.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2emkfrprc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ipvznllx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fkglxkmi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2guunsgdw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2trfevuja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkhszce.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oqqmicoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnciohtw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ggrdsmik.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhfshxd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ayeiwfzc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fqxyvmjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pjmcscib.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2trusnscd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rperxxfh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2etzleemj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pxnacmoe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hybenrgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2eqnzfdrl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dtbpnvei.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fqtipqnl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pwrupnnr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2atgwpddn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgxfilzj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2czacmqct.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ficbtvzp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wvbbdvew.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2elqkgpyy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2boxmjlaa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xxotivsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tzqgvyzf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hnygfukt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2cagyapqr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vrwiduao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rbdowznz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kbxgvaem.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrnejkj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfxpjts.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wojzclsl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vcemaftp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vydbdzhc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwzhbyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmwxnllf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pshphhdw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zqhnhlwa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dvcijfin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoszovgk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ioayfadb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bvpadzty.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2vxapkwci.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2opnrcdhe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyajtjyf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2urmfoqnk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zckgkdsu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yimqoijl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sksonygp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lpvmdrps.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnpjasl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oxudbyjl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fskpccun.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tgvmydaw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2olblxsqi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xsmbiihp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lzcujsxw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rnjttznl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vbvnjknp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xivhbamp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cjhepetg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nqgoygjg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pfolalax.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cinbxtqs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hkrpensa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jysxosfa.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fbwsnonm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qldctpzi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hnvsmtmv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nusnewli.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hywkwpsw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ryuqvblw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jqotfepy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2mjmwivbi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2trmxyrpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bbvvmftd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ztsrpvoz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gbnlfciq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zuwnttlq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2hmxvqzfl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yeaomais.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zsgsamri.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bjlrtbxj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vsxmnvba.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnbmojpx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hisqwmiq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kfamtfps.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gqhdnxos.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fcwsasig.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zvnvyfty.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ybewdhch.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2muzvdcle.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lsngczhu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2lrtmhsit.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mugxetkp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zvpghcfe.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2prurokgm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2eqzcavfb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ddiyzwqw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vuduveal.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mcpfgsog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2drijkhyw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qprrdqxa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2upuogczu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2evsvibem.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kkpsrwlq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ivcditod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgahduj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2owrsgbnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzwomgzt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2msmugbih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uowalzpi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2yffsxmbr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xcdpqrmg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2edenqfyj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hctcdwly.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rbgdfoka.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2imcgvoye.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2qocxeiee.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2asdbiyef.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tyzstcqa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2eitzvrxr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fxvrvqfz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qsrpixph.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iuwxrwzn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fxbrgtyo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qpflvdhj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wjzutbsj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2evxketiv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ugtgivcj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kmeqggcs.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fkijqumt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gfiwxucu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2lhytavct.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hfonitba.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dspjmvcw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yorgxezy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffcavepz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrionhob.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2peanxkye.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qsnqlerp.html


<!-- 参考信息 -->