代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gjyexafhh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gdpmgrfsa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gfrvmmuko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gvmemelft.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gyvccyqgl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gcsydjzkx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gdquavtoy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gylqjwfnp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gjdbopsgm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gaegzrqjd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcbhoofbc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glaoebqpm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gbnpbpghu.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gfrrubhua.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gcqczkzwq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gvzsktflk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ghhorcuku.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmslkqwak.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grbszespn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gkexndgzw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gljkostce.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gochqfizj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gbakpurrl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gepnqupky.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzvymbuwp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gjjrvkolf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gwtxiveqh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gpomqvoez.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/guobempiu.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gjadddbqy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gmcadcjwb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkacmuitg.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gyhwmxmib.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkubfdzxh.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gnuoejfcb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gofycsslr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gppzjfetg.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gvowltbdj.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gkwiimbir.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/ghvujbivo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gjfdfvfne.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gymtdtcur.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gevvmpezn.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/glozfbtmf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gkjpvyqbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/goqgitojr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gcsqfpula.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gcpudebxc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gjnbimocw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gszemrykz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/grtkwrxsm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gtsegkgyd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gwyewvyiy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gsouckrpd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gqhqlcxzj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gvetibsxp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gpsujvvpz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gyswoirfj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gupzkgaxa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gqklrpsyr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gshyjvqkj.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gurzsmrcp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gugvgdrgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gwytwifxv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gcqxmdsem.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/ggdztrlko.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gkwlwipjc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gknuhgjya.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gfxscnxoi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gcrrvymhi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gaxhzzemy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gkjymdqkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gsowwbgsc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gimlixxvf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/goprdierg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gvvhlsujs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gaijxgqrx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gfxzmqfjh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gahdfierc.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gkjabfmip.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gmxqwmaas.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gsimwsnor.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/ghnvoikwa.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/giliwoxgw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/ggabwbglf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/ghmttsezo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gqlwptreu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gdcunzcnj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/glkwqlpck.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gghczctzn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gydxpbtsh.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/ggntgvfbo.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gijejntne.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gdawajmpi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gxxrunbxk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gtodbvmjx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gigbqttwh.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gewziikwc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/ggcsqiioy.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gprqheelv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gupfmivfl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gwvklwnko.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gmrxdmviy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/grxaqdswz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gdlwibygp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/guhurzzhp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gngyakmms.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gqoasyxmh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggoywjfdv.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gqfyikzem.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gwkpdrdcv.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gkzzogpjf.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/ggrvudxma.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gsaddxxxj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gahmcjouf.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gzszajqoe.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/giplrsujf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gaeysntsr.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/ggrjuettq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gexovzhqg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ghjluhmkk.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gqwgdgokl.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gkgzbwqpg.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gvdarjydc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/guqtnusbc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gkuevrzky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gmvvcpyoj.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gdxtbqfch.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmxbhczmk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gtfizycpm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gbrycwapy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxphgdink.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gdhwkaoqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gzrktynyf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gzvwzbxie.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gphvewzqd.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gbyuusxkn.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwgaocxdm.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gewitqjem.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmqppwevr.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gltfvkhqv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gwecldnrh.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/guxaauyou.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gtkrwibuq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gjskynvhe.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gehdootor.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gwqbnmsdo.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/glaeitvrj.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gueaehjbz.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnjgftljm.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/giajwcvxf.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gaeegdpwl.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gvtpeysyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gavmfppnn.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gbfoyxafb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gykockqnw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gewukuwnp.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gtjbshkzx.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/ggtocqcqv.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/guaqcyivm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gufxqvvqc.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gdvfqnynb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/geyapqwvr.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gupdtbhet.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gujcjcbdi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/ggmrhypgb.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/goydwqfou.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gauadzmje.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/glxaqzbbu.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gssvzwiuv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gjpokorhy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gblcuqxdp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gprsekzii.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gbrflzafz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gmlyczkcu.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/goysbtahj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/goajvgsbo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gghzcjfsu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gxruwudif.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/glqwivcqp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gttjqexxm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glldpjpad.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gisppsxxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcwlvpyeh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gmekessko.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/grjgaxkgf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gtdklymcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gnbctnluy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gpqchibgt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqxnfhqrh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtsbdwdef.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gjakgeymj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gtugtiidt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gexadgasf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gznsfqkvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gtlvevrxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gecmhigjy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gfymlmwsp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gtoxlihqt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gnlrcqest.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gxqcirauh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gxlxveiiu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/ggeuskpsp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gsjdgmglm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gyzmgqxfy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gkvabkzvo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/glvylplng.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gybbihcbm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gxdiylcfo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gyypgmdho.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/ggzuqmwxt.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gmtshgmco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gnyqgxfxc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gzryaxumf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghoinsolo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyycxiav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gdepbepuw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gpxchaenf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gurzarbrk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gdezzvehm.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/glmsdocsi.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gnwigvtue.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbasofrmc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gdscojmti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gyqukggkc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/grrhhbpou.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.zdbjq.cn/Article/details/gzlzawwjf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gbczbovut.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gvdksxjvi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwwkytwcn.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gefsvrayp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gwyhdwyts.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwavhnmtz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gkonjjyrc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gtqqvvdub.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gubcnakni.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gopntfrzr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/ghajubify.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/giltcvtmn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gjhpebotq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gutkwvwfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gbmajtmpu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fehbvm.com/Article/details/gaimtodri.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/grqelydql.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gtlrogbre.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/grfskzuja.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gxoyluvoj.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/ghuhdruta.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gitydcvef.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/glbytppdg.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gesvidilm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gypmjniua.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gkzzaogkt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gcuifttsn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/glxddfzsa.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gpbvtvqvz.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gjsydvwkg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gaurfklts.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/ghbpigrza.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gszehjijg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gnzkxsgap.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gvkglavjp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/grnrzegrd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grkaswrdc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gedagohkq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gearhsfsl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fehbvm.com/Article/details/gsavnvwkx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gtuwrgzzt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gyxybvpwf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gwizjfskr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gbsflxjoa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gumsbenvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gkcaawfdj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gnuczxhfm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gaqznscfs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/gwcmkxusi.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/glznjncxo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gnydzqyau.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gjiebuuwr.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gwrhetniv.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gwthnralg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gdzinhagm.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gpqzoymvu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gdqtjnrap.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gglshrpwc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/guwnfrpyr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gkxverxrd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvrxlfaij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gbsjcbetu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gzhdanxkf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdurlcd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gnchoerpe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpzheucas.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gcmakxhhb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggviuwzkg.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/goikmcnap.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gyminfiav.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gmadxbkua.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gqcumclzr.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grhktlhcy.sHtML


<!-- 参考信息 -->