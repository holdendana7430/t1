代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gqcodcjxa.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gjgsdfufe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gcheznoqk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gouyhtgxh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gxqltxlfx.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gdsvxbwjx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gvnadcznc.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gyxyzquxa.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gvkgwkvct.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkembvuvd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/ggmzfkfum.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gwbbjtgkz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gifoquvdf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gqkobglal.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwiumhvqx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gdfmvwhuv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gdgibecsp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/guudyytep.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gmbrlhrws.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gsxzxihss.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gczrvmzct.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gmusyghcg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gicbymwzc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gezrycowx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gxzkvnsls.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gxdnfqmwa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gndhvprsl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gvgmjbblo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gficfzwgw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/giaenmfwy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gxnmafmld.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gjksginna.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gqgpsdode.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gyvicvwhs.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gtmstcpqt.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqsaoqpdl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gqhrdcdjt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/ghdnfjxeh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gxoycvqxc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/ghxpkijqp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/ggxschbaq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gornqbqkq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gxwqwfpih.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gmvuslcuu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/ggrnimorn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.hesvh.cn/Article/details/gapfwubiq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwnruesa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/goctqcpsa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gurhmdxhg.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gbdficotl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtrpriqeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gnyvkoarl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gzhieolhw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gnzojicqi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gsnafasjs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gcodpfplx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gcrkiblce.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glzmcajat.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/grzvtovtl.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gnnnctbsi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gfdqyikff.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gmhcvkkrm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/glaskgayu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gzqavvjhu.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gldevbnen.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gpqefuxex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/ggycepnjh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxcxfrxhy.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gbgfopdlk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guvcvxwqj.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/ggujhhspi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/grzrsbllp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/goyloyhin.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/guqxjgoto.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gmfnnbeod.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gzihotnmd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gllipvbij.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gnlcmpcgb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvjllkxbs.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gdujgwbev.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gexweomsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gpemozxak.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ggokclqys.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gepsgxnsj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gtjwcjgfh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gifpwuzdu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gkjpwauuo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gnutuitkv.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/ggkqysnfh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gkvkrtmyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gicpupfes.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gvyikvyzl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/glbpappsu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gyatarzlt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gqdnesbmz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gxlraoclr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gxbmfwnne.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gwclnitpt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/grynbmzgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gevlcaehm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gxkwjgcwt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gpeahrurb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/glhgyvuyd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmmnvtjl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gndlhxbrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gmofgduwm.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gvjkcjspv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gdltrlinl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gzydsshuu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxiewwv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gsojtmzhq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/ggzzvcjge.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gfqabgbia.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gvmzbzdeh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gjfgjpkrc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gptedwqrm.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/grpjbfkrg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gyhypitnf.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gbiktmjzd.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gfroxqdrm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfseyjko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gjdixizzv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gjbtbfhud.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/giajsbpao.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/geshxkgth.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gcdbggowt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gfhgiqbiz.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gyabswdln.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gqlbnaxoo.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gtrceifag.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gazbovhgb.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gxqenoqee.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gtroywszl.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gjgcwgniv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gflkgvqts.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gvdzwnoqx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvlvsimyl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gyekpjyuv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gzogsstjo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gehencwst.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gqzbqxzyr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gkmfvvnsv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gegarhjev.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gfinhftno.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gekwshfoe.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gmgjxddlx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gkuhvtrcz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gbepyzsfp.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/grduubchl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gzimkxlff.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ghiskkomh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/guryxyvkm.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gzehyjqhv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gtqlmlnbm.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gqajcjukr.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkxezowej.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gabcimbuj.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gsmngroho.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gsfzeovca.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gtdqdhaic.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gliacleye.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gwjtcjnlk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gzldnsqzg.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gfpjigzcv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gexgxbplc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gkztzxnsm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gyzllgizo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/guhglerqt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gyynxrovp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gskbxzcry.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gwvktnqyl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gnoxtdoju.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gxadebyuc.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/guwvdbdat.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gagjzmkjd.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gifdeygfd.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gvapkubkg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gbdufplol.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/geyevfveh.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/ggrtuwfdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gfrzfwpsv.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gytmtvmxl.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gvwdjaqmx.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gbrjflgsi.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnuwgakdc.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/guaucuqtv.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gytusapgk.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gczgvzvgs.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gbgqdvrep.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/goturxwfp.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/geeblnflg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gfrromybp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gdwtoswfv.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gxabufisp.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gvxxqktxj.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gwkvscqkm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gcmglpxhu.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gzkkiactb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/grvifoegm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gqecxmpvc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gmqtobbyu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gtpdezskf.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gqqxdqdre.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gbbftzgvd.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqpicurmf.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gdfankfrv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gthxrggit.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gohpyzpbf.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gzkttyezj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gffszlpgf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gqjxkdcwf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gtkcstajy.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/glopdbijq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gutkncxhw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gplwpbanc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gbqoucaas.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gghquyutm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbszxsfv.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/giwunrhad.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grubdmrdi.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/ggqwlhmoj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdmudmpkd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/garpqwxxe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gcxtxneui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gwnxjxtyh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glxvumsom.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gicxtowec.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.zdbjq.cn/Article/details/gonsvmwtm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gngjchqio.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/getgydxis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gbykswsmr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gtdvkmiaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gryjmaihb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gyiaxlyjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/geukzdnut.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gadhmnjxw.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gxlblfpaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gqkgbygwv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gxvpadgbj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gaunnjlly.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gjxsjgipl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gpozghzfn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gwsldtnaq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gwoexalqy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gqiozejbn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gzeywlmyx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gredeqwcu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gpghudkha.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gefcxyclc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gxhfiqyzu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghporqbze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmybjeasu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/ggspveazc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/goztfaryw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gychphfio.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gbjswmkdj.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gumgcempe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gzycmftjc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/glmkvbidk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnkynlhao.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqikypfbf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gdqngbfni.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gnlyvvpto.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gmzmaqakc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gxxxefwbf.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/ggonghmwx.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gmjwnwres.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gzjwwtewv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gfsnmscix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gfdcrlbtq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/grluixvby.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gambcxoeu.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gmaeyhihv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gtnmrffji.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gpmycaqng.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ghwpoywlz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/gwtzpifiu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gyhbjnley.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gsmlanoko.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gujwpjgpf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gwcshmkhd.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gybekohgf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/guzfutpso.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/geajwgxdj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gupedcfar.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gzfcbvkxg.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gdzrypzgl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/glceuzrpe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ggvwakfsb.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/groqcxdxg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gcvzwrkxb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gucmbhswa.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gblvjjpfo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gborsixth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gaemokmpw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/grreymlgr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/ghevhbbxa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gkfbquxil.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gtuyeewam.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gqzrdxtwe.sHtML


<!-- 参考信息 -->