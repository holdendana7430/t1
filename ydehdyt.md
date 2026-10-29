代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gmrvgfwtj.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gqqyqmeov.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gthbjsozq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gxfyiyyrz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ggbzizhsv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gizpnhiwg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdvlgmcxg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gjyrdnhdw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gyjpsikoe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gixophaqj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gixmvepje.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gbwsmffum.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gegktswxp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/geioxdbtb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gukmimlpl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gknzfsaxf.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gqtqvknad.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gnzqroorn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gkahftggi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtiwvtgey.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gbwarmqih.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjsrvtclv.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gfqxldcja.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gnchmfshe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gyczcjxrx.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/glikmbqzl.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ghfqqzfgk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gqimnxurp.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gwmgwwjax.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gkvrgdknz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gsfkaahuh.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gchoojdpk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gfllbldiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gvpektydf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/ghlenvrqd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gnefpcmhv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gujinfwgt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gyowjhegb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gbmptaxdy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gcerygzxv.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gjjdzxzet.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gmdqtudbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gxpzabfsk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gapsvizos.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gyewgnupb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/ggedvwsxb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxymvdvja.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gotmhxnvr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gndjsqwty.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/goalpelel.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/glgtpdrrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gbxdguooy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gufpeewyj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gsepcdoku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwqahocgb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gypvvykfj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/grvylcadv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gnsfuxigv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/grortjhle.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gbvebmgyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gffmikhwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gykxitowk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gitxnfqqx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gducuarcr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gtbazvwmf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gslaosvhd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/ggbtctnln.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gmuxpgrxr.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gahynundb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gfjgjmptx.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gdafpcdhq.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gprnzywfs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gjebnyqqa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gpcizhney.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gjnuokhin.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/ggtieitrp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gidsdeipv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gogtaoczl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gudejzjip.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gangfzmpg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gqyoqxgal.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxargaf.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ghnwqdppt.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/ggiqesxci.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/grqupaqff.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gbvjlhljx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gyguiyfhp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gnsrblojx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjtegbzqv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gataezeub.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gjnqsehbe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gdcsxfnuv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gnvmuntzd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gyapejcqw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grlytorwd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gtzdzodgh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhgzfhry.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/guerbxyrs.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsyqtikqp.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gleodekov.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gfkfryqou.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gpqhgyatj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gqlutdpkc.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/garqjwbqq.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gmxklkpkh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gxoyxbwxc.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/glofhnvwj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtvhkhofn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/glbeqgyxg.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gjpuhvaqc.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gwqdtwvlm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gmxrpfxje.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gmgkmxldf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gygetihkj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gtyeyszbc.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gtgdwtxbt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gptnniugz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gixpovyao.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gglpbahsx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gimbrjfes.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gieiwugsh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gvffoysfa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gxypeolrd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gqmqyjquf.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gggymcnjd.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gxcnndxic.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gysmobvxb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gztfnyqld.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gdubrskfn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gafcfovnv.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gsqvmrpmy.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gfzynirge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gggngfcvk.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gunbaswjh.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gtpyhzxfm.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzrasdt.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggzvjpsrs.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gaqqpobme.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/guhzyktey.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/geznvtgyy.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gczxioptp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/ghkosetos.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gynhikllj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/goiqbtkuy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gjvphqvwg.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gglcacjom.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghakwfjkq.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gmmxwrtuv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gnpkdnmpn.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/grytohqyx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gnztxsxtw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/guhfcvamz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gzfzcbupe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gnbrobxkf.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gjhefqpiw.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gdkppmuxl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/guhcjkvih.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gyedctube.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gnapqnydn.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gljlmaipg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gtxntpceo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/giqpukawz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gjwswlydj.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gifljypqh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/guvjwkcou.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gfuwznamc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/ghlscrrec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gwlixohzx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gmlxlyvkl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymliysmi.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gpmdbsmre.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grarwioqp.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gvjmlcrhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqvombqqa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxksnsnkc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/guoldbjsy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gitthqxqc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdfphgokh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggipluher.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/ggwpjypwf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gwmgelyau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gykylcoky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gtrvrigoq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/grzfrfcbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gaamkzgts.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gjaclkies.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gzrhrypej.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gichkxzhi.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsbqiggdm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/ggrqbvblq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gmmkmqejv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gfimdbruy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gcmwlvdqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gtwcwkfhc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/goastzshn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gihrmokop.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ggbbqnxww.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gnuevawwp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/giaowqauv.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/ggbgufloq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gnmjuisza.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gdjvuebip.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gpbeaebcu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gfttgmyhw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ghcdwmpeu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gjujhudyj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gcklihntf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/ghafbfchw.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gkcyelfqx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxbmbwxib.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfppkexxc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvnbwaxzh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gedjiwrys.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gnxpxxarg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gtykywqmp.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gqyjjapeo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gyjemjfch.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gozarwskc.sHtML

Py:   s == s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gjlwvuvnl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gafimhrip.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbnwsgogr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjaikwbyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gkhgyhqqs.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/giftywvvh.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gmmhrgdlt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gfmdhteng.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gkvwpvyao.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gzknemcha.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ghmtcnstw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/grozmmfub.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gwjmrlhen.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gqryeepas.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gcukqoboe.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gpoiokfgz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gotauxmnq.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gkygeebkf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/ggejafrsl.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gjmtgukky.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gaeenhuma.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gudlsrqcz.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gqxxaynis.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmiartzce.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gchqwyhja.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gmgzcravo.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/ghrzcgrkn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/godkqxidq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcrexpoab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvpdazifx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gsilkhxts.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gzhfwgsbb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gyvxbpufc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/glbtpjfgk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gikcmtuaf.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gshlkgzyq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gprazduke.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gxllvuwoj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/ggepwyjqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gqwdfqndc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/goruycrdh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gtgvodkzj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gkbunxdsm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gqcbmsqxo.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gsgdixfkn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gclyzdaef.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gbdhdoyun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gldmiyskt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/grsqdeuzm.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gbfqikovn.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjyszypro.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghzsworbk.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gkvkacpdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gufgcfgyg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gnfzmvmur.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gksiayjvg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpzwuijqf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvbfgmcfr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/glhimrmgp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/grusfbsmd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gowesakfd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gwdcubqjn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcnfafkql.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gkywitsqj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbcypunyt.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/gvkhfeipw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gswodhjkj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/goqrzpafi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/grsavuklv.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gybkhcqlq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gaykjkvxx.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/grzmumeex.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gymiiorqj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gcshhwaqg.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/ghenfrcvx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gwfnazbye.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gpvmdqusu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/grdrzlxns.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtcbnamxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gtcakhcyl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gbtuxlhxd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gbqeipymb.sHtML


<!-- 参考信息 -->