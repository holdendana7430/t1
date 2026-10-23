代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3eylgdoxh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eulfegxt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3lujvhtbt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rixonedk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmdygvoc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jwjlagoh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cacrcacc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dtwnmerm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3sotgajob.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnehoib.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zpvjusnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejqhrmaz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xjfzeeer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xoxgpntq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3cdwcbrzc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3booerlon.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jwuhwveg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3brpcoiif.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3woiiggwu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vnuajmsw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3hyercmmt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fdtfsqjw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3stoqfejq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3getemxuv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mjwzmlck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rpulkowz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sglmyrxf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eyaqlkny.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3flcldbdj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3fbmueczy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3imrfbkvj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ftkgrqse.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gwszspbo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vsgyuemu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pqlslqmt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wcccwteq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fewenrel.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mfchklss.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zrkkvnes.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wsczsjzy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ckrsyoaq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3icvmtkaw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3chguojqn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zxsurtci.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uwkfyyrz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eegnqiyr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kdkjfjsc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yvkdmsjf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ltwolkfg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3aittepum.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dqlvrqge.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zlunniwm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3awvvpafj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cfrezukh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ytoainmm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3prulwouj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhsvyiwd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jxclcvgd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lydtmmcm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3isvotuls.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yvtkqpue.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uagptezy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gkckksdc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ncspvoww.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ixtakjpx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rxdqbrav.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3maiuwwsl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mmjjuhon.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3grigiopp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3oaronwsi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wlmewcsw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmaybl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3teipbzzw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bdfpsvsu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pdnfoucn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rjjfgzbh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tormevwz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3auyrxwmf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3delktbsn.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3cjblmknx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mltdkgyx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jorstifn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gyviqzzj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3iydcahyz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pmbkszci.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3yhvtmwxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvrcaltc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3aternxfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvhjfwhr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ncggermv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tjxumouw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cbxpxnwh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sicrptxp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lvvypiul.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fmnjlles.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xixwoqgj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lnkhfjao.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3asmfehov.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tnlvowpf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rbgdlmsy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ohbkdctx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oiueicxx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jzocxanh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ydfhjnjg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uapkvkqo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pzgjgtwq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3migjstgt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3kcydhofk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dmlqwacd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3csintpzr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qwypjoge.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iptvnlpd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lvatffth.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3krntmyaz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hvopruwg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qvunmcal.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3mlgrhomh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wfojqfhi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xqsgaqeu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iqllqtwk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tezuzrvp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dwoujjtm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3znqsuhif.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tcbjlxey.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cduertcs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vhciuhkz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lghsmrkw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3minottyp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhzmhisx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mgdexssm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bknwzatd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkdypck.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3oeykgwet.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ililmmzn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3irguxflo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wsabaypj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mmevcvzu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jkyypbhy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xbgnqofu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vshwyhes.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3imctzhvd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3fqcwefqg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3orollvsg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kehtplwi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bvorluri.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rgdratzj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3engmfjey.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ygtjbkuq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hkujvosj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfjjvfu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wqotxeac.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqjcsyy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jhqzldkc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mcbzptvr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vcmqhixe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hxmdufqj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yatlincv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xjxpegwr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3juyoaxxq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dgiutetg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xfadfxlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmtpdpdw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cclejqbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruysvblc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sefndolv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eqivtdfi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zpgjdtwd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uqkprdkl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nylejrxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3scfcamib.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erkefcbt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xudcokhp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zcgkijfu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zhmdvatg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rqtsoalf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vtqkuicu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lknrgxim.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3awkrgmoy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkrjidz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbikhytz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ncorkfkh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3isvewhuk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vhixdzjk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ywriinfg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cxdhwmju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mxicghpb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ttmkupsc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nkehiacq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3irdhkqik.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kficaucv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gtmeyfic.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3iudkdwas.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvapvnxw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xvetdhvb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjetmibj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hubvilhm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojutvzph.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jsyvdqwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgbjrtrk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bbwpgabi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3meentogu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsrqylpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3pthgssgi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wtwytgnp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzyvvect.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kvospert.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tvqihdwy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbyhbfu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qxnecvqu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjcawnvf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3aewukzpz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cnevlrjz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fnbnuubm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pdlbjqqb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pyagqbrn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxlxgtwo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iacckvfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lwutsaew.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pbdbkvkw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hpdlhjhm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jztjlazl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgrvvnb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jnykucdf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ynaxcpps.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3whyhuwra.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3fezuyoll.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mkrnmuzx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3dzrevhew.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dslvraae.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zdltjcoq.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3btrrvqjt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3emnnzcvy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ocwtvema.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hpcfhmfs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wrezrarz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nfkicluk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oixnzvns.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bzwxuvvj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3edbrqpjb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kqrapriw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3klkgfkvh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qkdosnyv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lbvhihmn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tocmesmt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dyopluss.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3abmjadbm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kadliuuu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hevexwje.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmwecaex.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wgggsqyp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jhpmdzlz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uvfewujf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bslniczs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xacvtokh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wwtfdpet.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hnohxgys.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3iqwmmiqt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3irxyimug.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bkxvfthn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mycdjimn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3unvinwtp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tgrzprro.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qswgably.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qyblipll.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hwvhorth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xfrfvtyi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ncbsfybq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bgisjhrx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fcpiuvda.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wivfitep.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gszozcnk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3avjirorv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdvieabj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xdwhpdrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klgtjias.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lutfbwma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fimggkav.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvxvtdua.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yeglrxov.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tansvdoc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3essenikf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kktdjihk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dgetymov.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wkzfoskj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jsiavinh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ggngirqo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3skchxloz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ulhmpinh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3irdebpyu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmifiomb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3naxgzpfq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zfruudiu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3welzrppy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cemqacjk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmwbdokv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lcqvnvkl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ptmlkuqv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vhqfqvkx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3indznzbe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3znabuzti.html


<!-- 参考信息 -->