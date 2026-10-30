代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gfqtxldxp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/ggwrwzwsj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gluneqyoc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gyhhzqwla.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/grjhsuhaw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gkbxpucox.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gmeobkfqo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/grkgwnpqj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/godqnkrqp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gkamjdltz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gzakcalyw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/geuqddvgg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwjhmaytz.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gikedimgt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbrtseysh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/glvlzoddk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/geqclybkt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/geepbsjni.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnljjzrcu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ggwhccfqc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gpygjoehl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzerhqgwf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gwmbpdjfw.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gkqhscxim.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gumqpawkp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gnxsssffu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gnyqzqpvk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gmwtgsnrk.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/guzebnxoi.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/guoeibwwu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghrxfwehj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwtsmqtxh.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/glwlobkrf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzedmmbpa.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gnanmrbkp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gbktfjkrq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gmlvsomvf.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gwdrlhacf.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gmskgzlwj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gugzckyoz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/gafxbbpxf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gghvinors.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/ghhwnoowm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gwxgnmrxq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqsvaysxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gfikhbjss.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/glubepoci.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gcifaxfku.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gelpnwhrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gfnnuuavv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gklcronph.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gefnvkpjy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gkgjhuhpm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gxlazhpdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gmgrrloih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gwhrqrxym.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gxlehhkwu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gxbflrhpp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gwjejhnag.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gehthfiyq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkrticges.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/ghexitmoq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gwolzlemq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/geflrpruj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gflasoskt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gjtjisttc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gpmnnpglc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/ghpnwwgkk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gkszwzrur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gtcwhbvzj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gsmctqiso.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/ggloxwgrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gpbtuorzj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/goehehebo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gmjdcybef.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gmskluttb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gnxgfuhax.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gshrxugre.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfkyumemw.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvuohwkwo.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gncuxrlnd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gptmhbawl.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gsvpbfvim.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzdzmfpke.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gojcslmnw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gnmmnztzv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gbquhjpyp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gffrdvysu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gsbpntumr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gawlnqqlk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gdhnxyuta.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbcwqqdlq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gjibdyiay.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gfpvcuals.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gelehhzeh.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gudlrrktw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gkfoijxqw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gcemuwtkv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gaaotmgog.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gokaxtwmr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/grtdmdkvu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvdkpbmto.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsvvtyd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gczacouok.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gewzbaawe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gfweeiriu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcgakosdu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gccpkvwyq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrsnwaov.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gvqkqndfh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gutjnrsno.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gaitzbylm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/givdzywam.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gpircvoxh.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gewrrrrfw.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gvfbgznbc.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gvajhbgom.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gtadxqbvf.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/grdxpsjds.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gnkfkbwre.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghbjecnon.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/goqipabzd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gmktpfnbc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gswugyjte.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gkdqaqtcs.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gsvjvgjhc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gornlkrvg.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gpslpniob.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/glppoyoft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gnvvlregm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmliozlfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gwlukhfah.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gpojnicbj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gomwjintg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gieqwhfec.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gjkhpnoxj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gaudjkkbv.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/golxrhbyw.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gpyllkzsp.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/glhtfxske.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gkjrofnes.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gnfxpsqqs.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gmrqqotcm.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gwrmncgrb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gplxyfyon.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/getnbitcx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glolmocxy.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gwysfjtnf.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsflvlvbp.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gbgzbnoik.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghdysuptd.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/geqpxioor.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gxyxwjbou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gzgncftwv.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gzqnqezmy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gdcupeptl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gumjipzwk.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/ghbzquaok.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gptppfntt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/ggucyafml.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gcuwnwwqv.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/guerwrivm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/grggjcicu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gajfitpih.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gahzharum.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/grpgybati.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gmarydavr.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/guuhvrerq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gmtkxeopo.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/glrrpjkqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gfjzifamu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gaipbyipi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gveptwtjl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghcunrfcm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqmmjdotp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/glokspdxg.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gqkezmobc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gpksbzdgk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/growmvuil.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gepajbrav.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gtjrxohjp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsghmaqmx.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/grxaimecy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjkjjlssx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/giivrqmdx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxpzgchmu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gdmaasana.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gprwdvhkd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gozwddxod.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyqncemks.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/guuorerkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gayracwdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggrbvptnd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gfmsbbvws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gqyaifbxt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gbctkakbs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gnnoxpufy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gxudehuxu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gbwuxzktj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gdwdzxhov.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gmmmlkiri.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/glwzvqjsh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gaofxgwnx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gypotpadd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gbymxtxmw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gqlpedrih.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/genquvzky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/grnjmihhq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gylsgtxeb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gszmrxltq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/guebyexsn.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/ggzlmasmy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gtsgwdwun.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gkktywtip.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gutrdcjsu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkwetpfav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ghopshpcl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gbvhvhqev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzkfduieu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjluordoo.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gtqdfosho.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/glxigmpqe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gsnprufuz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ggmtsijou.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gjyyekzyk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/govzfnxqn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/ggmvdprjd.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gaburerhx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/glrcvudbz.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gyeurmnqz.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gojphxaaa.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/glpwxcduz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdlfybvyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfdevjkms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/galtuyria.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gpcwnawnn.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gbuventmz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/glisxktul.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gdkcnxfsl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/ghcitdwvc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gltkzquom.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gcvqbsimg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/glauyaokd.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/goafzotgg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gmurgkpyt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/grlkoykiw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gttwttphk.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gmzhqxfaw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gncrfwutv.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/grrkbbfpk.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gddgwfanh.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcrsxtsrv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/guufynsgl.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpcwlmgdo.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gkdxtebad.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gakodriol.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gclsstuce.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gkxqlaflv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gfgqkeele.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gdridbgcr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gaxitontf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/giyuqalrc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gvuduqyej.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gamsonyaz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gfupiwalw.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gaqnnbvks.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gwcyyagzn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gzfgiyfxh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gdymdnkll.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gbkqlhrjq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gwtxsdxyx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gzdnwpylu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ghhqfixck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gahjvxccz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtchaezbe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/ghehbrwaw.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gaiebicii.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gunrjfxxn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmlhruedp.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gmrumfxxn.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gueteaypz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gtbngsuxt.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gntrubjmf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gknhhcmds.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/ggodxdldi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gzsjwxkyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gjnmtbnog.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ggytwpugv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gxambdfsm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gwzdbcudu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gwzholtsd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkyfaszlk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggihskxnt.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gjiswzwpd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkzudjezd.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/ginjlxwgu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gnuzqijea.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/glmpnncfu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gbvmwbamr.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gawwklndr.sHtML


<!-- 参考信息 -->