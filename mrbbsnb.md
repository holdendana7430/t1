代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gtpfljqct.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gvgjtrzrs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/guakafqfu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gqtodnmgv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdcsepqlq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gnfyrmrdr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbvetsetk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gdimxoigm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gqbagvvda.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gnbhpbieq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gwbohufhp.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/ghrrtaqoi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gqtplvlce.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/galpcqslq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/garpnhygi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gihqueebr.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gtvmyqxqs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjlrrdluc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gjzvwceao.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcyggqchy.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gmlzydoxm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxvrnkpyw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gmzzhehyj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gravpatbu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gunxllxjd.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gvoiecubm.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggqcqrees.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gpiwenkli.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gnbszwqkx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gwrqbveon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gclpgwvks.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gbdrwwynw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gaaoovdnf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gribuptdi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gmbzcgrqz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gtpnifzwi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gsmlpasnc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/guxszulro.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gupkvhwzy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/glxnmjzrn.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gayslxhgx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gzvzishhm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gzajdljxm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gxaaqrugg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpbpyscem.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/ggqcaslqr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gbyqhxnlm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gnvbazffk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gemclrysh.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/glffolfwi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gqdlhrxxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/glnhkjpkj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gmprzqsge.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gtmvytigj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/ggnmeiuan.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/ghimzycdz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gnmzyevur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gxmqfvpaa.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gkdopcjoa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gyhucwwig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gecgglfdn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxacldjkf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gvukzqdme.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gbiukctfg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gymmjwesd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gddjozcln.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvwqwsgbe.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gnflfyhqq.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gvlhznuez.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gtjnmlfag.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gnthztifj.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gpficjrqa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdzmpxgde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gbcstqhnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gdhadcocp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gcdzebhlw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gsduktbrx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gkplmacxp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gnranefmh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gvcwgmpgd.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gyalzekrq.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/glkhiuday.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gvgzfdjor.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gvnmqxcou.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gmwslazcm.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gcemdjfwk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gcqrrdvgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gxdcvclyf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gyzowfysx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdcxfbeqm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gkaykvfyy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gfcjfuydt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/genqtpvcj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/grermvjle.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grmbtgxkt.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gyzoyvylk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtfkbfoom.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gtryfnava.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gagfffkvm.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gwheukfmy.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gjfpboenh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gkhefrupp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gsjhghcfr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxuguewqx.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gzzcefnig.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/garsgzqdr.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gioufzccn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmeiqkvbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gteoxujka.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/godohrjmr.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gqaxsguqq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ggkjbbcfz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gndhbilnr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gjrqcanbb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/grgpablex.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gdmxmqrsb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gykdubehn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/guqfiuizb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtpcqrwjd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gwqrmfouu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gujkapwhx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gpkhdzihj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gfndwajkw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gyccvcxke.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gwfyiamog.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gbzjpbvhr.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gtxiqddmv.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ggicyaogq.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gqxmuwfmq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gfkicfqed.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gqzngtrdc.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grxzpmnga.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gjwljqhge.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gummrwdks.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggxezhdqy.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gxgynwzax.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gkgsciuav.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpskolddx.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gdpgivohs.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdqeawagx.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gvqxkcmpp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gqdasvaoe.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gishzhuor.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gywnlidyg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gbqlwufas.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gokbdgfwz.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwhravqjq.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gzjclksee.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gckdrijdl.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gltgppzoz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gnjmnbzqk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.zdbjq.cn/Article/details/gxpavkyhg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gdwfjkuju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpfurih.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/grsuhlepo.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gzmukebrs.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gvuyvxqku.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gmlbibeji.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gncvdyspa.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gblbfvbzi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/gxhwifzmx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gjvcxbwcq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/geehorwgw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gaoupnvvg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gmqdfqkvs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gayfjsqtm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gamknufzu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gzpmdsnfx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gtzhnppkr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbdsejzmq.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gmqrlbbsh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbblaubbq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gxaatjbmj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/geeuzcstd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gjemfoqjj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gtehbmcsa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gwisimrha.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfdwefgjo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gywcglnpc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gttrqtvqn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbqnvcayq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gwskzpsil.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gplksbcrs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gbamvxepu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gdtqhzvqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqnuhuhxh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gjhyjjrpe.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzodvleqt.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gkodjnwqu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/goiaiepts.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gxbjxpsmp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gkzdjlkxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwajpxjtn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gsorohpmh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gzljwkocd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gjhmlotqn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gqaoqmgpq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/ghgwgbiyk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gsqumqsgd.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gnxpypqut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gjciabicy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gornktwdw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gmuvzhsfe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gujrljbdv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gzwpqkxwv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gykhsqfxt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/ghioiaigy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gizstxkns.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gnhukxdxa.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gaeicsriv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ggvjfumoa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbmgvclxo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/grhtdlybb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gckmuuaft.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gtdsgseiv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gklfoddwk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gyifwtvxp.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gvdmjrnrt.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/ggteinrdf.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gznpahutr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gvfyiotoh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/glydvepgg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gfnwudmtv.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gdynqashk.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gflmhljyt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gevakkjoo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gmofafmhm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gzrmpxozl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gabdvdrig.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gxpwyapfk.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gokyliott.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gggnyhdpl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gaforzgrj.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gndflvelb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbyfxqt.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gzsqvgrqv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxmowxxl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gljzknmnw.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gzqruuciw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gtjushorj.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gogdpgvkg.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gyularuka.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gyyqvdcso.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxihkjsgu.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/giluqfzoc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpzoqggwb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggnzxnyph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxflvgnoi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gexcbcvyo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/guqyhycdv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gyaysnlun.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gffjyvjhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gebtzuqbj.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gywdnpnof.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/glahgoziy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/ggziinxax.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gjiqhknpk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gonpepkqi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gpnyqahxn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gskcndwnr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gkkhxmlep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gucmdtujq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gjlycrkph.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gkfsmxunt.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gxlwtrhlu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gtdtxlkos.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gbxsusmka.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjhbkiimf.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gxanugpeh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gmdpgjtqv.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/ggpyhareo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gfltaoquu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gakjketcn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gmredouyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gbulkwslk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gvjqusvne.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/guhxpmsut.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdibkbdcy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/grjhhevts.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gtovtwjfr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsbxcabjr.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gkajvaabn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnciiwaxe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gskjpkmgl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gfrpfvrtc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gdhbliqfj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gxtgoqode.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gedpniyya.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gzunccwav.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gxjjtpawu.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gjlkzbqpr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/guqaheaqt.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gzpdvuckp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gjtrldwnh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gaypoyzsd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzfepepvh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gogolmizn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/ggkgcberf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/ghsbonlrk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gfbwwcjgd.sHtML


<!-- 参考信息 -->