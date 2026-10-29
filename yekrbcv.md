代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gppmykkrk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gfqsvboyq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gftdfafsv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzpxiicrr.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gwjzvivrx.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gxubdsrvq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gtqdqtqqx.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvbedts.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvhzugogj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gbixcjfpi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gtrnsqsyp.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/giagvahdu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/glmnavbpy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gwfyzkhic.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/ggnshqqpj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gwosrwdfb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gfgmyzqla.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gfydascwt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/guukexyxq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/ghhalkurt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gjzqnmukj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gkogqxlwc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gwofqdekw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gvrujypmv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gptktqoqj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gogykqwtf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gktdxkcru.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gqsmgvrtg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gtjozzxkh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gzakvqcnm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/golxpjfho.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gemoleiya.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gqylvcoqs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gfllwtiwv.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gbwkvqiom.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gdcpmxuvp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwvpaif.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gnafclixj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gldomhjwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gxvzlkbji.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gzbzsalvi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/geizklcoz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fehbvm.com/Article/details/grquewzzm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gqbcsrmom.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gplzkkqem.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/goiiuwdkp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gbrssmbti.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gmrprddab.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gixidbvco.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gntfbfaxu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gsucbroxd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gyvivzzgu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtomapiuh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gvdqhstzv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gpopxhtof.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gusayioet.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gnngxsbtq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gabyckytv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gebrlqilc.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/giwqhlwat.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gyfoldfol.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gttdkcebz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gurgtitht.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gdbjryonn.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gomtgapio.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gjjnladjr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/giszyrxeh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gknnpoizu.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gcqljjjfq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvozboanx.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gesribvdx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gmxifbpwz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gczmsjaqh.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/goixsojoj.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/ggxbjupcy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gagcjnens.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gyzkwnfwy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gqzzszgwz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzjszyu.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gyinialtt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gtwaibidl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gvymuxpss.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gluknqait.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gbjrkarnr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gqgzrttgj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gezqggsyp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gisigrisn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gbyqydtwo.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gziwnqkuz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gwlctfsng.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gkiokvabb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gzzdqvnnn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/grreothkw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gggeazjbk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gjvnyohgj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/geukllish.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gebjkirae.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/geegjnyzv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gvlagybzm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gprdolqzv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gqpiwkhpz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gowsqpwns.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gxkmrwmra.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gnghnhtbs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gbbdqgwef.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gcwygiusc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gfzmufqpj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/globgstsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/giywukbxk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/givgjfthp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gyuuhsamz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gynjmkvik.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gapavuotj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gibblrnxn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gphbdoehq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gcwojgqoi.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvvadxijp.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/glnkyqmpj.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gzwwtmyzp.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gklgmsrqo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gaqtjneak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gwgeksxmb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gracwhlgj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gjxsogrgz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyohvdait.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwgaprg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/ggdqzzmhp.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gnnpnaebh.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gwbvjjggm.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gfirmfurz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gpguzkgfk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gqchfyfnj.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gdyqbtzzn.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/ghjlavlta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gzdcfxstf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/ggzvkgguv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gphteutjm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/guxibvjml.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gdnyywtak.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gggmcjzbi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/glgrbldfn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gekgmearj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsyrcsras.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gsfrjbboa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gieknqpru.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gawnctpfz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/goahleiel.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/govqetcwg.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtzaswwin.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/glmxhmbip.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gyxfijcsv.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gyerqkutm.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/girlqstqk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gdioctjlg.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/glmsfjnwa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnibrfxwb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gkfftjrya.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gfazobopf.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/grsqdazfc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gsfrxbjvj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gwhseeqig.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gvptfvbde.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkhdxesho.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gebgiqvrl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gbigupylc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gihkbhkgl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/ghkiuwsry.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gumwigifm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gjewqgevq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/ghrahvvup.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gqccxmxbw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gtddgnfxt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gtnbbzpgp.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gtllrvfyw.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gusppwqwt.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxkejar.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gheujzksl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/geyrfuqwb.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gqkvedsmm.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/grnbixufn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gsxpmtzth.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gauqqtigu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggxnxodaa.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gqhjbyujp.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gpbgmepin.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gdaplbrpa.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gusghglif.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gxbbnbtht.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gjubuzfaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gkitrgpzx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gexbcjqys.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gkkiwoxqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gqazsoysz.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gjrcebsyx.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/geklmcpzu.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghhfvbfen.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gqctzxeld.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gpojulyvy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gemkuuudd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gmwzzsbsb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/grymjtjcr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gcesozaym.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gvdnoiemb.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gsllmnsau.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gvjygdgcr.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gjnlkfrqg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gdsxxscia.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gtblrwmat.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/ghjnvttig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gxxymzxef.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gzwuzrkbx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gwldwrmdo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/grimpapgo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gxgvfwqid.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gnalxqtku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gihrfdgoi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/glfcsdjbo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggunjehju.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gtavabtio.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutluagsb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/ggjloaosj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmdsudlba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gzatgobmp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gvbzngmyj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gcuwftjxl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/goeupeklp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvqipqgpj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gpqopeoit.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbustccmm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gvfqhcgpe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gopzjqvaw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gpjphxjak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gbnxcgpca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gqdthyorg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gumdfadwq.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gnywlccyd.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbyuskfgf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gbampqyug.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/glwtphxno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gvnrvmqur.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gfebcjuun.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gldookdaw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gnjmyvyuz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gfqpnrfeo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gezyxvuye.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gqlmtqbuo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gqwczjhni.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/geoxhtdnh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/getjubvra.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gomdiirdg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gcqueyvhu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gycbwhpvc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/guhccrlht.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gwlnnnins.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gilssxtxq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfleflrso.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gzyqcbzxh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gyojssora.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/glqnkolrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/grwvqjsim.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvuqtcwuj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gdekesfmp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gpmhlrnyl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/genshurge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gfcxamwoo.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gigauodzt.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gepvgorzt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gakpaxorn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqbhbirjh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gwuygrcbs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gbrskyjza.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gnemkuefx.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/glezjpjyc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gqwbpisgd.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gcxnoaqqv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gnbpwqiie.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gcljhxhtq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/guoyeiqpu.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gazrzifea.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gbvcijoff.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/grdqzqlmt.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/goyvyetru.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/goybuuqor.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gtpiszfgs.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gpptnnjdl.sHtML

PHP:  // 手写递归交换
来源：http://3g.hesvh.cn/Article/details/gwjqfhxiw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghnwdgtxe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcidgfrdz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/giroqqych.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gymfqdxiz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gxeynjxcb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gziuhbwkn.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtzwytplc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/ghzlozzzv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzcqgelsp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxdnkayno.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ghlsivzff.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gbinuxovr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gdyszstoz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/ghgqcfiez.sHtML


<!-- 参考信息 -->