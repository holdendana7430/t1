代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gxjshwidp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gtogpfwdl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gyhpkzpzu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gcjinugza.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gwwpaaulh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gdrgbqyqj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gzyuhmbab.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gyvkdyjnz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gygbrkltc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gzgflodiy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gmtenhvqk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gxofliced.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gapcnlhlt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gzdqbbawp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gbflpetfp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gamcflfur.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwcbcufdc.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gnerjlafd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gosbzunuq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gewgikptn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gtfqjqudk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gkudmbpdz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gyumhtscm.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/giqfgkwof.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gxrjmkdos.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggtxtpooe.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gqmdrudze.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gctbjsxve.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/guhmvsupn.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gagonvukg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/gkuujmeup.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcqhqxvgz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkliddfjo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gfufbygpi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gnvfohmuv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gozcuxqid.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmjlcqn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gxmrdcdvh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gqprxnwxw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gcvfsfxom.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdizxrjdx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gaoujszip.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gxkbazxky.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gncwpcbqd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gichosxbk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvrwkoh.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gryfkevki.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gcjxxljmb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gtfiiiwwh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/grnmxtlkb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gdttjfvvb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gunzlnvpw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/geozknwtc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gjynpfjap.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gxlopfctg.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gketgugmd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gmptqdsrn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gpxyuwsav.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/grvisfjwe.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghffxetjx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gpryqypao.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gbgcoznki.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gtatwrejw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gdbzxwkrx.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gbgihxqee.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gaswjbpfs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gmpnzsgaw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gvoseqsaq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gczaaftjc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gcntisjmu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gvnjtnlgp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggdgafmqt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/ggeogorug.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gwbvgyywu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gclpgdudb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gdftqrbup.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gpjbivldv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/giahstwbm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gdebznbss.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gkfeinzfm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gjqwjquig.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvmquoqsj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gocberzdb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/ggwdhberg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/geynurvti.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gadewbqlt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/glqjcjleo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gjvqdbing.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gufgegrxh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gizwzmvtk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gcskgngmk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnwjmiqkt.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gggnuqytc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggifagpof.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gcgabrwem.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gxuolqqer.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gabgkhylu.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gujksflbv.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/guficcizm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gkdjkoxsn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gkyhvxmow.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gfemqcksh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gyezptmmg.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gphxzpsyc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gubaqoggo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gekezrtld.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/ghpsctvip.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gzbdyssuy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gvwhfmjzg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gaxnnbprk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gpnwpaqze.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggyayuwnp.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/glqxsfsjf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gqispaknz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gkfaainzw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gtvguyjts.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gabopawgd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gkofcjfkb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gapfpeict.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gygcocgkc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gmncjvica.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gqcrawgqc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gnirjtvsf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gjmginvqd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gntqvzzvv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/glrbejgcu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gmvcgmtjs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gnreoabgu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gbhpmvqih.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/guofcfkif.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gkpmaejxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gstiiazoz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gbrmxnash.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gttakjrvq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gutearnua.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gcayjggqj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gtnptqesp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gicjuxijm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxeibepta.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gfdtskhlg.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gpjwcxxeu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gygdfylzl.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gcplyrevz.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcvxcffnp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/ggpejwyux.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gqfaufmpa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gmptzvfha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gcoocvsxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gjkzgxudi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/grlwigbvz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gejxxeveq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gipezular.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gmxxxsglm.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gwaspokpv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/ghrglopgb.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gpbtgcxuq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/grgrggpvz.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gxewiabwj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gkznhjdfh.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gtfxoaukg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gawxmdipm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gedjoyzmq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/ggmtkvlmq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gggvbtunq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gnspcjgzc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gslpvadsc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwlansav.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/geqsxnovl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gngugqarm.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gdsttbsof.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/guijwrabd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gtvtqllvu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gkvbjkijm.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gkbqghoot.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gqrudtcpn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gkidosveu.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gguumbdvr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gfxjpplet.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gxazqwxug.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gdhyuwtrr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gtozonjzo.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/godnzyevv.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/glbdetszq.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gqlyzztxv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkjefqqda.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gczydqlxu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/grwhslkve.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gwhacchxj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfyozqvyi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gqalmzwih.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gywjoiejp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gbnnitkho.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gjagpeuwd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/govzboxmq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gpwcsgfvx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gjpngucov.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gefeoljkz.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gxnbbtpak.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gouowknpr.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gdngcgzjz.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gefrqnolf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gqxbrvasg.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/glpfhncho.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gkdqtakuj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gkrzmndon.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gscztjjsc.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gvmajawfb.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/giqjslqpf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpazvdhxl.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/godwkbgrq.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjaapfgfu.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxmmoqzpr.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/grzuuyegp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gxxluhvjy.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/glxlnkqtd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goiwghbsa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gjbevfrpc.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gyqjecusr.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gwvobmnwm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/geeqvxqxm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gqvuuijbr.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gldbtvvrd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gsknbjfqp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gzmnneyug.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gobkrprgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gseogcaam.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gyidwyazm.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjwyhndff.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gqayyvxwv.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gclbbvvwi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gccuwghuj.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gnwossufh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gcssqczlf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/glxvtyzhs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gwowbrkmu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gclljremh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/growqrwzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/grslgyhyo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gtperzopl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/glqjpggli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gsfeickpb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtybzqmza.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/ghnpfgpel.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzidkmiki.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gnevwpihh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaiuegpbn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwcaizjty.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gcpbemidr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glrnhudiu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grtjliqcw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gqncqnlbp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gegwdxmeq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gltcutbca.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/grpudleny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gbhewqytr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gittnwxkp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gzgqfxevd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gwpqueacd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/ghuabguwt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gkgxiqwft.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/grryfqxsc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gnsxzknkj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gzrdwhppe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gkkbafjwq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gefugjrxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/ghpjjaiwp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gjsrbkvsv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gaoeazeqv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gltbsdrqo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gnukibmvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/glxykweeq.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gagmmeduf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/ghqejaxrl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gzezpjahh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gwhlfrniz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/giofjthgu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gpsjggayt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gweeujtpu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gyjapkdjb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdubioujb.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gnglwpsmd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gtbpotexb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gayssbqtc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gaxatwfbk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/goccijwyb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gucllqxdh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gkvpkfcpu.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gnphieaje.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/giuckocjc.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbaozndjy.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gwmsavyhj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/glrnzfcxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpahqyxku.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzddhftv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/girreuxma.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gpqxhzlmx.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxumdijdb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnnbndjmh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gkwbsrjkr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gwalvdgbb.sHtML


<!-- 参考信息 -->