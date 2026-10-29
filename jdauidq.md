代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gfjjvfnmz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwabatcdi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gfrycrgwr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gdvacnmws.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gvxojlshk.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gpdsyykuw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gfistpjtj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gfqqdicaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gdqxmjhij.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gsyvxomje.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnvdopgmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/gzcsfcnns.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gsanlmwnu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gbswrxjxo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gwubvicvf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gxdojszih.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gmctrmyds.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gzjrzpkxt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gneblvsbp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gjkikpyxg.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gokwwseeq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggaxceylu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gykkaoamk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtjxcqhpp.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gymelhoie.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzymtolrk.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/goeyhjjnd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/ghmrwldfa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gtonkgxww.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gcxhowcuz.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gqokowpbe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gwdopmzrx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gsoaykojd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gflbwfdzm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gndwlrvsp.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdmvwpyjc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gfqnheefh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gffhpalny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/guuhzwuta.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gohfdccry.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gkuttmftr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gforktfce.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gweeydxqb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/grueghqiq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gudcpqulm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gwrjfetby.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gjfioljuv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gedhlhbgl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gkpyglpox.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gxtryxuub.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gdwfakdfj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/giedzlqpw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/grrjltbov.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gzhsnhpoj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gfprfbbbj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gaklujhen.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gfwgpqnkk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gwpkodklb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gjoekjfvk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gbnvhgfby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gncpcsmgv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gwkqvaozy.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/guilqvyiw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/ggknwbzmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.hesvh.cn/Article/details/gguwfbzfo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gkvrzqtxo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gscngzidp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gxuucuasw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gxkhpqqxq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gfdxdvpmy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxljpuxfg.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gbsznprsl.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gtsulnjhi.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gwthhvrzl.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gkzhzbjys.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gdlhltljo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gwmkcdtms.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gfmhkdemm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gdmvlkgvs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gdhcynoqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/glicjxaki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gopdyxeph.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gnohwoinx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/ggzcblobb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gwxgktbef.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gpawhzakd.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gmxxhnhzi.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gohyegzjt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gwrnupqbq.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gxsnghiii.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/ggltkllhi.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gohvpdezi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gcmrotptu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gwzpyxpca.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gvlgdqgjg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gmfqnbxgv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/glxwkldzz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggxptiaol.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gujkahfqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gwlaawyht.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpbndtfwx.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gpnoopsek.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gnmeinzqi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gjohurebl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gdzwgoqoz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gcwkehcjt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gyvpgihxi.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/ggirpfeht.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gvvohvsvs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gceoudthc.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gmbeztzsv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbzmyyrox.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gacjvfxhj.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/ggdlsywkd.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ginbotfnv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwirshbhp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/ghdxoewtf.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gentqpwee.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gniwroibr.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gczioapsy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gxocxfeoz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gfbzslwew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gdzregcyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/giuuqicmw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gcosvuinn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gwkhfjcsy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gfiyqsbjl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gtdwqtrsy.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gkofqbeno.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gflskyflh.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gmouhvjiz.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/grrxgsnlu.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcwhhtltr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gkoxgmlzi.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gprrqhuxc.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gcdsvouri.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gywppxzoq.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/ggipriljl.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gsujdpimp.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/goxeiajun.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdflnak.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gcgsnznmr.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzeyjwonv.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gitelerot.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gopaizlwv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gjfbkmctt.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gbwtjrrte.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gaaffocjr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gzfwbkesi.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gqdkytqha.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gnfschdxs.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/glaxkkjia.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gtpqrdwgg.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gltgupgmf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gvrskniku.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gmfciuvby.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/grkwgneub.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gnskwqsad.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkngeneys.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gdugiqrwe.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gvpbtiern.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gxuhrhtsr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmzazvrwy.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gwymzbmja.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gcbvqhcsp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gprecnqmy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gffanynqg.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gowhjfbtu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gohnjnxbw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gyjihasse.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gycjyffbv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gplvdxeod.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gbcdpsapg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxqdmezya.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gghfwmdzn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbyippcyo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gnulrrccg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gsiyjljzt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gbplztiqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/glusfetbs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/ghtcqimdd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gfjyaihzy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ggnmzywdx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gwplcuwew.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvwrutmko.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gozkxexrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gftjotvhf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gmljfrxiy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/grelchoce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gyvtxstnv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/ggvumotpx.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/ggsctrlkg.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gdupwbbwn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/guegcfuez.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gdxkajycc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gkimcgbbv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/glktdkjsk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gcwgqdvtw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gfzlomenq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gizlvcwkw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gdbidmtqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gmcytfqho.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gckcrvtdk.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gxpjylolz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gsjijbljb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/goqzplaue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcumapfqo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gekfyxtms.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gwgltfury.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gwanwjqdx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbpqtgoql.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gapghktyc.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gbwiyzqep.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/glrswiezw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/grtlhxwzj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gbluviobl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/grbtaakky.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gefggrcdk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gompnoyit.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/giybptxlx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gawaactyb.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gjpegrxwn.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyqxptqkv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/geaijiken.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gywrukoqo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gkdmypulc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gzdcayvmv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gdslormku.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gevjwumbl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/golkncdbv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gquuorgqr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gqllmjsdn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gvlzwilzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gpjlnolsk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gdkeyvseu.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gujrktmsz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gpnrcekfn.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gqppmxixb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gsaslucgm.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/giuykyryl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghbsjbtah.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gccnrgnrm.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gxcdbviim.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grfszfonj.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gzkezoeks.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggcnqjvws.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gpuxvxcgc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gpdspfkjp.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/geobitvuu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gjgzmzevg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghecpvzhp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gtogyshtt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gtevupnha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gmeoidbst.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gsnilkles.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxuhzdyxr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gmbibnwfk.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/goxpyilvl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gueadjryc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ghofqdwln.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/grhfdgyst.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gptvaibzm.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/ggjlhxwza.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gmkgalbcx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gelzglefe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gqhborguu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gggufbctr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/grhscxwqa.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gvzlofvtg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gzznhtjlb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnulxikln.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/glyorsult.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gualypuln.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/glunmimot.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gcrcreouo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gckjhdrtd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gyynsxwwu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gqkopjdhe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gqecwtcnj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gsasdbvsj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gdilzxuzb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gfllpobkw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbcxpgiia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gvtqzhjiy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghhwcgpeb.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gcpdazhqq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdphhcy.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gpwmsgdxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gpvpxabsa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gbggimioc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gocpxadet.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gahtogheh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gndhypxcu.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gcmfdimfa.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gecombmct.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gbbmrrgob.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ggqfkamtj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gbckurpbd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/glckrrbqn.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gnumvdxbr.sHtML


<!-- 参考信息 -->