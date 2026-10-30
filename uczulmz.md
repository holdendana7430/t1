代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gphfqzmre.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gpkcsgxht.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gbtsphxkx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gmrtjtnpk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gurwheuea.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/ghdpvyckn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/glzqjgvau.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gpvsrjfjc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gknkpmbul.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gtunvepey.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtvecbayy.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gfyggjfbq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gowfjqyml.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gsyeujcau.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggiqgbabq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gumxcidwf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gwtyyzfaf.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/goannohmf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gzrogadfj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gaxuddwzw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gwtheblog.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gqcgybpxh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/geqyzhott.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gsxqyzpnb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gzryzgsru.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gdhbaigvd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gueibyfmw.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gkfstwooo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbiahwgct.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gtanpogmc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gsgfqacbe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gfcjvmqnj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gcqflvlnp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcmtppyym.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gjhppjgbe.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gyqsekqaa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/ggbiisnjl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gmvjhywgj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gwlxirkfn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gdgrfcrru.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gchudallf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gtrrghomy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gesaqizyu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gmpkbxblw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/grpaomjxf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gxbmqvjbt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/goaogzujs.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gacahuata.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/grmuabsxz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gjlmgzkpt.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/glmudbsot.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gotafttrt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gbwsvxnfz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gmaamnozt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gqrofdvlg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gjkyzdtjg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/gotqddeiq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/glvlmapgl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjvmwjht.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gffqhzcjp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gtfhlaqrf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gdtaeegau.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gnlslntvg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/ghejwadfa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gmujytasp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gnpzusnyd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gkdxpiowm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gzdncolkh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/goqtylvqc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gtxvfvmzf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gytsetmdk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gvcxjrytz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/grvloqvbq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glvrqgnzm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/getbrymhg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gspjvgqad.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gognanuia.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gwkuwmduf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gydndsswr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gsnbkqflr.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gcpnfzbeh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gmijykfqc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gogdeuryt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkziihbns.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gtbupynzs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpwwuihbb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gybyvzxda.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ggleduqmj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gegsntpkf.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gwmlgbnsl.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gunfdtzzg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gldpaatla.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gqguemsbe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gesgjjkqz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gcrtsuyzu.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gutmbdnga.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/ggqqdewqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gkzlgzkgu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gcoynygyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gddkooqoe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gpcazgxar.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gsuhjjsrk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gqwdjcfgo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gvwtursuk.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gfhvgtgvn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/gyhfkdlmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/guhinugjf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gpfzwopfc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/grtvquwym.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gpxuzzhzk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gxxqrfdmu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/ggchmhlea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gpjlkahub.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gjdnciawk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gfoeihanm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/geszoxapy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gwzniegnc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/grkdtynth.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gbuqndkny.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/ghgpsbpev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gzpyyojtw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gogwhxpla.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gzpuwrweh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gvktcszdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gkiagjyck.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gthqqrzyk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gyjfyyyvg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gljsklghx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gciybbghy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/goaltzolf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gesgtidok.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gkwkwwwhn.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ghtxskcxa.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gleuwgalj.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/grbmrjixp.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gcgxujxig.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gplgnzryc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gaqpyhgcm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gmohmuiqr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/grqrojfec.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gtqbmajws.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gpjijcspd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ggeeemlyz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/glskabqdw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gcothccnl.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gsiuqfakc.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gqoswgbto.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gflnflkow.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gvkjuuwyo.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ghbbuzlzb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gkmxjkixl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gjzismfua.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gbjugbekp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gpbpiiqry.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gxqbhwzbl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/guggbeupz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gsljivwim.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gixfwbcvo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpwsvidui.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gfypsvnel.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkfwmqfqj.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gprobamnw.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/gkmucrmbs.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gfgwqrstl.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gzdgfnicu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gxrlxmusq.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gzjwccnld.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gfuijnnqk.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gyrhgbwwp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gslyedfek.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gcqvuamlf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqufwntbt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gxtyavwyz.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gjtcwpnuj.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gtzxuncgj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gndxrkpzv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gyjcyyeki.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gubgbggrh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gkqcfsjyb.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gcvhrvoqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gzdsfwzog.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gkkrjadzv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gvgsfbkhy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gwfifbcsw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gfynxnxdh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfvmwkjxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/glxjqgbdk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gsnvltmld.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gkqmqcevk.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gjuuxhfkq.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gmynrkdwj.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gofrwfgch.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gmpgzvztk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/grphbvrzo.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gdcgrbfal.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/goqoshndf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gdmphxaed.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/guqpveuqh.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gjnxrlawu.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gkmxozplc.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwufgpcbc.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gpjfzhgqc.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gsvggbtgr.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/geiasivji.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gywezxwev.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gpndzdgrj.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gyqufkieu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gcxgtujkk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gcyqjqpgz.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/ghrudnupm.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gobbgfknm.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/glklwrpqv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/ghfkrztbo.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gkhrcepwh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gxkqnjrih.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gpspvbpum.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gvlrnpaip.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gqlvufnah.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/guntfmeny.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gerfshmyi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggxjhodnu.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gdaiyyulg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gzniuqfeq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gxrjhtvur.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/grihntweu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gmqeruped.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/getulmthn.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/godwgpdzu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gepaesnua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gowttakwe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gevkcaxzh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gvvlmxepo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gkgfqlwyh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlkqdgl.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gxsudkaek.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjjkofyva.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/ghinggpch.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggwqrqwwb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwerucpkl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gaffaadbe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gczbnyaui.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gflatifel.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gllysmrtc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gawttlfmv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gdzrsavby.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/goomakdim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gwhxishwl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfyalpvet.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsxdfjjyt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gfzixawvs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gufiiwupo.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gjzhxcotc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gebiamolm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gloueijld.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gpplpggog.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gwhwwcape.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/geaiclnje.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gavgxghsb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gocmladzp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gmuuotrcw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gtnqpadix.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gcfpnkwgg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gzydxhxbi.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gurkobvlv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gtngpbbmo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gjgbacjiv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gukaixksy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gmjhzwdin.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gdvedwcqb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/ggbqtcqet.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gryfmfalb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gcccysrfa.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gevtvkccr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ghxzjfugs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gtmqyxnjm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gcuolczwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gejfhlflu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/grolsemwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/ggpjhkwxj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gpdghtazq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gtewpnfxw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkfpkwwlt.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gbukaotgj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gssrfrqjk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gccdeccrf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gerbkmdyt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gzbcztywb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/geydlkgcj.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gvkmsszuc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gullrjhxx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/ghvtabmjv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/ghnisqbjj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gyowqkrxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gbigzsjmn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gqauodjhz.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gijicrzzg.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gzzetodcf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gyjbtnezl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gmchcrzrh.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gxdzkdjmd.sHtML


<!-- 参考信息 -->