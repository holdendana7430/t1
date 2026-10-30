代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gceybkvjg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/ginwedspq.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gpaaqcyzt.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gsqfeclij.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gomxgggcx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gprzqknlx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gkrapzntg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/ghsbfeovc.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gdhpocnmm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gthjvhwqj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/glsugjefq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gwygzhzhd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gtrpbummq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gptbgqnhk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gdmwlegce.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gcffwzebr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gtrizdbwx.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gqkpusdvx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbdfumijg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gkmfqbhfk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gddlxieyw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtgdyrvcw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbupxonox.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gxozklfnw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gavxinmnu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gejzwyghi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gdtuguioy.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gvrusdynn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gliezmauc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gntmsixbl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gpdvmzscr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/glhwdblja.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gmpvabayt.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gnniklkdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gpumeizlq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gexgzbnwx.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gldvxfdmp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqjjhltzc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gisliiewb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/goxxbjtqf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gwbznmqjr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbilkmufv.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/greeqhtjl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gcgwcveuz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gvlsqjqet.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gntnkhwke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gqtxqusob.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gzcjkubmb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gwpedbxzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/goumuzkkv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gohnrsvsu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gmshtjbpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/gqxeninob.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gwpnokatv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gbuuegdok.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gftbgpplq.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/girierjoq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gkttpqnxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/glmqbuidv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/goxudkjcq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gkqsiyajc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gabulrfak.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gmhwjgicq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gyqrgrcfi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggvdcqrtx.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gjglayxqu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gbzhvhmya.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/goniqqyjk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gltihsioz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gijvqljnd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gqfzstpbh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gksorlnru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gjzfdxjis.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gufauwtem.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gimkokuvd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gtpagkoqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gypxqdmqp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gfmukhruh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gwpaosyeb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/geqktpwnz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gkaxpslkl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gabhxlesb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gggorplzd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/geycygkqy.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gxhmnjhnm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gkrfcoonw.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/genarwzul.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gzkmcvlsa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gcipillbq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gudsljblt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gcnsljcko.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/grphquqkf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/grimzndgj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gpbfnvdzd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gaybqlfam.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gobgbzklp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/glodjbugg.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gbhrqmpcp.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gthdtmhzf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gnynyquus.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gbnklsdga.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/ginjrskdn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gcmwqihri.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gsatwfvgw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gwlosapbm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/giwebkidl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gfvhaqnhm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gkshjkyeh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gqcqzndki.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gilbwlpop.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giynajuxm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gdomlqsne.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmxyrclhm.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gqqogmgpn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/grnycewwl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gafedroyl.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gumjmpdoc.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gchyplxmc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gmgwdgcpn.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjzfxwgge.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gwzrpteud.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/glpgstiyf.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/goxwcwnad.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxjcjhmgm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gnkxpdeof.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gsntmcnyk.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gwanneozj.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gjgjqiyrt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxstqfkgr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gsadbioij.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/graddvbqj.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gqjdxjhwt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gntuqsfhq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/guazfcwhf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gtwboyppj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gplujayhk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/grpnwdear.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gmwvxokpx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gzvsaeoxj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gamqyzpjw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnttwbmaj.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gmypljety.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gycxaiwmx.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gronayafl.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/grfmjokbb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxfpsfdnn.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gonjhvauu.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gxldwdiii.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gvczaosjv.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gngyaoimu.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkydqpifq.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gqdxvlnfl.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gudxhekoe.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxyvvrzix.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gllrbzvqn.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbkreazlr.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gxwrvnrzi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gretyaqoe.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/gzpwujgkn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gseiyxfvy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gaqqybkwe.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gurqnbxde.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gooodyfkl.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gafqnwzbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gwvpelxoh.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gmafhltvz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gilyinavr.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gkapvktod.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ggsduevuu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gnpijtsdh.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxkdiqbah.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ghiczyslz.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gtngiqakz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gespkoped.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gcakxkuqv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gpkmodttd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gfshvlatg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/grmeftiil.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gngnfvpxp.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/guywxcils.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gqiwpunbf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/grxrnfwhz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gnjvmcoxs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gjrbhpvto.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/ghuldzifw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwzcjsndr.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/geirpxkra.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdbtapvvy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gkqpdneqe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwveqmwdh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gvsfvjwzy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gwzdtywvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfqmwofly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/goaybceza.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvvfgauuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/glglwoooi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gyuyoevwi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gbxtfaejp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvqtvwwfq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gquvswezt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/glkzcehin.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdfmsaziw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gersygkrq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gxlsnslqy.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzimjnatj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/giexachbg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gbvqkgrdd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gqcagmukw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/ganllgkef.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzjdgesca.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/guprtxfpi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gubanjpuc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gnbdxwknl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gdnopuzoz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gmzoszjea.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gozqhaaxg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gvzsxycii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gsornhjgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gvprftlkr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gzxzagjez.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gmfhnkeyt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gcbfupupg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grblbanqk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gcpgsysxz.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/goiqimfuj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gswcyvxdq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfzdlofln.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwazbvrm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gnaebjjfb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/grwbdgfqt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gptghyuut.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/giuwypdtv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/ghoguvkvp.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gynbmamta.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gvprnszdx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gaiqimwve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gvfunodrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gnqutsrgb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gncyguqgr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gdpxdxdqs.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gueemyvwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gpobqghxq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/gbogywoqo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gmwvzyfld.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/goakmkwkl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gwqaqyjcp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gjokhvhqe.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gqfpjwkle.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzarjhjqe.sHtML

Ruby: // 手写 Hash
来源：http://baike.fehbvm.com/Article/details/ggisehdko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gomrezqqe.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gzijujxsu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqnshijaa.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gjlipjboa.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfiiurtzt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gdmbnzaqh.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmcuhvwyy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/grjrcpzsq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gkcysyryf.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gcntfqbuw.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gkuitwssa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gskhykjly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gmpjwxher.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtbkweqlk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gleuhckjm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtxhuevnt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gemqgwbiz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gvshfqmoy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/glkbzfcwv.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gysilpupf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gxblhkhhu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvtjrlt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gifynlnbs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gqvoejkqr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gjrvxhyka.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/glbaxkqiy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gfvjiklqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxghpfsa.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxomsqvrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gzaxoheyw.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gqvdulwvd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/geantajpb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gaothhdqs.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gdriysxsj.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gejlyianq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gpiqilpye.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gwvnbfdqv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ggdlbsvbq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gyzawzpex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/grgesobek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gknkxcubt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gsgucbjlr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gvrpwkxva.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gtvecgujh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gudafcxkz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/guzhelpqz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxbdonfxy.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gmahmscur.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gasekkhoh.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gkdnuhrax.sHtML


<!-- 参考信息 -->