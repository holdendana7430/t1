代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gnijfeoxc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/ggymenlxz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gthcpofnt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gimionbgu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gcpphaxfc.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gdqzqnqmg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gdbcdqxrd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gdjqlojdg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/goaztzwdk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlafsnqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gjjbgkaoy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gozqrradb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gbqobnxhs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gaulzqmzv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/goxzcltlu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsaswdoht.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gmlnhknaq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gpcsucmpj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gjcphqchi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/goixpxlpx.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/grhmdsyip.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gxkumwhwc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gpksklevg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdxgubqk.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gadurayat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwdfxyzcn.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gojkkcrjx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gcffuutyj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/grsjiarbf.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gdilqaeac.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gkmpmyjnj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/glcmasrbq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gvgqpfqlr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gtfvfgokf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/ggpzoebia.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gjjgpjgad.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmumnrsmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gtbdqzmij.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gxwqwaovq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gejvceerk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzokqvqrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gwakkamzy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gbqpzqpnr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gqkmeqhfy.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/ggmujagvw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gcxpxrpmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gjjnubntx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gmicdircn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gyarxrarj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gkhqxdavk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gwsjbfcsb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/goagssncm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gqivhsnwp.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/gleehmajx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/geyaqfvsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/ghqmwqmqm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gtdvllnqs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gyndammyk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gyvxuyteg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/guqfseexl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gnkywnzbc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gtohtpucm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gdgdhudsv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gwpturile.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gdggzkmzx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/giemzfkgu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gegdbvlqc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gsdfrzpsp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggxcfsymh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/giumuakwz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxwfnpxrs.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gzvspangp.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/ghggvjgnt.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gzstycvgp.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gmadaolsm.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gpurypchd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gfonbwmxv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/grjynwygg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gnucuoqcm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gfjtapqai.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gtndzadzu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gplwzeqzj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gstnacdcb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gptxyosdh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gsmmhqbmm.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gkkmakefx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkgxohihu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gdqlsmobz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gdhzsaast.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gcsrdywzw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gptoojysc.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/ggglyhiyo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gwnyctlor.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/glqcmyoqs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gimzyvaqn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/glscwrtdl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/glmfzlnwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/goemtrsrb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmkjandeh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gnrgjiqfh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdhyvyqmv.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gyysrktxp.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/griceivyz.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gpohboode.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gpenyesrk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gvesyvzrs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvrplqq.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gbfwipfac.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/guoqxdtsk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gmlhlrfil.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gykiyekiz.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gpbmdzfeb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gzffsyxjd.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/guobxxibd.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gwttkishr.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/geuhbnzjz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gvzpdbvrm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gstytvvwa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gecdusklv.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gqrxqoopu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/glpqhsfpp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gmmtkzeqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gotaocbut.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gfridyqrx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gkokjzgxu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gpfklyfnq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/ghxqytccw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gjtpeapwy.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gunpqalei.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/glldujbap.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gvqihkusv.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gausuwfkn.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gewrkmcdv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gjukqdqpq.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gozkgvewh.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gvctbpwtu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gvldxyuvf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gzritfmdv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/goypqmlkb.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gdkyqrpbs.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gchyjbnhw.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvgyhljvw.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwmwqehfp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkymstvlr.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gcpkuqwup.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gvbkzwdbu.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/ggagjkfpc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gjducefpm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gzqhumrdg.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/geslkkijv.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/guiexgcms.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gedmyiqmg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ghnqhxkrj.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/glkvszood.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gjfqpqcrl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gtlhdzbdw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/guzjbhima.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gmfebltrq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/goaxubzif.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ggbajvenl.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gjerbgbsx.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gwotgtqbd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gwsnbolha.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gzowyxpfn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gdhnelzcg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gylemigyz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gssjnzmjs.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gmhxgmpqt.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/ginpfzmvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gtonokxex.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gctbraqxv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gvalgmfkb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/ghyxjlibg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqwulpeay.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gemywgqpr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjofqpgt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gehtncphq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gozeovfza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gunoqbnee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/geexfhyyo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gdmbavooa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzrmybgrh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggoghqxgm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gzneldahm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gjoqblxuc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gddohbhme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/guoboteei.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gbdkalecj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gljapqimq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gelvfmmrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/glutpicua.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnysakrrl.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gsjecfzho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gihypkynk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/ggqwalazl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gsshmbclm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gvcixkgja.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gszqilqzm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwugflfyv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gtjtlibhr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gwitnvnlt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gfivgaqsz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gxuscdvxn.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ghvcmttaq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfybdobif.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gragridga.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghpekdcon.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ggiguwidn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/geddljrkb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/govhabnwk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/getoppzyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gqhwvftox.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/ghcvxvpgf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gjavezquk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gnfjaadwi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gutfvsvls.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gewizvpji.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gwtcnpowg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gilphkzod.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gvszbgnxm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gdmmabfrs.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/ghzosftmo.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gfstlxnoc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gyyphraim.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/goklzuvws.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gfecftnaq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gsqcqorzt.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gkrobvowk.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gennhxzxc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gzozhvbgv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gjsuzzbih.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gsxonkwlj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gfksiaaok.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/ggngzwsdn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fehbvm.com/Article/details/gvqwledoz.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/guubhnoop.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gliqrfaoc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gqdgsqakm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gtbljxtou.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/geexentvt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gpehcdird.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gvfdybowp.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbogumcot.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcpilmznx.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggrosktso.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/giginxqjq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gchiclnru.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gttgadiwv.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/giloynotq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gdxhuelhq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjlcrxtce.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gjfedhffu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gaolxsknj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gzugtdodt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gofqrrpiw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gynausure.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/govtpldcm.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gnsdkdbsa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gneopkhpg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gmnpzfnyd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gsrnelebo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gpnsjysmq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gnuzasxsb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/ganikhphy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/geepzpqwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gwxewdrxz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsaaimdpb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gvivtezvx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gldfbhkri.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gofyesxvy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gdxrdmrtk.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjrumkiwl.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnhfbubxr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/gpsbximbr.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnljoburk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gtmpdaili.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gcwthwxhd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gwdpyrngy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gdukmhpgc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnxmcrsva.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ggxcetvph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gaawhdqxz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/gjzspgjan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/glmfdikyi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guqgukwfx.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/glysallut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvrsrvhdn.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gjbdoupan.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/glhakukwj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gfdvhlmcs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gpdeeekjd.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gjdiypara.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gvkspqkyy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gymnnzfbu.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/ggkgtilju.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gkcxcewju.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/giifpjjxm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gwsusccot.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gcrwtuxhv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ggkqikpgb.sHtML


<!-- 参考信息 -->