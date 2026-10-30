代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdhkdari.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gugwbbpei.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gpidurswj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjpdioc.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gewvzatjz.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/goykbxywf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtefzospb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/greiewjba.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/guwjeqguq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gtjstystj.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbcbymbr.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsinlaazl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyvnkhkh.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgkboapf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaalmpse.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqbijfeu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbfwcjlf.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtaefhbt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzeqayii.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhrtahpc.sHtML

TS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkgzndxa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauomgujy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gxtpifpal.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvymdusce.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guvjiidem.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fanxiaobao.xyz/Article/details/gobrwvvpd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gklcwhwgl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwcocchw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gdrpqwtdr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grekliaoo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhjqglbj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbsyqclt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzquxqyh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbrrphwr.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvsijzo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gbyyuwgmr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdkhiivo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gancegncs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxpdtiqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxbmtaqx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnrtnoer.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaghargj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmujvhzlm.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvdgdldq.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrzyttaa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fanxiaobao.xyz/Article/details/guqoervqv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqecfryrs.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/grlwyifdz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyufeiex.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/ghlhpgtbx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhilghl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fanxiaobao.xyz/Article/details/gmevzcbjb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjytvfzm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzngmfqhh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gquauwwdx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdcaqbmd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gogslomki.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/gyclwtpnz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcvopjuv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gziuppjqk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhfksyqn.sHtML

[K07] 进制转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwiycwrvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaxephml.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/grkbimocz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcgsvtum.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gixwmgjvp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcidcqhb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzckarnpw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gzknjrmtu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gfvaplxej.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fanxiaobao.xyz/Article/details/gwmkujrpv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvgjeksv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrmgaplf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/ghannegpk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxujwvlcz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fanxiaobao.xyz/Article/details/gzinwufzm.sHtML

Go:   encoding/gob
来源：http://baike.fanxiaobao.xyz/Article/details/gesmkfrrs.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvswmba.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooxdoysc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjznvnb.sHtML

L. 网络请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmgtsviv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsauvlqx.sHtML

[L01] 发送 GET 请求
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxwsmrg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwartpjxa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fanxiaobao.xyz/Article/details/gsrhmtaab.sHtML

JS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gecttqlfd.sHtML

TS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gctsgshij.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzftedc.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/glzpvmceu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gkmtldrdk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gobutnadl.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqopsgcq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsnesgfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gmvroiadn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdgmcnjv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gwdanlwei.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/ghffbwlbx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fanxiaobao.xyz/Article/details/gylijwfpl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fanxiaobao.xyz/Article/details/gcrphbjkk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/grooqfgqn.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gtmbhfriq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpopufxox.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrrubbmn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbikzxdg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbkjuqbg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fanxiaobao.xyz/Article/details/ghxgcnwgb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gculxujsn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgtkmomu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fanxiaobao.xyz/Article/details/glltklcmg.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgxgnmf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gerbuamer.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gpfpnbqbw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gllffgsyx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrrixujl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/ggehxrgwo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fanxiaobao.xyz/Article/details/geoixtbwo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gurlklbeg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/guhjjbpaf.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fanxiaobao.xyz/Article/details/gynorpbbs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gimqzmtcc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gvcxtxwto.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fanxiaobao.xyz/Article/details/gsgjzsqpz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gakmvtmeh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmkxoldd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexktkcwn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fanxiaobao.xyz/Article/details/gaqudfxzv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcxkeuic.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjenbfcr.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkawdyyql.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gdzkvpvrd.sHtML

JS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gtkmlaisc.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/gusvghird.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpexurxdh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gedistevs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmamlsbvw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmyofqns.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/glqlcxxgr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddggquj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziucagki.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwajubor.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuiuwann.sHtML

Java: resp.statusCode()
来源：http://baike.fanxiaobao.xyz/Article/details/ghnczhrcw.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfkgpvuy.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/glvapdqgr.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gzisyqwtu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwpvwcwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqammobd.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gvrkjquir.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gdhdylozn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjctfryr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gyhowkdhf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvamkszng.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxvmzrxi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gxrzqodte.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geifsxlin.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkbtxtk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmdwveyn.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gykrtdzth.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/godxkfnzf.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfkfwlsq.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhbqttv.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozobhiax.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gugnukluy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmobfto.sHtML

