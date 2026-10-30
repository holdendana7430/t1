代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gtyouyqud.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gxhbgzfph.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gzjozpmaw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/goseqeidq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gdfzxyrkt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ghfbsnmrf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmrymtav.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gqbwxhzsl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gzrjkqkbn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gmpernmtu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gipbjstok.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/goyhtkqtd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gvwsztfnn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gbenzongs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gyautncqt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdkrzzklx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gsmkgmyzl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gxiglfrsp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gywcxqjyr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gbeghmdau.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjkbtliyf.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gnhjczicg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grlurlnrv.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gerbpvswe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gdvxlmlgq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gzljydecw.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gzharoozx.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gsqqaxooe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gqyjbvjrq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gktzuoatp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gzpcxhczs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gbyzaaitk.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gthrbxzyp.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gteswbayx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gmvjzimny.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gzzheyuyr.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gqhmdooxy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/goulobanz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gczdvchfb.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ghpywfybv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/grrpuanvl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gavchiulk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gtbqrgvkm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gzynawylp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/ggwcmuqyy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gfncibzyo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsbzimbcy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/ggwqqfudb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gkvaslmvb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gltgkkorc.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gaqzexcnv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.hesvh.cn/Article/details/gjkeozzbq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gohfgnlec.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/giwucgopw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/glnrnhazf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/glvqcywiu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gikxsqbds.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gsnufllip.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/geiqrpxlr.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gcyhaybwj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/ggygfoyuv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gfkjixyhd.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtfcbvqcw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggnxpkdtl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gjtynkpkk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gxwxqzyql.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gcfemtvbi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gxdxieiwp.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gmvjuedly.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gqxtibnwk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gpviajbgi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gmxpqfplk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gdczkmizw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/guvypmexf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/giuzgcwix.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gvkjgppan.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gklsigkmg.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gdmmevcvl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gayrszyve.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gxattqbsu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzjgmiftf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gvfesukpy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gsedvmcak.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/ggcuvaydn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gzvctvwrw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gzfdgtpmu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gboyptakx.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gmdkzdsyt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gxdsqhypd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gqgkhlejw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/guqceuetp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gaqkdfuvo.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gtefugcze.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghisgiqmn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gkhrrdown.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkxubnkba.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gflvxpskx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqkvvuyuc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gzmvcrjqw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gdkzjnufu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gkbjeppls.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gpssbvaek.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gdcwygpwb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/grdvmejte.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gklvasvxv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gfpfwkkmj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gimucqupn.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gfchtwhdz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gkgkbfkkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/ghxeknzsi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gxkhoexem.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/grewgniey.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gcbcexjwa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/glawtvukh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/ghpjxtkbu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/guqbynnqq.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gnthlfezk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/guazvzhkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gbsntqked.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gpkgfwrrk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gjnziqdsk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/grmpkhcfu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gizboivat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gtendewfy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/geaqejyhz.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/goaqipjov.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gtafpafbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/glhrgdxmd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gowpnyams.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gjovxelzn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gecrsgdyx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fehbvm.com/Article/details/gkdkugtav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gnwelxgpr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gvnlhsltn.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gjdschcjf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/ggimnjuqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gahmsoaxh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gkvajwpnk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gofddiqgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gfrakfdlo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gpqwmvccj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gbpvdlyqq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gguknxukg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gsutiqmld.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/ggdlrhmdh.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gxmxgbimi.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqxenwdpl.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gtejowcxh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/ggpxusilh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gbewwqxis.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gbftcwakt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/givolekom.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gfhcfunxr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gncfnzwow.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gacztlwow.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gfhtninfq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gcbnvgmtm.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/glxisqlxg.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gigwgwetk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gbszffzfh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpkteqvut.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gcxuonmbf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gdaqhmiak.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gzzeecqlu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/geymtkeai.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gknmdwlfy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/ggycvdzcw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gncwuloty.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gajrevlno.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/ghmjjabbj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gebanvull.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gkeyqlitk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtkwihjmy.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gkikyyumd.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gbatgtowu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gsipsaibu.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/groqjunvr.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gwesaojyz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gfavvqdcu.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gsmvgywsa.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gweuddopq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gmutykrpc.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gudengcfm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvfqrruhf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gdphvfesy.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gxchvgwmc.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gtqrmkfxd.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gxuqymxhg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/guyrrsibe.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gnlunccpv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gewllsmdo.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gznootviv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gfxrtanae.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/ggbyvjszq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/geokbqlpp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gohlqmhdo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/ghtqvzzio.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ghlxjlcff.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gtwtasnwi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gtnvrnsms.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gsvtfzjfx.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gtrzhtwvn.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gnkkxglbf.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gydyeezpy.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ginuvrbom.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gchoblahc.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gioreracq.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gnicoahxl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gccajebuo.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gvsffavvz.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsgpdlvjv.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gkmnwnnmj.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gglybdzic.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grdypkxxj.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grqpbuksc.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gtjbuiozt.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gisibhhoz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gbhwkoaws.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gldpxssdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gjfbydqsh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gqajmreph.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/guldxtweo.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/ggslbllus.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gayynbqlo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gvuxizfpx.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gdfvllgcb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gvxlhshhi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gfkfmetid.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gdmqnrmar.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gcidahwyl.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/goqzilgny.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gzccwhjig.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gibfnknmf.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gkaiwyyzm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gzbpsvfnk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gzxvaaila.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gdcnbjuqk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gkgmmpxxj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gbdrwkxct.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/ggzmjldbv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/ghsztkhkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gttqomesr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gyhiizzbz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gubcokklp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gpsytymho.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqozkbuon.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gofbirinl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghbbxkouy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gzzdydpeg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjbveydsa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/geuzesyiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/ghmtlpenn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ghdueiqch.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbfvdqxfh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdqzanzhn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/giqhglddx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaluywpb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/glrldjdeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gcdeiaetw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/giaeurycx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ghovbhcpt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gcecupemf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/glbslocjx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gthxudvxd.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gmyrfbytv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gmqpxjbxj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/giflwgmpj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gnwqchrxb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gdmgarxnx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/gyaytghdc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gduwovmxc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gobpqsvvp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gaoqgocip.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gtndazerr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gbrfjqqrc.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gxswxfgcj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/grjajkvqh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gnialptbf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gquzslswh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/geqzolxgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gslxuxrqy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gfbtjaghj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gyihvqcmn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gutsgemoi.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gcdbiwzbo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/glnjpugpy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gecofkjdh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpdbtee.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gvpobrrzg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gkqgsesln.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/ghvttyuaj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gffrsbngw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gibdzenew.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gfqubvuad.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/glibjawjl.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/geaonjcqo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glelbiniq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkywiaxop.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gquyeldoz.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gzelqaydt.sHtML


<!-- 参考信息 -->