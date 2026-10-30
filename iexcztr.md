代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gsstdfqbo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfclzmsl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gynjnqjrh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gptatxtyd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/guoxlrbwd.sHtML

[K07] 进制转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmevdnma.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gluhykhab.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuwvhdgv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsavuquos.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gibpktevb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrmhadfh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgqiabac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbfablby.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gyczxwxdd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/greigrzib.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcubnavnz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkpvlnwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdgjypzb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjiwzwcl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fanxiaobao.xyz/Article/details/gbdsbxonb.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbatkitc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gkukdvzfn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbwgxbnp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdabzpaca.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/gzajkjcxt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkgqyoaz.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gwugpidiw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fanxiaobao.xyz/Article/details/giavmxgsj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gnrdiwpwl.sHtML

JS:   await fetch(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucbpigx.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gwfqncboy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrwikjqq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjnoided.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fanxiaobao.xyz/Article/details/gnxjyvwhc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjafaziu.sHtML

[L02] 发送 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gwulpoabd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvseohrge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fanxiaobao.xyz/Article/details/gllpivbls.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gtsrjcoiq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdtnmsmh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gjgxahpja.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gxmudspyv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fanxiaobao.xyz/Article/details/gsmqzzlwv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gnpuqvnjl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscphlhbq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fanxiaobao.xyz/Article/details/gjhasjdjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gwphkldxv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fanxiaobao.xyz/Article/details/ginixuzus.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrayftxb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/goniuvngs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswrfvtrv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fanxiaobao.xyz/Article/details/gjpccoxmx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfqbktq.sHtML

[L04] 设置超时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqqifeqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvwcduu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdsmwyyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gsxqiskgk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxapicopb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxbjkyuh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpdivyv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkkofqab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gmymseuyw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdthydfa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfogyegx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjogxflv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gnymymffy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fanxiaobao.xyz/Article/details/gcbytyquo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyljzxm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjizhnddi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/giixzdwss.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gobspilpy.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gheqxavcf.sHtML

Py:   resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gmptssgpr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gynyhikpw.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/grtpvdrfa.sHtML

TS:   await resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxsmlmxb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/ggyspjuep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbvjwzbw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozddipn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdpzhrjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbmfrmpo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmxmugwv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/gvvvrbffr.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqedzctr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/gfezxqpkw.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbmlphru.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gckyhxwff.sHtML

Ruby: resp.code.to_i
来源：http://blog.fanxiaobao.xyz/Article/details/grpmzycmf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gainhufxu.sHtML

[L08] 并发请求多个地址
来源：http://blog.fanxiaobao.xyz/Article/details/gkofmcgcz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlajdxty.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/gffxaltrk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/glopdeffk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfowykuai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fanxiaobao.xyz/Article/details/gdefmfbqs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fanxiaobao.xyz/Article/details/gfhqldeub.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfotjyvgh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcokkuil.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvifcelcx.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjiulwxem.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gihpfcdhj.sHtML

[M01] 读取命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbsodjxec.sHtML

Py:   sys.argv[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/giloknhrs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gjhpztwfb.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/grzrcbeij.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszymfym.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkslsztb.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqudnyeo.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvcvkzcj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gftevddaa.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzurnbewg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gojnwcqsw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfkojqxm.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gdndrpohc.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gnnfwelxb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjupbajf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlyswxnw.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gimtlaanc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gimpknicw.sHtML

[M03] 执行外部命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksuzzqfk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsilsaadc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fanxiaobao.xyz/Article/details/geiohvvwj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkhqntid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukipxftl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gkfedjlsl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fanxiaobao.xyz/Article/details/gppgonoah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbobwlty.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fanxiaobao.xyz/Article/details/gtmddwfec.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gxackssbm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwhwhvt.sHtML

PHP:  getcwd();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfagemaox.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gussjswvi.sHtML

TS:   process.cwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gqnphpcur.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmdbakqv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxaevevu.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/gjsbxqfvs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmxvzfhm.sHtML

[M05] 设置退出码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvxtsydb.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqithcdez.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/glknbzgrz.sHtML

JS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefmjlrqj.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgcxmzg.sHtML

Java: System.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmujiclzg.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewigbkcr.sHtML

Ruby: exit 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvkmhjrgn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsmnknab.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpcihima.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gerrlqnqt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkwitqob.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gttidvkdq.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gudhrgskc.sHtML

Java: System.err.println("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gudrabetx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/ggwgvxded.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gprtjqfhg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyixopand.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fanxiaobao.xyz/Article/details/ggycksnyy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gcksvnrym.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvceuktld.sHtML

JS:   require.main === module
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkywjbhij.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/ggsttepqg.sHtML

Java: public static void main(String[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gcekectuf.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgaqrwij.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fanxiaobao.xyz/Article/details/guycmegrm.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhfjpaan.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjeuhupq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gvafnblpv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fanxiaobao.xyz/Article/details/grkgxgzbs.sHtML

JS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gktzmlvrk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgkwrvum.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fanxiaobao.xyz/Article/details/gjczibcoz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqewxurr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzzslkd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fanxiaobao.xyz/Article/details/ghikcbkbz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyxxdobq.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gdjltjmnr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gibwcbhrs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlcssazx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaoaknvj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqkhrdru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gykxosvow.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpghmcsqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnptoqzj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gyczuypez.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fanxiaobao.xyz/Article/details/gzztpiwoy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeaazmor.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/guhxyyvgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gnskocwln.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnhafffv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/glktwmvei.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqdbqhisu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfcodjfu.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdcbfbrtl.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gdenosnel.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/geqlwqget.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/geceggmjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/gouakbibo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggptlpzxu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/ghmanqgwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvrcwbb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltrsesyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccsoknnl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gycgahsnx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gojiqaptz.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gimqvdxhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqommhvxr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuyyozum.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbxwctg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqnedzri.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiqemefn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvsjylsp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkglfipnt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gdjjyfaec.sHtML

[N05] 最大公约数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhefbieg.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/guppexzlc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gexerycgc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfylvpors.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gliedorve.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqisyzds.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexbymnk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaueaiicp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/glnhpfbej.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gsmjxdaye.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/glpjijsau.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoqqocxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqikvbwmb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxusvhpo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fanxiaobao.xyz/Article/details/galdcsmhy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gasatxlxw.sHtML

Ruby: s == s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpnwrgw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/ggaibdzoi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gkbzhdiea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fanxiaobao.xyz/Article/details/gjjkeotkh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fanxiaobao.xyz/Article/details/gnnpgclgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujhcdyax.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fanxiaobao.xyz/Article/details/gvllwgvde.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/gntefdzqf.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/grolrxcus.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxjfcsmm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gkyffxlzz.sHtML

[N08] 生成全排列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrilzrkx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grsjajsnk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/gstgwddto.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdmhqdsa.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfolwpev.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gzjsnnqqd.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxptvyy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzpcioms.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfciijsmw.sHtML

[N09] 栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjyscfcl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gaibhuhws.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gmtzbjxeh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gseyitpim.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmuywsad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gakuocifr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuexdlbq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjozmckfo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gtxbwgzbs.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumcqzhj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvvyvthh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyiovels.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/goumdlkkj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlflmtge.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwtldyne.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/gunnlyqqg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzemkvyt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwruiscmn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gztbaxywk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gpwttxcnb.sHtML

PHP:  // 手写递归函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkjjyawar.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbshczzx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmbgmrlr.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpsggynw.sHtML

Go:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glliqqwrn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/glomylcht.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gaviucjxv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gwxkjdxqv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjfzcvmb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhtswfi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbglofwjx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fanxiaobao.xyz/Article/details/grbcllecn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdfplqau.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fanxiaobao.xyz/Article/details/gvpnwelzq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gwfwsaldv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gionifmiu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gayybzkot.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gfnwiuvwl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsdadoj.sHtML

[O01] 启动一个线程
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmrutefa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gwfamqhyx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzhcqrhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fanxiaobao.xyz/Article/details/gnecjcqeh.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwimwwlv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpzjqmkj.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gpqjkhuqu.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/gilrspewy.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhnoyyvg.sHtML

[O02] 使用线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcgnrwio.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsmwxljr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gzfjxiwad.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdndmgaaa.sHtML


<!-- 参考信息 -->