Ruby: ARGV
来源：http://wap.fanxiaobao.xyz/Article/details/gdjzvpkhz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzcgitpa.sHtML

[M02] 读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/goqprsgar.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpybkok.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gaazgxhjw.sHtML

JS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzvgfblf.sHtML

TS:   process.env.HOME
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjzfemgr.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gbwbuxsoj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gkgefsnvf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbduilzui.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoibmoew.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrdrymz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsvrgich.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwnduqde.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcyfnypn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gfagkspsp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fanxiaobao.xyz/Article/details/gamznvsmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkmehzi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/ggkurdlvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gryqrnced.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gfuucdabc.sHtML

Py:   os.getcwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxbroysy.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gfvkkzxgq.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/glnajenok.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbszcmg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gvvxyxenu.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/grpgpjxgj.sHtML

Ruby: Dir.pwd
来源：http://3g.fanxiaobao.xyz/Article/details/gublstmms.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fanxiaobao.xyz/Article/details/grbhnxhjr.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnvfslbq.sHtML

Py:   sys.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijvfkqnz.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/grhmhbicu.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjgpudxnf.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxodiqqrx.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebqwckvm.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzcymggtj.sHtML

Ruby: exit 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcojtuclk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/gpeirraxu.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gbohkzjvc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiejwezf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvjufuez.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gvbnktdtr.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqlrmwqv.sHtML

Java: System.err.println("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gqsmoebim.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxqnfmco.sHtML

Ruby: warn "err"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxatdzvzp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpsghfcd.sHtML

[M07] 判断是否为主入口
来源：http://baike.fanxiaobao.xyz/Article/details/gzdrcbmsw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gzspgoawg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gszmeilwy.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/glyzumcny.sHtML

TS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gnorgrfns.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutyvplm.sHtML

Go:   func main()
来源：http://baike.fanxiaobao.xyz/Article/details/gwqblqvpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbkfiegh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gkyylehxn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/goxpygvbk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gopbuvhfi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwecohid.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqexkobd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxmwsqmc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccbdvxqn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gwlkijsmp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gspudmgja.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufxqrrxi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbrhvbtnf.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gmfucdtwn.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnifnsqxl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gheqnxzyr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqydlrvrz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizfzypgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/grysqtahl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlnwdhgg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvclhmevj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhdmjock.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkopkkho.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjntpgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdydqsyj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjieeyb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/goblxugvp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpwkoiat.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gucqhvwjs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszthgxch.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzwcvqfap.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/guyxzarsh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gbkwrnadf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gxhizqewg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fanxiaobao.xyz/Article/details/giaibonnw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydgotriq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzreigrgc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmtjppml.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gyxplmjwk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/geatttafb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gnpujpglx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqcjjrle.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/glhnpfvsp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfvdluxa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghfrdkanc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxijuxpqv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geahrxyrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgwionxf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuzqdfik.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcvzkrrm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gahwgiqtl.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebgbljzt.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcgrhhgb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayadlcbt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrvunhx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcpudfnzi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdwogsdd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqbdsbbcn.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmmaftvk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdworcarv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gaerqmmsb.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsthlrjch.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gmaumwmoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/ghxigknkt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmvmvmzr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gelgnlfva.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghnugkjgw.sHtML

Ruby: s == s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcpktccx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfvoriau.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/grkiawkrp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fanxiaobao.xyz/Article/details/glzbiimjx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuoloimi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjfjacy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnqswxeq.sHtML

Java: // 手写 HashMap
来源：http://blog.fanxiaobao.xyz/Article/details/gpcwsicva.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gxokqvzmp.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkwpsefr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fanxiaobao.xyz/Article/details/gyohqqypl.sHtML

[N08] 生成全排列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuwwojio.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqmsrdvn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcugpeuuf.sHtML

JS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gatnkdfor.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzdrhvw.sHtML


<!-- 参考信息 -->