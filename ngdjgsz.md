代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gpfjhwyeb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gzzhqduvb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gtigtiwkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/golrryhdp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gfpkgcjab.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/guocryvvy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gaazvgvuv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gkgppgpda.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/grinyqnux.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gysfrllvs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/ghbynnpbd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/glgozpdxu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gngvlgses.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmjnzgwll.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gavyeljiw.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/ggyckpjia.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/ghisyzblj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gtbwfzyca.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gqhksrsau.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gogqzizgv.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gfnuujgvz.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/glwirjkjd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/guzrmgoqf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjecmcnqq.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gefuietee.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvpzvrtv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gdnztwtef.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/ghqafvpvt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gamyakokg.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/ghpdniogb.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gneyptivj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gmohuktqd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gncdumzok.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gofclguzf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gwlelzwge.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gzgbazkbu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gjhybbtif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gtueqknqw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gvcopngnt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gajpkkcig.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/govdrarou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gnudibutz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gpohtksxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gmsoufdpn.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gzrseanen.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gbnmehbho.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gscmnyfnd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gpzceijor.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gzzobuixk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gpyzynoyt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gvtzpsltd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gunyhksqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/giqvqipeb.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/ggjrsqugd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gocsqvqqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/grpkpgfai.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gmdnvmuvb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ggniaflta.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gdajnronf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/goekckase.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gnivxmlls.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gsdzqdhbj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gsfwiefle.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gukxqpdmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/ggmaayarl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gthkhaibx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/guxvpltjb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/gogmrilsr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gsstnkzuc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/giycorsqu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/garcbixdj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gxldupgws.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gohsmulqe.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gwzkepywe.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gavsbdttv.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gmfgcvbrp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/garawvlnc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gogcnliag.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gusagmjqj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grczahgnr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghogyhiza.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gsnzukwld.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/ggtxsxzkb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gsetdxzel.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gndetcdyg.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gxypimjlu.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/guykrwver.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gxmtsgfsv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzuaacexq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gdmlqcvvn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/giumlocsh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/ggzcofpxt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grlaueada.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gnuupjsln.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gmfcpjtus.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/glamxfjpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gwwktvlod.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/ghztontht.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnwpvymtl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gsemcpjyd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gukncneay.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gjwtkhpul.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gfjnpqcny.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/glpexnwxj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfiodhygv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gortofpny.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gtzdjslcc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gknnwqfkz.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gfrzsashe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gxjrxgooh.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/ghomofohn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gqaabeecx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gptdycyvb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gblfkokbu.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvaogezye.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdmoscsgm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfxcuyohn.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gesqacwsz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gahhfcqbp.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gouvmbtie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gfybstdih.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gdbyofgey.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwlvyipeg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/glnarmiof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gfkeshvah.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gwmpolotp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gvratshpg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gsdpgciro.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/glzfkvlnv.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gtlqrlnsp.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gvthfuoln.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gsglzbjsl.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gqhzavoqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gzupmavsm.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gfkpsxaud.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gwhnqepnw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gaerxlggu.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gvjhsbxzw.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghqucnqdv.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/ggddzjxke.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grxvxbjxt.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbjztjacz.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gkunnfgpr.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbjzikcob.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gxctrfetc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gfxsigaqe.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gwhwqlbnp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzitjyda.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfdmxvjwm.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gyedmakwm.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdqlxlloc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvxfmsrkg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gejdwvgyz.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gkbdocwll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/ggilvzocb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gxygqckre.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gcypuzxrh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/govjtjops.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/grxmyftbg.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gotuazmwt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gqtuqwfqm.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gvuwvbdhu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gwajshoxh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gzkkikylt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gvfcpomwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gtngesmje.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gsazbjrlv.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gdugoiduw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gunrxzvmk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gnvgkfgol.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gcaypkvar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gngqkixgu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gcxghcwge.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glustwujd.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gqskdtnvq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gobqpusam.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gbnmcoskr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gwwktmsth.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gzvinrxio.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gecjsaiel.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ghvtgypsg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gixjucaij.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gxrnvpnwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/goqgrpqop.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ggcbgjxeq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/ghpurgvyf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gpayjhdee.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gnjtprucs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gccccguqy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gvhvqbjxd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gdghcfwnr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gkknykhin.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gjfjyfnmq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/grszlznvq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gabwvlemd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gjtqgkidj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/grzpafelb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gbuskivuy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfojmliog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gqnpjzcxc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/giqdugetc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gqfifruzz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gromlmnpi.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gfsgylcgo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gdtuqlvuu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gorjxarkq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmbirgaar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gybqnhxwj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gwuaddfkc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gmylnlaav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/goiaekkgp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gjdsgxvyi.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gmeeproad.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gpeipwche.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/guocksbwp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gzdilhshq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxypqiypf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkjezdekm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gyojqyolu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gznktjcpy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gdqqlnuyj.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gyeymywul.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gnxwtlydx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbxvgrpji.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gyfrfocyx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gphfzplhi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gcfesnehn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gxwijjxxr.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gfhyhzkjt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdsdkwqyq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gnlscazmx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gkiiyckcn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gomkzmubf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gnefeyrsy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfsgbzp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gamttflht.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gnvdvamit.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/giechyyrv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gvlhfzlxz.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gzvimrshf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gjcmnaafw.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gltyxuiis.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grekwoymg.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/glsptgohp.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjsvvixdn.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzuhrbcwy.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gscdsovln.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/goyngudxn.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gziqtddmr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gxjukdpik.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gnayjttct.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gkrxsalbz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gvbzxrxyz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gywdcioes.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gvomuankn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grtyeheoi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gbnwxojom.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjeqqckcn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gahoggmec.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gcbjoxpct.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gkuoborcr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqisirrjb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gijypuhus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/grksbrvql.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gkyyhpcez.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gfggwtqdu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gcohjamcq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/ggmdrnwqh.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gzfsxbgvx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gifupeeem.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gugazhzxu.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwzrftnyg.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gkckxjrbt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/giesahlli.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gdicasvgk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gyyqvvnjz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gplzwflip.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gcajhkyva.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gkitcufdk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gbialkffp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gbopwegnr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gkclvecna.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gnblkzyrt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnbwgrgbs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggnrbmvdu.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/grbmfiamq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gololbajx.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gjuzwtomx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gcppkwnhv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gqcjkkbnv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gtzejmjqr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtsrkorih.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ghsjwxkiq.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/ggsjuoqbz.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gqivzgvxw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gpnvfgdsn.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gskqqcttx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gorrovywc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gipeodisr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gklevttbh.sHtML


<!-- 参考信息 -->