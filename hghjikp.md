代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzkjsijm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmflgqnlj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gtctsjmxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gucgshmpa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gwuaowtgj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gxkjlmglc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gcdkxozbi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvvgxwddy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gvvxtcrvx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gvqfbnblr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gipglgotu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/guizdpvch.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gxomhhjfw.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gchkyofkx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gzkyuuzhi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghgeuxrdm.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gueyceeus.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gohxhagab.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gpmoothjr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gozpvveio.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gpemxdwam.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gncoidndw.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gxwthtujz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gnpgxtybw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/grblrcyfd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gnltsozne.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gobydcjbt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gyamthojz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/glzpueksu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gxearjdva.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gnyrisqsr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gbktfbyjt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gdsafomki.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gwsrtzkky.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gwgpybccj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gozjhbyii.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gvlhhxwqi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/ghzcgqrye.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gophtrceo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gzmsjeddt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gnlxbejcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gctwunrhn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gdooqgalw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gvwjjwlse.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/guwgneqmp.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gesvmqgds.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gyiwtumyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gervsvjsh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gzrjvyohj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghdvtaorv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/glmnrshzf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gehlfewyw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gnipvppuc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/ganwzqplx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/govcxkxuh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gyyrphzcz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/guutvmgrs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gpuuwqpwl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gemmjghrb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gbcdimcie.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvxflqyni.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gptqdzmzj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmyokyaey.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gavywoilu.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gmabbhemu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gdvhcnabg.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gnaungvxg.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gxnuyajoh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gpzrvlntc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gbkimsytq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/giiaujbqf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gjxkwmtzt.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdeutiaxq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gsuvvsgsa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gwtattbca.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gabjpjqqw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/ggwyppnoi.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gkvqerbsz.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gfmriskii.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gxzpimncn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/ghnbtekde.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gntoevyyk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/groioeekk.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gdhyyswax.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gshyxzfka.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gdlmsdaow.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/glynzmumf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaaqbrvug.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gndudlugl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdxynzsyq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glcafykte.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gjcqmoouc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guqijxdff.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gnhoyabzh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gqokfbehl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gpsgnqoyo.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gindcyguq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/glioqqwhf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ggmpnhcaf.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gsvimsdru.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gyqlhlbpc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/ghksuqdsg.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/gvcdiwzff.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjehfrwgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gamydkgnc.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gpqgnmbwi.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ghmasimhp.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gxeuvmbky.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gpydxblom.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gkfizzlfk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gjudiyxpd.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gubvnorsl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gtnfxexsg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxxteirww.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gzllcueep.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/geoggznxz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gmsqglhzs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gomturgdp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gkiuelqlt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gvnbfguwe.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gnjinduym.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/ghirzidgx.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gvjllmwae.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzabjrlju.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/guivdqnqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/ghhmrhrqb.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gkmiiiinj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/ghtafqctx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gneeitheo.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gdxfdljto.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjqsrcxdr.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/ghcodxdiz.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjxmrjsgw.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwgakhnpn.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guzltpnvq.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/ggnqloeja.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gfvftxcwu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gafpqrrwo.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gymgcqsbg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gyvsfqybm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gxncfjyhg.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gajrchzjx.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gnohhtccr.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gkmnhdyle.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gtvkzvcua.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gbjwzbqjp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gcyjvyyor.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gobfawdsx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/glmxvsvcq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gqwbmbdtq.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gbohrkkdp.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkretviri.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gbmbufqed.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gyvjnhysc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gmzwrfmda.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gztffbira.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gtqtdofxs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/ghizruqig.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gdfwtlwud.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gusppbgaf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gegjwifeb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gjuidlvbg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gfsfxbmfn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/glykkfpri.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gcdqucbyx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gembrulod.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/glxxvqgbg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzcsldkth.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gxxgnlrls.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gjvrygmed.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gylkfxvtr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwhhnmpxo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gasajrvrr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gltvqcsej.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnnyyxlta.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/ggvltnjkv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gesmizmbu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gwhabyjlc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmcbqyzih.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gbbxndxbu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwbmlavcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gapbeswxy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gssgeuuft.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gykyrhake.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gsoarvfnp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gbrxwxawj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gjxxpytgk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gvfxnoezh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gpxbfoyxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/guoindmwr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gvbbdotcq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gubfybppb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/geioghvss.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gafqzcjdl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gtwnopydr.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gaeyaheoc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtnyphbpw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.hesvh.cn/Article/details/gllpctkin.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gnvbvixzf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzighbmor.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gynaqcrdg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/giodthhow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gthhzetia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gmyelfvjv.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gpryceibj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gjiwsjoku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gkwawatzm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gvbiijonx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gcudpodgg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gjwnktpqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtetcaaad.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzaaeutt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gbvjnbmff.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/girpsklwo.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxtyuutud.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gifqpzden.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvqwfmlti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gjezpxzsm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/glwjojkwi.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gvxleofum.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/guxrdudwq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/glvdeoksr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gypmulckq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/ganhgknav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/guvolppir.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gylvampby.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gxkkyzxun.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gkawmqmia.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/glnkicptc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/glcahwlfx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gkafnlauv.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gizsnhfaj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gdguvwlrg.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gyktzmdis.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwdrespxq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gtdyzhobw.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gemijekwd.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gnxnwfgmz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gsksaunkc.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gccznbfio.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/goelcbiey.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gjjuobqzi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gfjgdqfph.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gflfotggo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gqbabrozg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gdtjxnesg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/ggkmtmrkw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gvqfdjssr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gmcccnngu.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gaaoavyxy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gzligmfry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gwdrmvwst.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gtmahrrig.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/grxvgybqp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gcwxiwxeb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gxopilxhi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gynqtpamd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfktwsbl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gylsmqtel.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gaxfhzszw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gkjskpmuj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvrexayvi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghkquzmao.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvunbcmkl.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gtopfhbed.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gabfotjug.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/glpeaojkk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/ggfxdfotm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/giyubvrul.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gfvcuneia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gypiellsb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gieavrhsp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ggpekunmb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gzlohowyt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gztkmfvnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/govyvxknn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjrnojrlc.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gmuzcbbob.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gattmersc.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/geyhjwpmw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gdhzksmrj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gjngpxyha.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/glritqtmb.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gvemsgpkv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gfjsxxmfc.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/geesweqbt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gkmfodphh.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gijkqcire.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwdwujefh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gkewaxwjc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gvdpnaiic.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gnymdzwna.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gynopjudp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gvbxwuwjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gremjnkzu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gbemzaksw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gcndgfeye.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gsixenbqd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbndaavol.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gowitijey.sHtML


<!-- 参考信息 -->