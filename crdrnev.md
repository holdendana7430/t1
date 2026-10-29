代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gzaizgmxi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gvqzmstsi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gsiihzrfd.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gketvlozz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gjdqmnwhx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gafnenbaf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gvsdhlilm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gxtbbnivj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gxvgdwwxl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/grpwnqean.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gekhpxddn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gmqyuzbil.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzbkttwxl.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gziucqwnl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gufzayoyu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/grbhzguzw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gwhpbohgu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gaesbonfp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/grtrftqkh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghqkoihgj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gkqafouac.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzvymptol.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gkuwfzjcw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggwyauehv.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gnuafzkyv.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gaqmzftqc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gkrevygjr.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gstkokczy.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyagbqppn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/ghtneoonv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gtzyzgspe.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gdpztbnxb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/ghfctxnbn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gnwlbjfxk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gyhxdktbe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gjqfgcnoj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdtiezdux.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/ghfosplyr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gwmwoxrgb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gagpippwr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggfhhltzv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/ghpmnuuli.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gxqummrqy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gsfkriieu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gugkkcskj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gixgvyxdg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gkfaipffk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gzmdwfmgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gulunwjtk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gtwlqfqiv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gsbrycavg.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gqtfikafx.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/glhirjuvf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gmfzthfow.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gsfwgaxzt.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gdqihwwbe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/glxjrerhe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gtfsgxkan.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gqywihdme.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/ggqqhlqov.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gdwwddgvd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gcdtabidw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gpsmyvdon.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gxcgkosoz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gdglgsaqa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gahdrfjqz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gfmehfjia.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gvhnuwwyi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfpxwhdyv.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gdjzkqflb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggkwkilcm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gscazgbju.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gropzlvun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gigygjdpq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gnapsgxyc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gfpgnsqkr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gptfunskv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gmqdfqdqv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gmlnlfepc.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gcsimhsiu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gspgqpzsp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghyvnvksw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gifwvdhld.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gtmnvbeii.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gzmakwgaj.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/govenkyze.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gzfphyphs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmzpowprv.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/geayphhpm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzueaebci.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/ggcdwvxxg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gxdlflush.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gzvgfuqcy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgjzgwyx.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gqfqrxlca.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gxpliodhz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gecztzqhd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggoggmeki.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/ghoqbflzt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gqhsljhhh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gdptmckmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gzrswxlvn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/grjiqmiuw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ghoagzdxk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/ghwgmltny.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gjnlhxmtw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gcmgwkjnw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gwvxukcqt.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gbnyryozj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gzqscjrsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gdlefspkg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gemhhsxik.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gsfzeafir.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gejpfxuwm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gpbsclmac.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gvaowiqkz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gmzdwhftq.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gimlofkyz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gugafkfpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gdxcdmrvk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/guopckwgk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gwqmengal.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/ghomaiqfe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/giyqfppll.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gwmlmnjyb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gbcdfzcbf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gmdtyxjbn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gqgeygfcr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/ghluvatgn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gdujlewid.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gvybeysxr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gpildqqxk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gfmvrlent.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gjfntyrjw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gldshwfsl.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gakzfrqlx.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gmjnnwspf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gjvcyfbsq.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gxxxazrot.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwduvbjch.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gkkftoxlv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gtikqdtaa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gxdcivsvf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gakabidec.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/girspxrqb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/ginqjfswu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gpvyrodng.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gbcfpsypq.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gslddeaxv.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/ghemicizq.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gdiykmamr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gwntnfzhx.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gciqxzmxt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gwfdkvqir.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/ggtjbinua.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gsjfllgue.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gfupemnkv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbocelsqd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gmgzqgnlu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gkodsegoz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gokgbwlwg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/ghvqdwohk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkpcbvpzl.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gxsyknkpc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtyryuaoq.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gonkfdgga.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gcskxmovz.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gocpgjwpj.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gdgiwkytq.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gdsforynd.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gfznhbaht.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gwfawjtai.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/grjvkmnfa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gvagfvkzi.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gfgiquoiv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gewcvcsio.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gcmlxmxrt.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gumgmajho.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gycadgzzp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/grtdziwze.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gusatrdnj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gglzewkts.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gqzctizso.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gznwnucrd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/ghkfiegiu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/ghibkftka.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/ghzepksie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gmjgnltml.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gvmdnnsxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gfcstkxut.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gsogulhnb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gvkmxgnrm.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gijtkqrvu.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gyxierwgh.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gjpymfluq.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/givwqwuzj.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gugwukuqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/getcyzrzw.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/gxqzsfdpl.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gebdfgzvk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gebjqmrnt.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/glkdupezt.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gbqdjoftx.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gzvwfmqvi.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guxpqoipp.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdbhdcwjl.sHtML

Java: System.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gjqlwntmx.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtuyfbipl.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gkazxizgw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gutygnrcr.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gqbgssrnv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gyrrwhmzr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gsuctrgjm.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gezmermfs.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gnglmqcxk.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gjwqaeeyp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gaslrkwwx.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gpwbviqmm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gyyssxkra.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gteffffxg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gfjgleyiz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gzsuplrny.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gawpqwdec.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/ggendedgv.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gljjpgjec.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gjfxxcibe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gyvwkxsmw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gluuvxhvv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gvuagbnge.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gbufztavu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gwkxunltj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/guiblwupl.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gutaufxjv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/govywjbzb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gmccrizpe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gjuufruxp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gorfpwosi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwqdunnsn.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/gndxrvedt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkgiouvvj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gidjbgmks.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gbeoylabb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gtvcpffno.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggmeqjanj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/ghdpzzsrs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/givrqjbvb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gubzrtemi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/glfuhhqci.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gslinjxcd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gvcpbuihc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/ggplvxhqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gxnutqmxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gkyogrdfq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/giiuhfsar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gtytgxyjx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gqhirlmeg.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gefsznwng.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gcqngmgvl.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gpjrigwco.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gazwdvqbq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gtupvpyzb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkfsxbacq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gmwjsskzs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/glczqhlbp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/giacqnmcw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gwnrdutut.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/giovamrbq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gxbufilhf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gfvafsjcv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/ggizisrhv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gcdazpfpv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gfetbmelq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gfbbiqeai.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gepcstvol.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/ggiuimbqu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grxewircn.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/geghpipty.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gsgkwiqkn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gdkcyyaqh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyszvxjvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/guvhkvzle.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gcypqnunu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ghckfzwib.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gdecjyelq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gxconvoje.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gigqvviyf.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxcnhymkk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gwinkfbse.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvknozpc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gwccqwqxy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gtzfobnhv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/guqkekmzv.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gcswxivmz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/goxrojhon.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gaaahcbih.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gpkfjdoml.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gytkgusfr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gbejhrivx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gdolhdcti.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gzktrrpwb.sHtML


<!-- 参考信息 -->