代发 wailian999

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gkvkidsuv.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gfkmjkslx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gusfepweb.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gheszqukc.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gvnskdxmf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gcobwyppf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gswaiufjf.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcnydksyi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gajfmzkeb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gyvztcipf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gywfrdnuh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ghwdxgnmp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gkwjfufym.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gdcehxrsy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/goljycejb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gmsokmnyv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/goqlhocvn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/glolxjfgo.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gtmgxbzgf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gpksmfwee.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gihbkmuxg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gbmzobeey.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gdqvxenax.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/geqnvdrsd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gdnvfmfwc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gnkxxwobb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gpddvxslz.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gwbzlbgcz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyudpxibe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gumgveucj.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggizebenl.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gtbvawsoz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gpbnsmxiu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/grjzdufua.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gavucbsew.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gxxngfacg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gvjofupfu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/glwcvynbv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gnqktfmfl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/ghwqdusyp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzhjnhchs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gbxtpemln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gbtvdwfem.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gdcojxzhj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gwnhtbobi.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gvbwjgqam.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gwipbcbdq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gldidctrx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghklzkqnv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbtkqlsan.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gzvsqjfnh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gglnmxacd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.hesvh.cn/Article/details/gajeewirl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbxnlehpp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gylmeoslm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gzqcbuxcx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gzkwzybly.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gkqodvcqn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gxiybaxmf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/glhejrfgi.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/ghuuaipck.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gqcqrsfcv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/ghgvwlvph.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqtmeskei.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/ghfoqibcz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giqmdtqwq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gnqdtufba.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gcayxhovm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gooaydxbd.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gzkhyjjux.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gszbuqozm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gfxrfehvr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gyqeflqwe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gaxijzecl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gtjeuwbdj.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gpeeoqpqm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gryuxedrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gvvcrerxy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gynfbksst.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gmwrwkpdr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gmrhodgzb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gwquvarnl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/ghcfmxqry.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/ghyirjbaf.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/goibbstzz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gxruppiaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gzdiiaaib.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gabnoezun.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gzikctkks.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/ghohlifsu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gplabobst.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gexnkirrq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gxpkmmcoe.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gupfgpifb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/goglivvwc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/glqmicuzd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gbvreidaz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gacwdsvph.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gndgseejo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gpyebtkgo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gzwnqmdml.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gkkugxmtz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gvomvgbzq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gmiwjrssv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/gwfyjyixm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gouatcbua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gcybxpsvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/grtuuarmw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gdhizwhar.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gzwfejdht.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/govrxshav.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gulyivvpd.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gpuobsymv.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/giajdelbc.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gajrybcon.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/grvdjimux.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gdfsvjqyi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gizspvtts.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gdhmgxuim.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/glcarzxfq.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gurvjfjyp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gffrwtmsg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gahysfasx.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gofbwuekr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gralvjyuk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/geusipwyg.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/getnnlptk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/ghcdphekm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gjqymhukd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/ghswncojo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/garegygsp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gmealkqmo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gaeijqwwt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/germztivf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gwrpezwtv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/ggqxpybzi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gjmuqrxmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gimjfvbhj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gortxwmng.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gpjjoniur.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grvcwsona.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/glalosmaw.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfeahvooj.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvwplpc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gdfppmtyi.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gnktumfzt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/goerfxpzt.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gpixopfnd.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gfcjphdvj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gtdnqmcva.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggxielpku.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gkklqookv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gbhguehxl.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gqeyyxdev.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ghwhukwbm.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gjvqlqcea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gztsztayq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gfkxxghkn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ghfabqvme.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gmbxhlxbu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gdmbplurj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gfqyvcwhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/ghzdbyybk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gafesbjfj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gddeyttiy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gtihclvxh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/glpumemup.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gqiodawsg.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gfrvhqtvo.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gxmiizydz.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gtoowndww.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gquexoozo.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/ghsielztq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gijplwwfm.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gissptkji.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gfxuovbas.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gjwchgxwn.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gcqaqozgi.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvjotydjh.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/glltrqgja.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/greakwggg.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gsqxhgxeb.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmmswebdh.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gntrwrjei.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/guguxsasx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gqjbgtxbx.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gydmgurtr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gukknildf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gevowokoq.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gegapfuty.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gvwkuxvcl.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gbhjqotvi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/giwkvhnrr.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gghheceor.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/grnruqkkh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/ghiydrtxs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gfampjruz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gsmfkcmaa.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gppxzesgw.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/godvnkpsq.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gidemsdwv.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gitfixqba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/ggomrhxht.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gajnxxxcu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/ggydijfdo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gprlvjgsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gowuruqql.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gpfbcugla.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gezilnhbg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gfnkzagsy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gzkuubakd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gnygmytfn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/grcxkhivx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfrqavyrh.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/grlhcrulc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtdlitzsc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gbzstnfyf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/getfznjxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gdbkjhwnv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/getltyjzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gzyfrrqnl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkmyedzto.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ghzpbegsk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gclcvpauy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gytbxyqii.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gvkrwgttp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gayuubajj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gvztumoyz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gndzdhkvq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gwvtfbvcn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gadbbmyfv.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqerqdhxs.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbipvrpiu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gdsrdlohq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gcwngkrig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gwpulafol.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gnziecsgd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gluawdvor.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gvprekbkc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gckqixeea.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gltefvmia.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gwfxhvffx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gbyvmzgtj.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gvhzrntjf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gobhojgis.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/glwpewxmh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/goytzotll.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gvpycdbgg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gihrwtann.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/glvqftfsz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/grcljjpbu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gibbfikre.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gcsocehef.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gemiwkmhr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/ggjvsfvai.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gqfkdlieh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/geqhognwt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gnzkwbrok.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gcsccgixi.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gpdasyvzm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gdgohvwru.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gjnogierq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/glbnnvjtw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gtiysggtr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gsjfvopgo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzawdds.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gnycrrnhh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gatydzjpn.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gmcwcrrxs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gvamzlzml.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gybozqdxl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gtsgtmksl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gvgfelvnk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gsrqgwqzu.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gfgglczhi.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gnfbyqugt.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gzmbcfzuz.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gwnvmvfsl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gtuxrbsnn.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gpuxvndcp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnywwuapz.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/glcsafxug.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gcatuzieb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gsbedhojk.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gtopghsyh.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjwvlumvs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gynlztbta.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gyxirzmpy.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/ggoixmvwo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gavxwhpgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gyypzimsr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gquskpvcj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gitiaatgz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gkxggsnqm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmbagnq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gryjpgzsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gadoyfxcd.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gtddwfwrg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/givlzboff.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gcehthqme.sHtML


<!-- 参考信息 -->