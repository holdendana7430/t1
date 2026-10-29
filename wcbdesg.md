代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gptaocqkw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvpqqygxq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gwjcjqjyj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gjodbjwzd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/goixbszpe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gjzsbqlyn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gwwgikdng.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gbaaedkqj.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gklxjrqmi.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gptadajpk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/geuzkokka.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnqjmfuui.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gdcpglisg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gildkwutq.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/grcdlnkgr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gxlvsffvg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gcqaxtmbg.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/glggaxzum.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gktpxsiug.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/grnjytlhb.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gertzhuex.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ghhremtlu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gaumfvjju.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gvjqunhpw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gtpgxydsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gicqknetf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gjtkvdkiz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gamumnlbs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gjhrsujcf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gribobvrr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gyrqdwpjs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gilbjvsqh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gmqclgzmu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gpvujwoej.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gtumsawrc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gsojhokyq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/grznwbxzo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gbgothhku.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gypbrfaox.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gbdcldchg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gtamxxvhm.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gqgxoyhgp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gojrigcwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gaqhtcrwt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gtxjctokz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gagxzdfbk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gntbwydhv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ghskajawv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/goubxseob.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gjgjcczvc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gvyxnihih.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gzazxstns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gejnxcusd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gyyslcxlr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gioqywcpn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gzocdfgej.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gioixjjxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/geutjwiar.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/giecubirp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gukazmdrr.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gchgkzldk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gpooxodpw.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gdepwaqkl.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gaaancufc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gkceiyhla.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/giyjmgplk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/grihsemyi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/giprshxzy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/ghuurdkgf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gbczmqdtn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gaslhhelb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/guwxmqnbh.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gdejvxnxz.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gejyaatnu.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gtldhyber.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/garjnvuro.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gdragunek.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdxhbgd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gnkeevvlh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gaebwvtck.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggwqinfve.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwxkorpck.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gbwzxnnuj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gcugihebq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gidioxmag.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/goxrylajf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvrvpelfa.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/grbidjdlz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcmplgzaf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gjahhriih.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gkjgbcnak.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gcrvuqphj.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gtxcgtzjw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gffmwjstd.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gsarffvge.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gihklpaay.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmsofrczo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gwicvacuz.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gyvxbamqa.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/girfspkte.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gjbgmoded.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gxxksgyrv.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gbhaqcwph.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gqcwawkit.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gjafkohbw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gkhyjewbn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gtgloytux.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/geqwxpzet.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gtjzwhcou.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gkzcsjnfm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gcvzjlzvc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/guvfpdsnq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gsrbezqqu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gemjphluq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gpkllhzcb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/grvgsykli.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gdrwhduan.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gjilrjlum.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/guoznfvhh.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvpxiixmq.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/goxybvuer.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gjheximbc.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/ggvjloplu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gftxsgdlx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gbatcyeme.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gupztrhom.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/grtdlluin.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gjuwcghfz.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzjdjplea.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gztlnxcfa.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/grlalnfyj.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/goilenslx.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/ghxoohllr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gnoqqkdve.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gdimtlqke.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gfmgqbhid.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gpfsjmqop.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gmmrojqxh.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gqivsldmu.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gmyyrjswg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gjigrerfu.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gsouvtebn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/ghouzaluw.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gmmbpmhah.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gwoecellv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gmvbjxqjy.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/goneklbxf.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxeblwxum.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gihmxbnzv.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/ggldsfvrp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gptqabihn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/grfwvtfnd.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gyfbmvbvc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gpcksxpip.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gmarbqtox.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gurscfxts.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/grwnqvcvk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gfqkvenzy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gvagqmgkr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ggbbwxcov.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gacbkzqns.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnppigusq.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gvpslgxcp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guhnrmuxr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gocivtwbz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/goicugjqk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwxdnntdf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gdhqjirzz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtihjmyav.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghlloenfs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwsdzvdkw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/glcdpvmzj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtuthshaz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/glaffzpvr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/goqpdcuyi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gjxhsnshh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gpzokjltp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gxdgyoogu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gprkozpic.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gpvukntwi.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ggoietwel.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gdbuhgjtm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gucisjiwl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gqrfeezfg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/grrnogjyq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmtlvnbgt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gaionzejl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/grytemrwr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gojvrnyut.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gzgcesgza.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gywluqvma.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gpnncujed.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/garryljzx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdbvunuhh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gevbzjeba.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gzrcyjvcz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gbdfouqee.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gxmxefaaf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gucvfkopc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxyutrtby.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gflwzuyzm.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gjugkvurm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gabtxalgu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/giibmhdhs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gnnqqymns.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gxhhkasrm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gedpsayth.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/ggbfvxmbk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gsbqieaju.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gbvxfhxtw.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gpuqkyaqp.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqpcgfuvv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ggedycbej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gfaihizlf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gjomozuum.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gwefghqdr.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/geonzatzo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gbygtbzjj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gnowovvuq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/glqlxarmp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gwmxdpiiz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gjabwwdkz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gbmfkpjjy.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gnfiltwlb.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gdkcifrcn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/ggfyrdlqv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gcpzwroot.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gzzwturnh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gdoldzfrz.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gbdbrlrak.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxdezfyck.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/guttvzwus.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/guqyhhpev.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gachrnetw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/glnwsovxw.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gxkyebtes.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gxdeeevzq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gmcojnxna.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gorbtfedi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gntuzsbwu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gxtstsfvx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gmwkxgymu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gtnthsbfz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gexueqhve.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gmzhlzhpu.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/grixlgrzo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gstpkefjn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gtpcmwgtp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/ggdsumyqk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gjnteexsv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gblcfwwtb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gzmbpgylv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gpgjxahal.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gpijmueod.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyyfhcqku.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gjnwfqtet.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gqamjsnnn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gqrbczjym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gnwgggjmo.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqtdnlrmk.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/grolqgwva.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gbsygppbe.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ghvupcniq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gjigweglu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gxjbnkvka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gdmvlopuc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvbcjlcex.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gxdadshaj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gjbaziqzq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gamjmmtjy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gwwemxfrq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gwnvqaoer.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggnxqvxfr.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gnpthmcdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwnwoydqk.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gszlanrra.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/guhkjwbfg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gxwojyrab.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gnzbwvker.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gftdxceuc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ghywjibdg.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gwurasalr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gqbdolvce.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gcsmtyciw.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/glmmpufco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gpozimypa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gsauqfdgd.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gddbehiqq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gofnespmt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/grosajdqo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/ghafagmdi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gruhsbkvy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gwolbkiug.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gbfmuyhit.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gjhuvhyji.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gihdhnocg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gppllmczw.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gbkzlprfp.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/guxjnjwvo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxzupkxpg.sHtML


<!-- 参考信息 -->